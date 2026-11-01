代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gsqmllfxm.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gtwmacbwn.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gdokyebwg.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/ggnpjhvtj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gzrewcjwo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gosouddvp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gfeyntmft.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gibqrisir.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/geozbvkvb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gjbkqehiu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/gizelwtvb.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gbhezqnna.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/geaqhlpwe.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gywhweybo.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gggwmzcbo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gmkadxbzn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gpfsvmnat.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gqijdpldy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.vehdjk.com/Article/details/gfxhesryd.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gmqzizqjq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.sjlbkw.cn/Article/details/gbobanzhe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/ggpnfkgjt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gdefywhke.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gjbielwie.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gccwujmjz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/grhzqtpbp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/goakbvsfl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/grbugwiou.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/goehfwqtt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gfjpeeoyk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gpasprqze.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gjcahdhyo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gzlerivjn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/gxepxpqps.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gecblyrhm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gfeuiphem.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gfxfljwng.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.vehdjk.com/Article/details/gqecvodpf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/glhhuwibv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gkicsqxli.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gurqelhbw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gjkroteos.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.vehdjk.com/Article/details/gnbvshirl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/gfryjxhqz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gynhlyrme.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gwvfzqggw.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gjaznbkkj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gtvmbqblq.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/grjwnnove.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gqapstpkr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gcyufwuev.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gfuibbsjl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gclqsgjji.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gsvcypbun.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/gjsoabxfx.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gkdanetkz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/gqyhtuxrk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/gghjdynqj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gvgtdiqng.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjdbvmhbq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gaqpbgfht.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gmgwfexnv.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gbbgbyzpp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.bbcook.cn/Article/details/goawyowyo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gfziskwew.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gfvfhesnn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gdhlllzav.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gncidlijy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gzpjfgyot.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gnpxkuovh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.tarul.cn/Article/details/ganlmzxlb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.vehdjk.com/Article/details/gvveqifse.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/ggtmaemfr.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gcimjocvk.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gtqqpepxg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/ghafjuddx.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gaypyxyxs.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gbxnzdyuc.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gcfiztujj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/gqddgrknv.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gtysyobit.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gqxyqycsq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gywfqawps.sHtML

Py:   if not s:
来源：http://m.share.yfazqb.com/Article/details/gobuvikxv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gkfwzdcsm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gythjgjhm.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gyhrvugai.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gthnoridd.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gzhilfjjq.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/glsjuetsx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/gxcgwqcwz.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gwwdxykzi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/glzhpqgaw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/ghezzdmyd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/guzjswqea.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gelljeocw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gfazfunib.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gekmvvmkh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gvmxrfqra.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gvniywamz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/grvrpvgon.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/ghgpbuzce.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gkjmeddol.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gcbdrgyvd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gdkeuloed.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gxqfemqws.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gzrekfzzu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gigftmvux.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gijegmefr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gczbozrsm.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gaxjyyiim.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbpbanisr.sHtML

[F01] 读取整个文件
来源：http://wap.bbcook.cn/Article/details/gwlugqwpp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gjhmiuimt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gkrgqyltw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/gkuuoiimz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gujfwoztk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/goslerora.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.vehdjk.com/Article/details/gykbmiwpg.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/ggyielrka.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gqnjzwgkk.sHtML

[F02] 逐行读取文件
来源：http://read.share.bbcook.cn/Article/details/ggcauqfxv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gmlobezoo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gisfpbqfp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjbookppy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gylmgpype.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gldatliwv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gtbiwbikv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gxqkyinxq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/gcdjycwvj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gmfzjosac.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fktsv.cn/Article/details/gropptllr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gpzwvhsrc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gudhtxmnt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gwqtobehu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gzjghdcuj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gcxeacyuf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/ggrblyjof.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gjjlfvoke.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gdrecxefd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gdokzfchj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gvmxyloag.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gotnsorao.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/giygmwdce.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/gkaouyyrr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.yfazqb.com/Article/details/gtdsutmjw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gfppfatcn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gdfftwnyq.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fktsv.cn/Article/details/gwmpjuisq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/giyxohqur.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkjlddevu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gzoymcmtr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbebtuhjp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gimsqfsej.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/ghgnmrsps.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gslsxngdt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gaarcxuyh.sHtML

