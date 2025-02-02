---
title: <dialog>
slug: Web/HTML/Element/dialog
translation_of: Web/HTML/Element/dialog
original_slug: Web/HTML/Elemento/dialog
---

{{HTMLSidebar}}

El **elemento** **HTML `<dialog>`** representa una caja de diálogo u otro componente interactivo, como inspector o ventana.

<table class="properties">
  <tbody>
    <tr>
      <th scope="row">
        <a href="/en-US/docs/Web/HTML/Content_categories">Content categories</a>
      </th>
      <td>
        <a href="/en-US/docs/Web/HTML/Content_categories#Flow_content"
          >Flow content</a
        >,
        <a
          href="/en-US/docs/Web/HTML/Sections_and_Outlines_of_an_HTML5_document#Sectioning_roots"
          >sectioning root</a
        >
      </td>
    </tr>
    <tr>
      <th scope="row">Permitted content</th>
      <td>
        <a href="/en-US/docs/Web/HTML/Content_categories#Flow_content"
          >Flow content</a
        >
      </td>
    </tr>
    <tr>
      <th scope="row">Tag omission</th>
      <td>{{no_tag_omission}}</td>
    </tr>
    <tr>
      <th scope="row">Permitted parent elements</th>
      <td>
        Any element that accepts
        <a href="/en-US/docs/Web/HTML/Content_categories#Flow_content"
          >flow content</a
        >
      </td>
    </tr>
    <tr>
      <th scope="row">DOM interface</th>
      <td>{{domxref("HTMLDialogElement")}}</td>
    </tr>
  </tbody>
</table>

## Atributos

Este elemento incluye los [atributos globales](/es/docs/Web/HTML/Global_attributes). El atributo `tabindex` no debe utilizarse en el elemento `<dialog>`.

- {{htmlattrdef("open")}}
  - : Indica que el diálogo está activo y disponible para interactuar. Cuando el atributo open no está asignado, no debe mostrarse al usuario.

## Notas de uso

- Los elementos `<form>` pueden integrarse dentro de un diálogo especificándolos con el atributo `method="dialog"`. Cuando se envía un formulario, el diálogo se cierra con un atributo {{domxref("HTMLDialogElement.returnValue", "returnValue")}} asignado con el `value` del botón utilizado.
- El pseudo-elemento {{cssxref('::backdrop')}} de CSS puede utilizarse para dar estilos al elemento `<dialog>`, por ejemplo para atenuar contenido inaccesible mientras el diálogo modal esté activo.

## Ejemplos

### Ejemplo 1

```html
<dialog open>
  <p>Greetings, one and all!</p>
</dialog>
```

### Ejemplo 2

```html
<!-- Simple pop-up dialog box, containing a form -->
<dialog id="favDialog">
  <form method="dialog">
    <section>
      <p><label for="favAnimal">Favorite animal:</label>
      <select id="favAnimal">
        <option></option>
        <option>Brine shrimp</option>
        <option>Red panda</option>
        <option>Spider monkey</option>
      </select></p>
    </section>
    <menu>
      <button id="cancel" type="reset">Cancel</button>
      <button type="submit">Confirm</button>
    </menu>
  </form>
</dialog>

<menu>
  <button id="updateDetails">Update details</button>
</menu>

<script>
  (function() {
    var updateButton = document.getElementById('updateDetails');
    var cancelButton = document.getElementById('cancel');
    var favDialog = document.getElementById('favDialog');

    // Update button opens a modal dialog
    updateButton.addEventListener('click', function() {
      favDialog.showModal();
    });

    // Form cancel button closes the dialog box
    cancelButton.addEventListener('click', function() {
      favDialog.close();
    });

  })();
</script>
```

## Especificaciones

| Especificación                                                                                           | Estado                           | Comentario         |
| -------------------------------------------------------------------------------------------------------- | -------------------------------- | ------------------ |
| {{SpecName('HTML WHATWG', 'forms.html#the-dialog-element', '&lt;dialog&gt;')}} | {{Spec2('HTML WHATWG')}} |                    |
| {{SpecName('HTML5.1', 'semantics.html#the-dialog-element', '&lt;dialog&gt;')}} | {{Spec2('HTML5.1')}}     | Definición inicial |

## Compatibilidad de navegadores

The compatibility table in this page is generated from structured data. If you'd like to contribute to the data, please check out <https://github.com/mdn/browser-compat-data> and send us a pull request.

{{Compat("html.elements.dialog")}}

## Ver también

- [Formularios HTML](/es/docs/Web/Guide/HTML/Forms).
- El evento {{event("close")}}
- El evento {{event("cancel")}}
- El pseudo-elemento {{cssxref("::backdrop")}}
