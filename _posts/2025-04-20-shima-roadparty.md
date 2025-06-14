---
title: "志摩ロードパーティ ハーフマラソン2025"
published: true
---

<p>2025年4月20日（日）に開催された「<a href="https://shima.roadparty.jp/index.html" target="_blank">志摩ロードパーティ ハーフマラソン 2025</a>」にて、霧雨魔理沙のコスプレで 10km 完走しました。</p>

<div id="photoGrids"></div>

<div id="imageModal" class="modal" onclick="closeModal(event)">
  <span class="close" onclick="closeModal(event)">&times;</span>
  <span class="modal-prev" onclick="showPrev(event)">&#10094;</span>
  <img class="modal-content" id="modalImage">
  <span class="modal-next" onclick="showNext(event)">&#10095;</span>
</div>

<style>
.photo-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 0px;
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

@media (max-width: 767px) {
  .photo-grid {
    margin-left: calc(((100vw - 100%) / 2) * -1);
    margin-right: calc(((100vw - 100%) / 2) * -1);
  }

  .modal {
    width: auto;
  }

  .modal img {
    margin-left: unset;
    margin-right: unset;
  }
}

.photo-grid img {
  width: 100%;
  height: auto;
  margin-left: unset;
  margin-right: unset;
}

.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

.modal-content img {
  width: 100%;
  height: auto;
  margin-left: unset;
  margin-right: unset;
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
.modal-prev, .modal-next {
  position: absolute;
  top: 50%;
  color: #fff;
  font-size: 48px;
  font-weight: bold;
  cursor: pointer;
  user-select: none;
  padding: 16px;
  background: rgba(0,0,0,0.3);
  border-radius: 50%;
  transform: translateY(-50%);
  z-index: 2;
}
.modal-prev {
  left: 30px;
}
.modal-next {
  right: 30px;
}
</style>

<script>
const imagePaths = [
  "/assets/2025-04-20/D4D0574E-4958-44A4-806F-8939E9BF9030.jpeg",
  "/assets/2025-04-20/DB103E60-8778-4FB9-B8CD-A3384125F754.jpeg",
  "/assets/2025-04-20/186407F2-5BDA-49FC-8AF0-2E5AB3D88154.jpeg",
  "/assets/2025-04-20/D244C895-67D5-4700-86ED-1ED2A072EAB5.jpeg",
  "/assets/2025-04-20/5091B24E-D78E-4E04-87C4-DE1D1C7E62C0.jpeg",
  "/assets/2025-04-20/5CFA83BF-A4EB-4199-8E46-AC437C80A45E.jpeg",
  "/assets/2025-04-20/BD9AB53E-BAD0-4669-A2AC-F044A0C18DBE.jpeg",
  "/assets/2025-04-20/E3079483-47EF-4FEE-9751-C54A36E3CA21.jpeg",
  "/assets/2025-04-20/6C3AA074-37DB-485E-AB6F-B278AEE321B8.jpeg",
  "/assets/2025-04-20/8937AAE3-44E6-4CBC-A6C6-F47E077AF2AA.jpeg",
  "/assets/2025-04-20/EB0A5E1B-AFEC-4CFA-835E-A26A838DB4A1.jpeg",
  "/assets/2025-04-20/7B37F259-9F08-4F12-A079-2B62B48A957E.jpeg",
  "/assets/2025-04-20/7143F58D-0E45-402A-8729-CEE016D42AB5.jpeg",
  "/assets/2025-04-20/5E14BD13-50D3-4984-BC6D-70F300590254.jpeg",
  "/assets/2025-04-20/798424E4-A96A-42EC-ACA0-D3BCB7FC5AED.jpeg",
  "/assets/2025-04-20/7F12D8A5-97C4-41A1-A3CC-8175FC42B345.jpeg",
  "/assets/2025-04-20/44E3EE24-FA79-40FA-B115-A0D52642872D.jpeg",
  "/assets/2025-04-20/70CBF31B-0A72-48DD-B1D8-F0EB0D017EA1.jpeg"
];
let currentIndex = 0;

// 画像グリッドを自動生成
function renderPhotoGrids() {
  const container = document.getElementById('photoGrids');
  let html = '';
  for (let i = 0; i < imagePaths.length; i += 3) {
    html += '<div class="photo-grid">';
    for (let j = i; j < i + 3 && j < imagePaths.length; j++) {
      html += `<img src="${imagePaths[j]}" alt="Photo ${j+1}" data-idx="${j}">`;
    }
    html += '</div>';
  }
  container.innerHTML = html;
  // 画像クリックイベントを設定
  container.querySelectorAll('img').forEach((img, idx) => {
    img.onclick = function() { openModal(imagePaths[idx]); };
  });
}

function openModal(src) {
  currentIndex = imagePaths.indexOf(src);
  if (currentIndex === -1) currentIndex = 0;
  const modal = document.getElementById("imageModal");
  const modalImage = document.getElementById("modalImage");
  modal.style.display = "block";
  modalImage.src = imagePaths[currentIndex];
}

function closeModal(event) {
  if (!event || event.target.classList.contains('modal') || event.target.classList.contains('close')) {
    document.getElementById("imageModal").style.display = "none";
  }
}

function showPrev(event) {
  event.stopPropagation();
  currentIndex = (currentIndex - 1 + imagePaths.length) % imagePaths.length;
  document.getElementById("modalImage").src = imagePaths[currentIndex];
}

function showNext(event) {
  event.stopPropagation();
  currentIndex = (currentIndex + 1) % imagePaths.length;
  document.getElementById("modalImage").src = imagePaths[currentIndex];
}

document.addEventListener("DOMContentLoaded", renderPhotoGrids);
</script>
