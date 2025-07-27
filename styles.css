window.addEventListener("load", () => {
  if (!window.LemonSqueezy) {
    alert("Erro ao carregar Lemon Squeezy, tente atualizar a página.");
    return;
  }

  window.LemonSqueezy.Setup({
    eventCallback: (event) => {
      if (event.event === "Checkout.Success") {
        console.log("Compra concluída com sucesso");
      }
    },
  });

  window.openCheckout = function (variantId) {
    if (!variantId) {
      console.error("VariantId inválido para checkout");
      return;
    }
    window.LemonSqueezy.Checkout.open({ variant: variantId });
  };
});

function showSection(id) {
  document.querySelectorAll("section").forEach((section) => {
    section.style.display = "none";
    section.classList.remove("active");
  });
  document.getElementById(id).style.display = "block";
  document.getElementById(id).classList.add("active");
  window.scrollTo({ top: 0, behavior: "smooth" });
}

// Mostrar produtos por padrão
document.getElementById("products").style.display = "block";
document.getElementById("products").classList.add("active");
