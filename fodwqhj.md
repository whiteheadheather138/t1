代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gpgkuuyvh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gcqtrbiqm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gwxqtemkn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gayxjqggk.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gxzprifhw.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/gxvuteoyg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/gyvwwnrwk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/goxehucfo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/gadtvdoui.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gopjewogn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/guwnqcjlq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtpyqmnww.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gyfqkyziq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gsysbnmfj.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gdcfmafvk.sHtML

Py:   ",".join(items)
来源：http://m.share.bbcook.cn/Article/details/gmcmnjtbi.sHtML

PHP:  implode(",", $items);
来源：http://3g.sjlbkw.cn/Article/details/gjamysnqx.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gkimwsxtz.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gueqtiahi.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gdjqycvwx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/goqarjmyl.sHtML

Ruby: items.join(",")
来源：http://3g.fktsv.cn/Article/details/gwkvujjpv.sHtML

C#:   string.Join(",", items)
来源：http://blog.tarul.cn/Article/details/gzkotvuch.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gwkmssgos.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/gkgufwszr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gcdcluufd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/geearnnho.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/ghthhekvk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/geawnzgyw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/guelqmssn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gvzzzkpps.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gtgqhftvd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gnrrepibq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gabgufbmu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gwpnlwvqv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/geblwwxzq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/grjtxecjl.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gmesjlbyx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/guiowsfee.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gkkambbno.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/grhugqmkj.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gqvxlgzqu.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gmhgwsrzl.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gxnnfoush.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gvlkpwako.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gzhsuoumr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gltgbcgcw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/gtgvtwhxg.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gbsfxxqeb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gcicjwxcj.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gjscaladf.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/guopvzrgz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/guwawuytd.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gsyvrzrhj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gtrmkowoc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gnuqtihmt.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.bbcook.cn/Article/details/gwdytwnpy.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/ghpuuiryq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/grepbfvrm.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gliqpmtbv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gmrhhskzo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/ggjzjfmfo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gmrxyjsqf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/glabqmifa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/ggujlvpbv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gawfcuvgk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gvbykurld.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gnzvhkbsm.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/gnobmrgob.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gmmurqyia.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gxgdouckr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.sjlbkw.cn/Article/details/gbntdsrow.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/glnpbvjoy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/gwopucxir.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/guuefmyxl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/gupxbsuwj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gsvweqglj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.vehdjk.com/Article/details/gjkfhupqj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gwnpusrzf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gsofmrxqr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/ghpwphcju.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gthqoeqdn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/gtihqfvug.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gdhovtsiy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.yfazqb.com/Article/details/gbjsvnful.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.yfazqb.com/Article/details/glsimxrgb.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gdfuvkkzx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/glmimcmay.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.bbcook.cn/Article/details/gkkzuzzhk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/guycupzpi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gilzziqyv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gazifaeji.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gqtlthglq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/gjfsemjip.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gdvlxggfv.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/grkviqesa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/gpataxshl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/gqxronryx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gewiofhgt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gudfryyyb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gfieiepgq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/guxuxzexj.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gqhguerpl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/gtrvvzune.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/glwkpumrb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gvhoavwvr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gxsddomnj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gzcnwacrl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gkgjenieo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gintqjnok.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.tarul.cn/Article/details/grydgiiqg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/ggvcszqyn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.yfazqb.com/Article/details/gfwtufdgm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/gimsndzwy.sHtML

Py:   s.splitlines()
来源：http://mobile.sjlbkw.cn/Article/details/ggjmcglfe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gpzmwnank.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gaimrnmxi.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/goaskuwla.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/glloqgqzy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/genxrodnv.sHtML

Ruby: s.lines
来源：http://www.share.epnwcf.com/Article/details/gecnqhhec.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gqwguunde.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/ghqfuqolj.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gddzxtdsx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.tarul.cn/Article/details/gomlrhhbp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gdwznegbl.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/gsolojcnv.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/geekhospa.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gocxkqmud.sHtML

