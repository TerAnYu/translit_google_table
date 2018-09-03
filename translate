    /**
     * Возвращает входную строку, в которой все вхождения из search
     * заменены на строки из replase
     *
     * @param array search Строки поиска
     * @param array replase Строки замены
     * @param string subject Входная строка
     * @returns string
     */

function str_replase(search, replase, subject) {
        var string = subject;

        for (var i = 0; i < search.length; i++) {
            var pos = 0;

            while ( -1 != (currPos = string.indexOf(search[i], pos) ) ) {
                string = string.slice(pos, currPos) + replase[i] + string.slice((currPos + search[i].length));
            }
        }

        return string;
    }

function Translit (subject) {
          /**
         * Транслитерация строки.
         *
         * @param string subject Входная строка
         * @returns string
         */
            var string = subject;
            var replace = {
                  "А": "A", "а": "a", 
                  "Б": "B", "б": "b", 
                  "В": "V", "в": "v", 
                  "Г": "G", "г": "g", 
                  "Д": "D", "д": "d",
                  "Е": "E", "е": "e", 
                  "Ё": "E", "ё": "e", 
                  "Ж": "Zh", "ж": "zh", 
                  "З": "Z", "з": "z", 
                  "И": "I", "и": "i",
                  "Й": "Y", "й": "y", 
                  "К": "K", "к": "k", 
                  "Л": "L", "л": "l", 
                  "М": "M", "м": "m", 
                  "Н": "N", "н": "n", 
                  "О": "O", "о": "o",
                  "П": "P", "п": "p", 
                  "Р": "R", "р": "r", 
                  "С": "S", "с": "s", 
                  "Т": "T", "т": "t", 
                  "У": "U", "у": "u", 
                  "Ф": "F", "ф": "f",
                  "Х": "Kh", "х": "kh", 
                  "Ц": "Ts", "ц": "ts", 
                  "Ч": "Ch", "ч": "ch", 
                  "Ш": "Sh", "ш": "sh", 
                  "Щ": "Shch", "щ": "shch",
                  "ъ": "", 
                  "Ы": "Y", "ы": "y", 
                  "ь": "",
                  "Э": "E", "э": "e", 
                  "Ю": "Yu", "ю": "yu", 
                  "Я": "Ya", "я": "ya"
                };
            for (var key in replace) {
                if (replace.hasOwnProperty(key)) {
                    string = str_replase([key], [replace[key]], string);
                }
            }

            return string;
        }
