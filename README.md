# Red_Social_properties
Creación de código para una red social. Opción de realizar un nuevo post, teniendo en cuenta un constructor y una propiedad llamada "Text".
Estás creando una aplicación de red social y quieres añadir funcionalidad para crear publicaciones.

Cuando un usuario crea una publicación, el texto "New post" debe ser mostrado automáticamente para que luego el usuario pueda añadir el texto que desea compartir.

El programa que se te ha dado declara una clase Post con un campo privado text , y el método ShowPost() que muestra el contenido.

Completa la clase con

- un constructor, que muestre "New post" cuando se llame,

- propiedad Text , que te permitirá obtener y establecer el valor del campo text.

Una vez que hayas realizado los cambios en el programa para que funcione correctamente, entonces en main, el programa tomará el texto de la publicación del usuario, creará un objeto de publicación, asignará el valor tomado al campo de texto y lo mostrará.



class Program
    {
        static void Main(string[] args)
        {
            string postText = Console.ReadLine();

            Post post = new Post();
            post.Text = postText;
            post.ShowPost();

        }
    }

    class Post
    {
        private string text;
        
        //write a constructor here
        public Post()
        {
            Console.WriteLine("New Post");
        }

        public void ShowPost()
        {
            Console.WriteLine(text);
        }
        
        //write a property for member text
        public string Text
        {
            get {return text; }
            set {text = value; }
        }
    }