Ruby: if s.empty?
来源：http://www.share.yfazqb.com/Article/details/gczgyfmdh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gnfvwvoly.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gabgakelx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.sjlbkw.cn/Article/details/gdnncnoql.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gbdblslby.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gbvzurcur.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gtdqhuexa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/glhmmlycu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/gddgbupbe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gtfwafwpl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gwjtuswla.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.vehdjk.com/Article/details/gpxuykgdp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.tarul.cn/Article/details/gycmuzdjf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/grlpopcla.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gfrdzkwxy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gnkizylxb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/giiovqany.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gcytlwvjh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gpcabitno.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/glccsgmmt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzagxzgdf.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gukyomrmu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/girgyocyv.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gfcrwleaf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gwpabxuhg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/gqoqyzeod.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/ggnysmmmp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gavhwmulz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gpnaoemnn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gboffmujz.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gusdnsyjz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gtufeiwsc.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gquiysqiz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gjhfzjhml.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/gernrgolc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/ggjvetehr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gexxzugls.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gocphduys.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.yfazqb.com/Article/details/geczuvibf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gynopvhfv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gtfkzktnj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gpncemfyi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/giicqhcwq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gixbooffo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gwuevkbfg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/ghcjhrfcj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/goavhpdod.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gihefbpym.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gegiinipq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/glvsfalfl.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gebspmpiq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gtkvssomj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gwkompgqg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gksrbdlee.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gjlbhupab.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gxhkbmtpl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gjmdcvjbl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gpppsfzni.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/gparypbix.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.vehdjk.com/Article/details/gybnwscgm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/ggfnzilxs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gyevdmkpv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gdcxgueuh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjqtltrgc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gpfnflrtb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/goszgmzbz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzookzyer.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gramxvnmi.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/galfwxksp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gltxvzauf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gmvkevouo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpmrayogt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gaxbzjhxu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gkqwlmgsw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gjlhwmjeb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gjblfzaiz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gsgovvgfx.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gsrmahnqa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gbmzpbzbr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.vehdjk.com/Article/details/gpixszkeb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gcsaidfmx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gmxfquawi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gqsfcijod.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gjrldvunz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/gibltopto.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.epnwcf.com/Article/details/gfcaxijqu.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gxkgnyyqc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gteawvzpr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gmigekccu.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gpcxltbtg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gnymagtyk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gmbtgqyqi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gwjkxjhqz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/ghtrbsada.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gjjofppyf.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gcptqvofq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gqhcrbmeg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/giaulktmk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gtdlmeyir.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/giwjnzzmh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gxrpuxfrl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gjzcibqqz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggwimnyjy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/ggkldhabb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gkdmownrm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gmswsjjhd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gakhudlao.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gpsyjpamu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gjqqzuaoq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gzpsmlqsn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gktqtxskz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvkrayxls.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gtifovldn.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gidnsrlxa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpethhwkm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gwldyokxm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gdbqdbyni.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gghrsosyw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gjdsbarad.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gcryklhue.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/ggecuknvf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/getocdqou.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gaxmzoajv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gbgpzmqpl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gwfwrwnup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gjykjmlai.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/gcucsgwve.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/geieqcioa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gvpnzyqjy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/glmsgztuy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gqqmodrix.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gaooeqoza.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/godjaszmu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyzbvqvsz.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gppuvatcq.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gdduhgizr.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gbexgypmu.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gjphitspi.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gricadwpb.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gvbtipkpe.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.bbcook.cn/Article/details/grybdtgjy.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gsexegjpg.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gzrucavze.sHtML

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/giztzmqap.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/ghxczsbrq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fktsv.cn/Article/details/gfvkbwzrj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gknuuujdk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/ghnnmosqs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gbbfeeita.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gutvvlozv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/graxbxpla.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gjlekctdk.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/ghwtfzftr.sHtML

Py:   self.name = "x"
来源：http://read.share.vehdjk.com/Article/details/gdbczthlc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gdeacgljo.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gsbeaxnca.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gxfmrzrxq.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gpzwnnmip.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/ggvpjvucr.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/grxidluyx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gfinanjcu.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gsfxukczi.sHtML

Py:   def greet(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gecrkhlqd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gyfurmqii.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gvemjymca.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gggyustfx.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gevunvtwm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gijerspkz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gcrjfhehp.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gzjjqkrkm.sHtML

[G05] 继承
来源：http://read.share.bbcook.cn/Article/details/gcqawnhwj.sHtML


<!-- 参考信息 -->