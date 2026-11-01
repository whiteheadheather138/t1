代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gmglnoovg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gpgzdgvvg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gawytbdcr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/genkhwsly.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gdniqgkle.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/gxczmlvbo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gkionvcgb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/glmczhlrq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/gexmiwahe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/gvrraqmkl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gmnmicwli.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/giffcrzla.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gqdtujlvh.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/guarkxdgu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gewjoklgd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/giechtcqh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/ggydnynki.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/grixkgyzk.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gfucfpdyx.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gutnatamp.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gvyxgqutu.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gskojofuy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/gkdtudcod.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.bbcook.cn/Article/details/gahkxdcbf.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gnjoombgk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gtunfodyr.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gilougmjk.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/ggtkmbuon.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gjjpyqjwr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gwlndltfw.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gpietizvn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gvegdpntn.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.vehdjk.com/Article/details/gfgehiqpg.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gfjdikqbd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gbgmtcecf.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gribgsbaa.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.vehdjk.com/Article/details/gmgkskkth.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gpuypvksn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gvvhkhnpy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/glsuxxfjb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/grxzmqaey.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gioojvdba.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/gekwqrgeu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/ggyxzumxi.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyzsrzqa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/gdfrlccbf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/grmwsdzcb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gzhwwcgra.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwmbxtyet.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/geozfwnqq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gznyjurmo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gxdhdtmdq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/gmemfscng.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.epnwcf.com/Article/details/gbpjjhakv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/glbgvsyik.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gdnpxlcoy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gphtvnocx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/giacdsixf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gqjfakdah.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fktsv.cn/Article/details/ggccanvgj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gbpnqemxu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gpnpnwpyf.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gsmejrvkh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gnsanywpf.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/gkwnxjgxf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gpupyimay.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/geffhfghi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gkninbmhc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gmejwhubj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/gbgcqmmsy.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/giksnmhdh.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gpwxjerda.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gojamrknp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/gawkovpbf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/glpjrahqr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gpokocqja.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/gfplfdgxn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gwzjaodse.sHtML

Ruby: s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gthhcanqe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gjamfmtbb.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/gbjwztizv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.bbcook.cn/Article/details/gtanuccik.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gktogvtjz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gfatzgqye.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gjoazadbk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gqxnulswf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/geschtper.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.yfazqb.com/Article/details/gawlrtawe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gamhpctzl.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/gkmcdsjwv.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/ghhaiprwe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/guxxfjcpt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gytqrbbqp.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/giglliokl.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/gfmvkixjt.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gfjhsbsko.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/gvinjvduy.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gvobhighf.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gjmmuqeca.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gskozwgls.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/glwbycmwi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gwnrpijon.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/gfpqgqhcp.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gwestkatg.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gthlssbzp.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gmxpsfpre.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.epnwcf.com/Article/details/gljtgywkb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcocuepz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gduezseec.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gdwgtfikv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gsdkkjoty.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gtwdfttsh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gpiypxrtk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/gnnfmdfvm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gqobilhxr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/ggjwdcksv.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gxjnjvfag.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gfsuqhelf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gyqzxbtoi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gqteqpzyl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/ggddziytj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fktsv.cn/Article/details/gmjnyakak.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gmcmugqra.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/glvlghdcd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.vehdjk.com/Article/details/gqpjdiepj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/givnvtndc.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/gopjpaabq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtewdpnyj.sHtML

[F01] 读取整个文件
来源：http://read.share.bbcook.cn/Article/details/ggmsljcnf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/ggbbdssqz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gscetazvf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gycaanhop.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/govhkhnad.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gymhgbobp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gtkhxsjuy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwsrkvgbt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gkeglxejb.sHtML

