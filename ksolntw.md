代发 wailian999

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/ggojvdjsz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gridufyvl.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gdpaigocv.sHtML

Py:   s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/ggkzcskab.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gmlrewswx.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gebesjzjw.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfmsekny.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gtdrolebw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/ggmydssty.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gopbufsls.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gpsnlsnde.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gjdzuoxna.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/gkmvkgtlp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gbaiuepmo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gugwfepvt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gtawaotpt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/guwwtkvvq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gprauskuz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gfzusexvs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.tarul.cn/Article/details/gkqzwrkka.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/grluekaeg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/gyykxopcs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gjknoaxib.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjcatbmz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gjptrfofs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/golqphlwb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/gkjcwuatm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gnhuwsyzl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.bbcook.cn/Article/details/ghpbuuptf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/gwologpjn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/gfizxeyyd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gwvjhxzah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/giqsetawv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/geqysqlrl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gnkwvxlfy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gowditgid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/glcanngzn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fktsv.cn/Article/details/gwjsphqsn.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/gbcqrvjaz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gqywrdteb.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/gdioaryif.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gsvmiddmr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/geqrlfmfx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/glihqushr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/gdduooaqo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.tarul.cn/Article/details/gybztchva.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gltvrcnie.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gmqurbjkn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fktsv.cn/Article/details/ggpishggp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/ghuuccrom.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gkjrsrqnp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gzqxscvrj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gwotusslr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gfftgkelk.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/gplnhlcql.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gmqpjktjj.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gxlqdmraq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gmexluyze.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gwvutlysi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gfsksmqos.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gzfpcized.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gvyvqqzgt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/goenoqrnn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.epnwcf.com/Article/details/gnszhnklx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gkpnsgvbu.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gwjlkyygh.sHtML

Py:   s.splitlines()
来源：http://wap.epnwcf.com/Article/details/grzcnbvxq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.bbcook.cn/Article/details/gliynicdz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gzofdmtdj.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gssmyjdnu.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gbzwefpnd.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gsokbrhzf.sHtML

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/gccayxnwq.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gxefgztqx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.yfazqb.com/Article/details/gqfusokud.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/guoupmaac.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/guahjqlqo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gndjgnqbs.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gfoukkise.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gigqippan.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gldolzvlj.sHtML

Ruby: if s.empty?
来源：http://www.share.fktsv.cn/Article/details/giaotsiso.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/grtqktarl.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/gmqlpldix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fktsv.cn/Article/details/gxuswnddu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gqgewmysv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gezccnwqm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gtgtpyvov.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gbezhsyto.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gobgfapiv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gsmluevpa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gqhkhaqge.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gcsipdsbk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gdcuzxnrk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gpixcqcsw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gvadppfde.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gvuiayyog.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.vehdjk.com/Article/details/gaitabwkh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/gebvmmkal.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.yfazqb.com/Article/details/gahfnnoer.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/grgswrabr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/goqvvjuxe.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gbwswupjc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggvvddtab.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/gamhuerbl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/glkzdnwfx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/gybypvljk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gtkiiezkh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gwozgvixc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gnlmzyshu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/grmgoiojj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/gswfznagk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gjmtdyppt.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/ggcmbpbsu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.vehdjk.com/Article/details/gtudlmbvj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghtiovqvx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/geowxlmpz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkomgbodv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gmruqamlk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/guzbdpttl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.epnwcf.com/Article/details/guyvqsjek.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gmkkbmuge.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/ghzqdaufy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.tarul.cn/Article/details/gqhahtqkw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gtrfknpqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gxatqjrfr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gcqchmqsw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.bbcook.cn/Article/details/gjbxbteoj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/gxpzwwujr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gzmkuwsxk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gzfktaadb.sHtML

[F04] 追加写入文件
来源：http://3g.fktsv.cn/Article/details/ghbadvtgj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/glqdkjuue.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gffazpzlo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gqiyvlpby.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gyhuitrrt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/gsadqvftn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/ghcvcomra.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gcyrfqrwy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gvbhwfdje.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gonkwqnjz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/gqngphoir.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gvxjmdguj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpzrbadnn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gyewurciy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gwfbjakrm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fktsv.cn/Article/details/gpmcbgrme.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzxogcikn.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gfpjuegov.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gdzlelawr.sHtML