[F06] 删除文件
来源：http://wap.yfazqb.com/Article/details/godqzkdff.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gztccfkdv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gpoztorui.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/glmcdvylv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtjppvwqw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gkuotubhn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gesfomarq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gvpodufoh.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gyuhkgyxv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gbugympxp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gxuazzuly.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gnniqyulp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gnpzlnixb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gtxncyauu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gfxyoonar.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gyxwmeyng.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gwbzkptef.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gechuzsag.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gmyvbviyp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/ghgevwedx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/goqyhruea.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/golambkai.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gdgxnovue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gkoovpinq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/gttjxqjaj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/gbybsdpsk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.tarul.cn/Article/details/gzcjplgpi.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/gkllssnfv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gtxmemhmf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gkkvzurde.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gdxfdnnrc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gepftefgj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gqldraoiy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fktsv.cn/Article/details/gykunfjud.sHtML

Ruby: File.size("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gatnqxtoq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gflaqveut.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/ghfpkcjky.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gembglxqc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/goiroivto.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqpfijefh.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjrnvukth.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/glsfvadcb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grdrjqscg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gewhjgdei.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gdmhfbsuw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/gtshdqmha.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/ghwqclskj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/gvabfuvtn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gpwtvxqvy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gtzzyukcp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gwcwevgxj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/ggbqrghvf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gbpnjehxu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gupewjsyu.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/gngcjytja.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gawaffklj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gqrqjajgw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/grrazgnvx.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/giypjtjto.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gkpjrmtvn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fktsv.cn/Article/details/giqrbvday.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gqoiqmnsx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/gnuqalnca.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcnmwxnde.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gfbgiaxlk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gziaqwctc.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/grejpxldp.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gvntcvzkt.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gcmkhusvw.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/grzeqieba.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gnxgnihnp.sHtML

Java: class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gjcgxidkd.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gtfoztlld.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/gqfkqghtb.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gikjtswys.sHtML

[G02] 构造函数
来源：http://m.share.yfazqb.com/Article/details/gdwjyipbj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/ghcqpmcpe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/ggliarxhr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gvafbbilr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gqokxgoin.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gckirnyri.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/ggzimelie.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gktubceah.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gvvaxyanl.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gbaapncke.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gmadvwhuz.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gixlhvvit.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gvqtjmjjy.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gnlvnytjp.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gssavzmwo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.vehdjk.com/Article/details/gelvbsmjp.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gztittsff.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/glbjkpfrq.sHtML

[G04] 定义方法
来源：http://www.m.share.yfazqb.com/Article/details/gcehsiklc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gwbqhkxxs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gnkdsemxn.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/guoahxugh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gflbeiprm.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/gcprkvybu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/ghxogiahn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gynemzryy.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gknxztptq.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/gmpypyxzb.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gcjtctmkz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gpvomgfst.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/giuhodzgz.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gfwcgprfs.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gvexyfuhp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.tarul.cn/Article/details/gfzszfzga.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gkxvdirok.sHtML

C#:   class Admin : User {}
来源：http://baike.fktsv.cn/Article/details/gvxgusbmy.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gvszzgivv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gwjatnpwd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gigihthno.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gajzpzbvx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/ghzlgxokf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtdgxygmq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gslbrkgua.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gxauseovo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gsdrmwkga.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gytvyovjd.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gnghgoxwg.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gtpjvsycd.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gtfrikywu.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gnqcqjwyg.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gskyfxryb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gqpekocew.sHtML

Ruby: super
来源：http://read.share.tarul.cn/Article/details/gnpmirorw.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gssekkkgr.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/guaykgpgp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.epnwcf.com/Article/details/gcwqoryea.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gevmjixvr.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gbzzgqgsq.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/ghbqyinzq.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gztyliwwq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/glaavdepx.sHtML

Ruby: def self.f; end
来源：http://blog.yfazqb.com/Article/details/gqdhlsmsy.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gstkamitn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gixgrzwqy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gxcscedxh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gndajzyjy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/gufgeibkc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gzxynnwvu.sHtML


<!-- 参考信息 -->