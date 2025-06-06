Esta es una libreria para usarla en CPP entorno windows aplicacion de escritorio.
Opción 1: Usar el control en tu proyecto C++ (Win32)
1.	Incluye el header y la DLL:
•	Añade TextShadow.h a tu proyecto.
•	Copia la DLL compilada al directorio de tu ejecutable.

3.	Vincula el archivo .lib:
•	En Propiedades del proyecto > Vinculador > Entrada > Dependencias adicionales, añade el .lib generado por la compilación de la DLL.

5.	Crea el control en tu código:
•	Instancia y usa el control como lo harías normalmente en C++:
 ```cpp
     TextControl* g_textControl = new TextControl();
     g_textControl->Create(hWndParent, x, y, width, height, id, hInstance);
 ```
Llamadas al control...

g_textControl->SetText(L"Texto sombreado de ejemplo");//Texto
g_textControl->SetFontSize(32);/Tamaño Fuente
g_textControl->SetFontName(L"Consolas"); // Cambia el tipo de fuente aquí
g_textControl->SetTextColorValue(RGB(0, 0, 255));//Color Texto
g_textControl->SetShadowColor(RGB(128, 128, 128));//Color Sombra
g_textControl->SetOutlineColor(RGB(255, 255, 255));//Color Borde del Texto
g_textControl->SetOutlineWidth(3);Tamaño del Borde

---------------------------------------------------------------------------
weblackbug@gmail.com
sergi@canalinformatika.es
Programado en C++
entorno WINDOWS ESCRITORIO
