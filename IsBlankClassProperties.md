```
        public static string IsAnyClassPrpertiesEmpty(object classObject)
        {
            string message = string.Empty;
            PropertyInfo[] properties = classObject.GetType().GetProperties();
            foreach (var p in properties)
            {
                if (string.IsNullOrEmpty(p.GetValue(classObject).ToString()))
                {
                    message += p.Name + "/n";
                }
            }
            return message;
        }


```
