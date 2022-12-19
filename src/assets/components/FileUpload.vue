<script>
// import React from "react";
// import Uppy from "@uppy/core";
// import AwsS3Multipart from "@uppy/aws-s3-multipart";
// import AwsS3 from "@uppy/aws-s3";

// const uppy = new Uppy({
//   id: "uppy",
//   autoProceed: true,
// });
// uppy.use(AwsS3, {
//   getUploadParameters(file) {
//     const presignedUrl =
//       "https://test-upload-multipart-baothg.s3.ap-northeast-1.amazonaws.com/my-object?AWSAccessKeyId=AKIA36DVPTPR7KQCPR6Z&Content-Type=binary%2Foctet-stream&Expires=1671340616&Signature=F6fnvSMTCTqNWeQ7fcDNpF9LcrM%3D";
//     return Promise.resolve({
//       method: "PUT",
//       url: presignedUrl,
//     });
//   },
// });

// function handleUpload(event) {
//   const input = event.target;
//   if (input.files.length > 0) {
//     console.log(input.files[0].name);
//     uppy.addFile(input.file[0]);
//   }
//   // uppy.getPlugin("AwsS3").openModal();
//   uppy.use(AwsS3, {
//     getUploadParameters(file) {
//       const presignedUrl =
//         "https://test-upload-multipart-baothg.s3.ap-northeast-1.amazonaws.com/my-object?AWSAccessKeyId=AKIA36DVPTPR7KQCPR6Z&Content-Type=binary%2Foctet-stream&Expires=1671340616&Signature=F6fnvSMTCTqNWeQ7fcDNpF9LcrM%3D";
//       return Promise.resolve({
//         method: "PUT",
//         url: presignedUrl,
//       });
//     },
//   });
// }
</script>

<template>
  <h1>Test uppy</h1>
</template>
