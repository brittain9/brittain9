<!-- Heading -->
<h3 align="center">Hello! I'm Alex. Welcome to my Github</h3>
<h3 align="center"><a href="https://twitter.com/acb935">Twitter</a>
<h3 align="center"><img src = https://github.com/brittain9/brittain9/blob/main/computer.gif width=75px></h3>

---

    namespace Welcome
    {
        public class Alex
        {
            #region Properties

            public string m_UserName;
            public string m_Name;
            public int m_Age;
            public string m_School;
            public string m_Major;
            public string[]? m_Interests;

            #endregion

            public Alex()
            {
                m_UserName = "brittain9";
                m_Name = "Alexander Brittain";
                m_Age = 21;
                m_School = "University of Texas at Austin";
                m_Major = "Management Information Systems";
                m_Interests ??= (new string[] { "CSharp", ".NET", "Computer Science", "Foodie" });
            }

            public override string ToString()
            {
                string ret = $"Hello! My name is {m_Name}. I am a {m_Age} year old {m_Major} major at {m_School}.\n";
                if (m_Interests != null)
                {
                    ret += "\nMy interests include:\n";
                    foreach (var interest in m_Interests)
                    {
                        ret += $" - {interest}\n";
                    }
                }
                ret += "\nCheck out my website and feel free to contact me by email or Twitter.";
                return ret;
            }

            public static void Main()
            {
                Alex a = new Alex();
                Console.WriteLine(a);
            }
        }
    }
