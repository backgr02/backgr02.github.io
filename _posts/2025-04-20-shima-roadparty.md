---
title: "志摩ロードパーティ ハーフマラソン2025"
published: true
---

<p>2025年4月20日（日）に開催される「志摩ロードパーティ ハーフマラソン2025」の 10km の部に参加しました。</p>

<div class="photo-grid">
  <img src="/assets/2025-04-20/D4D0574E-4958-44A4-806F-8939E9BF9030.jpeg" alt="Photo 1" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/DB103E60-8778-4FB9-B8CD-A3384125F754.jpeg" alt="Photo 2" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/186407F2-5BDA-49FC-8AF0-2E5AB3D88154.jpeg" alt="Photo 3" onclick="openModal(this.src)">
</div>
<div class="photo-grid">
  <img src="/assets/2025-04-20/D244C895-67D5-4700-86ED-1ED2A072EAB5.jpeg" alt="Photo 4" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/5091B24E-D78E-4E04-87C4-DE1D1C7E62C0.jpeg" alt="Photo 5" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/5CFA83BF-A4EB-4199-8E46-AC437C80A45E.jpeg" alt="Photo 6" onclick="openModal(this.src)">
</div>
<div class="photo-grid">
  <img src="/assets/2025-04-20/BD9AB53E-BAD0-4669-A2AC-F044A0C18DBE.jpeg" alt="Photo 7" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/E3079483-47EF-4FEE-9751-C54A36E3CA21.jpeg" alt="Photo 8" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/6C3AA074-37DB-485E-AB6F-B278AEE321B8.jpeg" alt="Photo 9" onclick="openModal(this.src)">
</div>
<div class="photo-grid">
  <img src="/assets/2025-04-20/8937AAE3-44E6-4CBC-A6C6-F47E077AF2AA.jpeg" alt="Photo 10" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/EB0A5E1B-AFEC-4CFA-835E-A26A838DB4A1.jpeg" alt="Photo 11" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/7B37F259-9F08-4F12-A079-2B62B48A957E.jpeg" alt="Photo 12" onclick="openModal(this.src)">
</div>
<div class="photo-grid">
  <img src="/assets/2025-04-20/7143F58D-0E45-402A-8729-CEE016D42AB5.jpeg" alt="Photo 13" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/5E14BD13-50D3-4984-BC6D-70F300590254.jpeg" alt="Photo 14" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/798424E4-A96A-42EC-ACA0-D3BCB7FC5AED.jpeg" alt="Photo 15" onclick="openModal(this.src)">
</div>
<div class="photo-grid">
  <img src="/assets/2025-04-20/7F12D8A5-97C4-41A1-A3CC-8175FC42B345.jpeg" alt="Photo 16" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/44E3EE24-FA79-40FA-B115-A0D52642872D.jpeg" alt="Photo 17" onclick="openModal(this.src)">
  <img src="/assets/2025-04-20/70CBF31B-0A72-48DD-B1D8-F0EB0D017EA1.jpeg" alt="Photo 18" onclick="openModal(this.src)">
</div>

<div id="imageModal" class="modal" onclick="closeModal()">
  <span class="close">&times;</span>
  <img class="modal-content" id="modalImage">
</div>

<style>
.photo-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
.photo-grid img {
  width: 100%;
  height: auto;
  margin-left: unset;
  margin-right: unset;
}
.modal {
  display: none;
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgba(0, 0, 0, 0.9);
}
.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}
.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #fff;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
}
</style>

<script>
function openModal(src) {
  const modal = document.getElementById("imageModal");
  const modalImage = document.getElementById("modalImage");
  modal.style.display = "block";
  modalImage.src = src;
}

function closeModal() {
  const modal = document.getElementById("imageModal");
  modal.style.display = "none";
}
</script>
