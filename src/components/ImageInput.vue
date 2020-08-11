<template>
  <div class="ImageUploadContainer">
    <div class="fileDragBlock">
      <div>
        <input class="fileInput" type="file" name="files[]" id="FileInput" />
        <label for="FileInput">
          <div class="uploadButton">Browse file</div>
        </label>
      </div>
      <!-- {
      this.isAdvancedUpload() &&
      <div>
        <div class="{styles.orText}">or</div>
        <div class="{styles.dragText}">Drop your file here</div>
      </div>
      }-->
    </div>
  </div>
</template>

<script>
export default {
  name: "ImageInput",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
.ImageUploadContainer{
    width: 40%;
    margin: auto;
    display: flex;
    flex-direction: row;
    justify-content: center;
}
.uploadButton {
  width: 170px;
  height: 40px;
  background-color: #007dba;
  border-radius: 4px;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 16px;
  font-weight: 900;
  font-style: normal;
  font-stretch: normal;
  line-height: 40px;
  letter-spacing: normal;
  color: #ffffff;
  cursor: pointer;
  box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.25);
}
.uploadButton:hover {
  background-color: #02557d;
}
.fileInput {
  display: none;
}
.fileDragBlock {
  border: 1px dashed #31708f;
  border-radius: 4px;
  padding: 30px;
  background-color: #d9edf7;
  text-align: center;
}
.orText {
  font-size: 16px;
  font-weight: normal;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  padding-top: 10px;
}
.dragText {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 18px;
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #333333;
  padding-top: 10px;
}
.heightGap {
  height: 30px;
}

.changeName {
  width: 50%;
  height: 42px;
  border-radius: 4px;
  border: solid 1px #f0f0f0;
  color: #818791;
  padding: 0 10px;
}
</style>