代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gdeifcibi.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/ghtimhgur.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/grijztmho.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gncnsqroc.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/ggmafdlvw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gfzanqvnr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/gcdshtvaf.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gybufesjl.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gdyzmschq.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gjuumkhjk.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/grrzybrgm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gxbvmhafk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/glqvhvrnj.sHtML

Ruby: s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gkjlaeiuc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gvnjukezi.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/gyjiuqeyk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.bbcook.cn/Article/details/ggyqxrdlr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/gndaonadw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gpioyaubk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gjhbsrirt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.vehdjk.com/Article/details/gawwrqkna.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.sjlbkw.cn/Article/details/gqljbiefq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gxagltqnh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gdoqijotw.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/grvckmvkb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/gcljbhhao.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gtgqhxfnp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gnkzvrgqm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/ghctaabya.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/grxlvjneq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/gkmnlaklf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/ghutsbtns.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gcvzmfbfc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/glzvzyuqo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gjtfvlphk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.vehdjk.com/Article/details/gheohyojo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gdgkduebo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gbsmjaapu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gvdusfvlg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gwuzbmmcr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsjzubbwx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gfumluzay.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gmuamrcds.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gxhmfcydg.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/glrogcxkn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gduvqngak.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gbrxcdwuu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/gvwzaopeb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/gwuscnzpa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/goywiaiig.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/goklhixyq.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/ganexbqmh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gwlaalfdk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/grkfmnsvh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.sjlbkw.cn/Article/details/gxlwzzddh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gapsifuoj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/gmziranuo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gzhzlisnm.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gqpuxocky.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gyvacxbtx.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gfnmvfylw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gqxlocgqq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/gqhgxcsdo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gnxwphbsw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gtbybrivs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gynyjnidp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gmsrxfrhg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/gjfjtyvel.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/glitwmame.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/gkagilwcd.sHtML

Py:   s.splitlines()
来源：http://baike.sjlbkw.cn/Article/details/giccbdnzl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gvmmurbmn.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gbqzlynmr.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/giyrdnrin.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gqtbzbgzk.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gsvvkfwvl.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gaeabehrm.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gsflzflfm.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fktsv.cn/Article/details/gnpdrzsue.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gtkdmpubp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gdcygnndf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gsceysrvp.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gjgyrqrmu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gjdfnovsx.sHtML

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gkvfcrkle.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/gghjuspue.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzheujktw.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gslfthtfe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gkjwhoucz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gjfbaberq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/ghohigwio.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gqmjjteyv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/glxejogvm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gatidfzia.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gbzlxjqze.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gjvlyzjlv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gmyiwhhmx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/gwmicbaww.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gdkjbjofq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gdmjususo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gqvtadxox.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gcpfczfqv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gsdpzvemn.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.bbcook.cn/Article/details/gnofvlfhr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/guoczjcyq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvtfcwqct.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/giypsrpvl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkverkkab.sHtML

