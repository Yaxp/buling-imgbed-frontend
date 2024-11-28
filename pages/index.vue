<template>
  <div class="upload-container">
    <h2>上传图片</h2>
    <div class="upload-area" @click="handleUploadClick">
      <p>点击、拖拽或粘贴图片到这里上传</p>
      <p>支持 jpg、png、gif、webp、svg、bmp、tiff、ico、avif、heic/heif 格式</p>
      <div class="upload-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M12 2L12 15"></path>
          <path d="M5 10L12 17L19 10"></path>
        </svg>
      </div>
    </div>
  </div>
</template>

<script setup>
function handleUploadClick() {
  // 跳转到登录页面
  window.location.href = '/login';
}

</script>

<style scoped>
.upload-container {
  text-align: center;
  margin: 20px;
}

.upload-area {
  border: 2px dashed #ccc;
  padding: 30px;
  border-radius: 10px;
  margin: 20px 0;
  transition: border-color 0.3s;
}

.upload-area:hover {
  border-color: #007bff;
}

.upload-area p {
  margin: 5px 0;
  color: #666;
}

.upload-icon {
  margin-top: 10px;
  color: #007bff;
}

.paste-button {
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  background-color: #007bff;
  color: white;
  cursor: pointer;
  transition: background-color 0.3s;
}

.paste-button:hover {
  background-color: #0056b3;
}
</style>
