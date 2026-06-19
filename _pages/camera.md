---
layout: default
permalink: /camera/
nav: false
---

<style>
  .camera-workspace {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 180px;
    gap: 1rem;
    align-items: start;
  }

  .camera-preview {
    width: 100%;
    min-height: 360px;
    background: #111;
    border-radius: 12px;
    object-fit: cover;
  }

  .camera-actions {
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
  }

  .camera-actions button {
    width: 100%;
  }

  @media (max-width: 768px) {
    .camera-workspace {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="camera-workspace">
  <video id="live-camera" class="camera-preview" autoplay playsinline muted></video>

  <div class="camera-actions" aria-label="Camera controls">
    <button id="start-camera" class="btn btn-primary" type="button">Start Camera</button>
    <button id="stop-camera" class="btn btn-outline-secondary" type="button" disabled>Stop Camera</button>
    <button id="capture-frame" class="btn btn-outline-primary" type="button" disabled>Capture Frame</button>
  </div>
</div>

<script>
  const liveCamera = document.getElementById("live-camera");
  const startCamera = document.getElementById("start-camera");
  const stopCamera = document.getElementById("stop-camera");
  const captureFrame = document.getElementById("capture-frame");
  let cameraStream;

  function setCameraActive(isActive) {
    startCamera.disabled = isActive;
    stopCamera.disabled = !isActive;
    captureFrame.disabled = !isActive;
  }

  startCamera.addEventListener("click", async () => {
    cameraStream = await navigator.mediaDevices.getUserMedia({ video: true, audio: false });
    liveCamera.srcObject = cameraStream;
    setCameraActive(true);
  });

  stopCamera.addEventListener("click", () => {
    if (cameraStream) {
      cameraStream.getTracks().forEach((track) => track.stop());
      cameraStream = undefined;
    }

    liveCamera.srcObject = null;
    setCameraActive(false);
  });

  captureFrame.addEventListener("click", () => {
    const canvas = document.createElement("canvas");
    canvas.width = liveCamera.videoWidth;
    canvas.height = liveCamera.videoHeight;
    canvas.getContext("2d").drawImage(liveCamera, 0, 0);

    const download = document.createElement("a");
    download.href = canvas.toDataURL("image/png");
    download.download = "camera-frame.png";
    download.click();
  });
</script>
