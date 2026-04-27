## Objetivo
Reemplazar el QR del PDF para que apunte a tu p�gina `verificacion.html` con los mismos par�metros que usa Equifax.

## 1) URL final para el QR
La URL debe tener este formato (igual de �larga� que el ejemplo):

- `https://<TU-DOMINIO>/<RUTA>/verificacion.html?country=CL&document=0171051754&verificationCode=a77b616f-307a-462b-5244-6e231a8cf569`

Notas:
- Si abres `verificacion.html` en el navegador, en la consola ver�s un log `QR URL: ...` con la URL ya armada usando defaults.
- Puedes cambiar `document` y/o `country` en la URL si lo necesitas; el front los precarga.

## 2) Generar el QR
Opciones:
- Generador online (r�pido): pega la URL final y descarga el QR como PNG (idealmente 512x512 o 1024x1024).
- Generador local (si prefieres offline): cualquier app que genere QR desde texto sirve.

## 3) Reemplazar el QR en Canva y exportar el PDF
Como tu PDF fue generado por Canva, lo m�s r�pido es:
- Abrir el dise�o original en Canva.
- Reemplazar la imagen del QR por el nuevo PNG.
- Exportar de nuevo a PDF.

## 4) Checklist de validaci�n
- Escanear el QR del PDF exportado.
- Debe abrir `verificacion.html?...verificationCode=a77b616f-307a-462b-5244-6e231a8cf569`.
- El input **�N� de Certificado�** debe venir precargado con `a77b616f-307a-462b-5244-6e231a8cf569`.
- Marcar �No soy un robot� (simulado) y presionar **Consultar**.
- Debe descargar `informe-dicom-platinum-360.pdf` (mismo archivo que el informe DICOM Platinum 360).