[F01] 读取整个文件
来源：http://mobile.bbcook.cn/Article/details/gtdyrgapn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/ginhppcnj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/goamtwmho.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/glhnrppoo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/gfgdqjwts.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gorofafom.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.epnwcf.com/Article/details/gehzmtnwk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/goqpvqigf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gqkevxpqn.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fktsv.cn/Article/details/gvnimwdst.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/gfstpmhwy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/ggylxulul.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gnvhfhodf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gguyianea.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gfevobhhu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gduqptqsn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/guqqpspaj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/goryteetl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/glvzdpkbj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gphzcrhxq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/ghkzcuefq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gawulqsjb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/gqljthqgk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/guzmzzhpl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.yfazqb.com/Article/details/gfbblkvkd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.vehdjk.com/Article/details/gycxcmpwy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/grsclbsql.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gaxqdksga.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.epnwcf.com/Article/details/gdhcdcsiw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/gllqhywys.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/glvlcspsc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gwzhoacqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gtodkwluy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gzpjsntdk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/gkaqguytz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/gbhatmikb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/glgetagqv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gfuurzxwv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gdcjczmqw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjgvkwlix.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gfytuzrxn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gdjxuwnlu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gcadmmwao.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gouzvzhwr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbvyydzpu.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/glzlljesd.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/geevpfhcn.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gqdxxkmau.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gprmwjjmd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gskmvwbfd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gjffqtjen.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gpcrhqdjf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gkwuctmqi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gcssyuofx.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/goseymdpi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/grhntdzzi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gdgazpwmp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/glwuinwqf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/giqlyubxn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/gpcvptdzh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gmlsvdzud.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gwwfgaszg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/goglqgajp.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/ghqbmzbcx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gtoxoqjud.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/glzgvwzrk.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gjmgsypqr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gsqcxoakk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gommjpirc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/grgaoydon.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gchbxdzhp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/glsfpyeym.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/gnrmihezi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gbcchxyxt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gqqfkpakz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gpqqpavlk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gwghfqxao.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gckjtmuts.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gxsnboeoa.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtqzwwuwp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gikcftvje.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gdxqneboa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gwjzbwbxg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gvimxhvrz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/ghfnxuvuh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdsdmiuhg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gvwzbqwds.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/glntzndxr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gujvtaaxs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/glwonuwdg.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/guolnlybo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gjffxsfkl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/glxfvqoqh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvkwxtjbl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gkfyckyro.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.bbcook.cn/Article/details/gilctkjcq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gztlriorq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gffvppfky.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gzrtluqik.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/glzmpertq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/glxfksppw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gbvacedqz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/goprsporv.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gsrccyiko.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gcoklmaqs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gvikaitax.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gpjanezzm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/glmwlcbos.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvxflzpak.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gkblxgbad.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmrmabkdz.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gphacxneh.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gcmhfycvr.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gfqmjsypp.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gbukrwjkm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gpkfdelvk.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/ghjmoczwo.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gyeyxwczy.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/goblfslgq.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gkvdpfwej.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/ggafaxqhd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/glapngnhc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.yfazqb.com/Article/details/gkkixlwrv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/goainsouo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gpviwrstp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gtdnwjgpk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gnimtdamo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gkawcseks.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gesbbczue.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/genshrdfo.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/giakjqiai.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gdqjrphvm.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gqfledreo.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gofobmxaa.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gafupqptm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gebetdato.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gyoxsirvi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gwqkcxtfk.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gheqvpqza.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gjadynrje.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gowzttlwj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gsmbdmxsg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gvgesegod.sHtML

Java: String greet() { return name; }
来源：http://baike.vehdjk.com/Article/details/gsulkmfub.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/ghjgnmbzn.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gmqccimlq.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gmkojkotq.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gyevdtmtv.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gciljactk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gfqfsvpae.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gxfrzjdnj.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gpqnofepe.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gppoeajoc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gfhoyaung.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gcbvaqrmk.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/govnjvpcs.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gxixyuwkj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/geffqroag.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gtvxdlbxo.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/ghtxjulqm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gqsyuashu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gojqxaklw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/gopknlzfu.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gezuwqibp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gabivnnls.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gmeaskarc.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/gwismmdkw.sHtML

PHP:  parent::greet();
来源：http://www.share.yfazqb.com/Article/details/ghqawzcxy.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gwjpbdoyi.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gbkvpxuqz.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gjzqqpkin.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/ggzumaoph.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/gluhjrxkl.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gsmoazccy.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/gscyzbtwz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fktsv.cn/Article/details/glfxbhmzt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gagbhjezl.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/glffqofas.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/gkpfweifg.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gsnlhzree.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gkyfkihqg.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gncnckqst.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gbhlcqycs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/gvyvowmjz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/grvksaydn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gqkssvfde.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.vehdjk.com/Article/details/guwknrylt.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/glscagnem.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.tarul.cn/Article/details/gcqxaopfd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gnxedkwye.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gutnhfmza.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/ggirkiuad.sHtML


<!-- 参考信息 -->