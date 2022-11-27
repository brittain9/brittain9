
<h3 align="center">
<div>
Hello! I'm Alex
</div>
    
<h3 align="left">
    
<!-- <a href="https://twitter.com/acb935">Twitter</a> -->


<p>
📧
<a href = "mailto: alexbrittain9@gmail.com">Email</a>
&nbsp
&nbsp
&nbsp
🤝
<a href = "https://www.linkedin.com/in/alexander-brittain-b07369206">LinkedIn</a>
</p>

</h3>

---

    namespace Welcome
    {
        sealed class Alex
        {
            public string UserName;
            public string Name;
            public int Age;
            public string School;
            public string Major;
            public string[]? Interests;

            public Alex()
            {
                UserName = "brittain9";
                Name = "Alexander Brittain";
                Age = 21;
                School = "University of Texas at Austin";
                Major = "Management Information Systems";
                Interests ??= (new string[]
                    { "C#", "Electricity", "Building things myself", "Sushi", "Elegant code", "Construction" });
            }

            public override string ToString()
            {
                string str = $"Hello! My name is {Name}.\nI am a {Age} year old {Major} major at {School}.\n";
                if (Interests != null)
                {
                    str += "\nMy interests include:\n";
                    foreach (var interest in Interests)
                    {
                        str += $" - {interest}\n";
                    }
                }
                str += "\nCheck out my website and feel free to reach out on LinkedIn or my email.";
                return str;
            }

            public static void Main()
            {
                Alex a = new Alex();
                Console.WriteLine(a);
            }
        }
    }
    
<h3 align="center"><img src = https://github.com/brittain9/brittain9/blob/main/computer.gif width=250px></h3>