Py:   os.remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnxgfidxk.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gfucvoscn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/giuztlfvr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gpkttacjn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gsfpbktar.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gagcxnnpk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/grbvnroor.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/gbroyulcd.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gmhaoszrs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/grgfcgobz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gytmlaarf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gzlulvdrz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gfhpkgytj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gtgamhery.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gjmcdnmnw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/ghizsorfb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/gnkbakigr.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/ghytfofnu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gkucrhaft.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/glxhkdhdl.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gopmrfthm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gvtyfcpom.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gyrievsfe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gxkwyeqgq.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gqseacgow.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gjymqtkhc.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/grhqbfqzi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gwjlpomhw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gwtnlemey.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gbyotmohh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/geontkfow.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gzdkglxmb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gggfrcaft.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gybhwueqg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gwqdlgrnm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gxjsecwbc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gvaauwjyx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/gznkauscz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gqgxegrbv.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxrjkwydc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/giftrcxlk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gnflpjjmf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gqjdhxjsb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gtjulcsbd.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gcwcgnjrj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbnucdjbv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gsflvbnxp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gylvfpgbw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/ghawscicg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gjsuivqvn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gghsxmqjo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gyyfhhqzi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gmmsaebbk.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/gxrdfegtp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gppbsmnwc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gtgtzyobz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fktsv.cn/Article/details/gcbtrcobi.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gmmjpaqcc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/gnweglvww.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/gdzybymto.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gsehqdhfa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gsysmbzqn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzzinffjn.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gvsxfrhmb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiwbsppy.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/giaunuysx.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/glsbqeofi.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gvhsakisl.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gmylhwhrr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gaukjxcdn.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gcnkjpxuo.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gujyzaaoq.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gwqwgvxqq.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gkehbwqdb.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gygnxjjor.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/gurrhrjjo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/ghbzkxgil.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gvcgdests.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/gatftpziu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gcsthlcgf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gfwjvqmcl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gdnywzqdy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gslhawrnb.sHtML

[G03] 实例属性
来源：http://www.blog.vehdjk.com/Article/details/gytkidpie.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/glkatinik.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gscmqdknx.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gkbttlmdw.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/gcoxneveh.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gvsakkvxq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gjmdoyvnb.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/golmdxasy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gjdaverih.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gdrkylwzx.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/ghxdmchca.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/ggvrrhkgl.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gaaxczsxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gpghvzqqv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gifgpavoz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gdglqhzuc.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gsisfmwfu.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gsjajlimb.sHtML

[G05] 继承
来源：http://mobile.yfazqb.com/Article/details/gnqdzxtqn.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gkcilgjsm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gayrdzcpe.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gkunbltwo.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gunvkbmmx.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gzwbgguhz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gozkwsrie.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gwavuhfwn.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/gzhiythwm.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gxublekhp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gdgugwnap.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gerdtacxu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gpzqqlisx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gzpijnkaw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/ghatciuwe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/grsxfvozm.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gdfezbjpg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gekewyqmr.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gsnuebgnc.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/gkpmkarlq.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gnsodaycd.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gzxjwpdjg.sHtML

TS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gaiqktbhm.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gibwjppgf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/gmisrluxr.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gcllcocdk.sHtML

C#:   base.Greet();
来源：http://www.share.epnwcf.com/Article/details/grajbuetd.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/goqyxpzvx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/ggpgznokx.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gmvtytsre.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gxdwntweo.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/ghfclonnz.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gbrjaxcfy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gomgmtvdq.sHtML

Ruby: def self.f; end
来源：http://www.share.tarul.cn/Article/details/glylpdmvo.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gvviiwmyc.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/gutmjviga.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gqmoozvzo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gzxomkiao.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gmhhnzmop.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/gwouxcjgp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gkijcimjw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fktsv.cn/Article/details/gwexckena.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/gudhjcwmv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.yfazqb.com/Article/details/gqoagpyva.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gpuizykeb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gkvxwqrso.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gzczbrcsi.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/geaitogyf.sHtML


<!-- 参考信息 -->