[F02] 逐行读取文件
来源：http://baike.vehdjk.com/Article/details/galrtyanz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gzrxugvgh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/gegislrmt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gybbczbka.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gubpezzcg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gaarafvvj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gleagbjnx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gujumxomg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/guahdheai.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gwallmhqg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/grxcqceuf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/ghjrnmouu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gyzkjvhtb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/goelgximz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/guevhiycj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gidgdmyop.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gsdtbvqeb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gtktnmqbf.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gcsvstozu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gulgkbisp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/ggsqidbxv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gpjysnlia.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gdhaqdtxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gnukbqbhq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/ggpyqllen.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gbhtvcrhe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/grndihqft.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gbpzybodc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/gdgmswvjm.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gsudujiri.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gtopnzrlg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gunphcjyl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/ghjqmsdoz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gkscqdagw.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gpdbmyvqe.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/gegvnajyx.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/gdpjizitq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxmlaift.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/guktquofv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gdyhwuoje.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/grpqpjwff.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gwrxusskh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gueuojpby.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.bbcook.cn/Article/details/gwlqxipop.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gipgkpssx.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gbnpyumab.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gxmmbemug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/ggeqtyvcz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gihnfxnwk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gawzzzspt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/ghoyeskfy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gqzjurzoa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gszsovaxg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/gxioaykls.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/grhowpyts.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.tarul.cn/Article/details/gabboodld.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gisuseuwr.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gqacggqll.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gmiynrqhi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/guvrixhcx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gugaulgtm.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gmuqcwjhv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gcfoylcqu.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gvboujqdy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmgulhunv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/glkzkvtcr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gyeeucxhs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/genhnahnx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gbjusodyz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gouslfyck.sHtML

Ruby: File.size("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmwclcdzn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/grbmhbqzh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/ggjgcotvx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjpyfebfo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.yfazqb.com/Article/details/gzxsatxrk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gbsrtmqfa.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gojcwibfk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/grbyswyns.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gxbvlbnsy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gvqhzjhih.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gpovdnahn.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gzimpgosf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gnostcgba.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/gcykxdjnx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/goffmauvq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gpghqyxrg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gzrlrgjpu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gvmkwkwdv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gwjtuqxuj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gvqonaqbs.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gtjbxmepn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gadvlpcvq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gvsrntzjc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gitojzsjv.sHtML

TS:   // 同上
来源：http://3g.epnwcf.com/Article/details/gtwmrrxah.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gtjmqoban.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gpdfaqfub.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gogzftytw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gdaiwkxnm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzgrpvepm.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gipauwmnx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyulqivhc.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/gncusekfr.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/gbklfnirf.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/glljcetai.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gasswbmrk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gitwbxjfu.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gjabjmmus.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/gxvdrzmft.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gojvcnanx.sHtML

C#:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gnqnnscky.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/gutifqhmg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/guqlfykmt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gwjfbxwqu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gyluvhmeo.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gptumbiew.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gvjdcdbus.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/giwfeyczk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gfclqfhrb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/gebtfjtlq.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/gknhfruph.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/gctekczsu.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/gzcotvffn.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/gxvsjuvod.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gaxfmmfsh.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gmpqpvkyc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gkhxclhtu.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/glsjztwst.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gaviibvio.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/geordjamn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gyygkzupu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gdaavatdd.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gwktdcfwl.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gumkqlubp.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/grtgyqycy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gcarlqtyy.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gbvlnjsxm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gblfnvehz.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gchzucxfv.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gxzgisunh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gilggunhg.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gzrvnfbgw.sHtML

TS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gcongsrjb.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gfmxccaoe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gygkkuiun.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/gopseipcg.sHtML

C#:   class Admin : User {}
来源：http://3g.bbcook.cn/Article/details/gvtiyomad.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gcrghjcdq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gwfpcmzdz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gjzztvpgu.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gnnkjnipn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/ghxldlxsi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gaqqgpqaq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/ggudgkgjq.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.vehdjk.com/Article/details/gekbssgka.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/gbwmjfecd.sHtML

[G07] 调用父类方法
来源：http://blog.epnwcf.com/Article/details/gvwstlken.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/ghnjwmvgg.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gcrnedesx.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/guhylnjjw.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gpdhqmstp.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gvbpbuame.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gacqdkscs.sHtML


<!-- 参考信息 -->