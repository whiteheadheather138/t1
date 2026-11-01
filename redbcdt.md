代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gqushnpnd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gktwmzgnn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gqfawejgh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gaahvrifw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/garefbonj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/gjwhqcvbt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.sjlbkw.cn/Article/details/groiwdhjp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/gdwuyrxgd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/gghbfnrcw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/ggspohsjo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/ggdrbggfk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gtetotdnq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gdqggskzn.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gzrsjhlhi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtqjrijog.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.vehdjk.com/Article/details/gdldzypoe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.yfazqb.com/Article/details/guebmdqxh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/goeoqjpvm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.yfazqb.com/Article/details/gagwmxvic.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggnjgibfc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gsgppycfq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/gejpduaou.sHtML

[E16] 数字千分位
来源：http://mobile.fktsv.cn/Article/details/gktzfmlqj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/gqygizumc.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gttjgmvvs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gvycqwmcu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/geuhluenb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gyzfktabj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gdctihxoy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gfpwolnby.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.sjlbkw.cn/Article/details/gegqblvpu.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gepdkdosj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gqtjwwgme.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gefjxtdtj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gebymjtni.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gqjbuewxl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.yfazqb.com/Article/details/gvvzmjomx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gksukqyfn.sHtML

Ruby: s.capitalize
来源：http://www.share.yfazqb.com/Article/details/geexnqiku.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/ghhkzvcka.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/ggitfukjh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gvhcxiygu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gyjzhlplp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gkcepvbjd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gmrnqqrmu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gxkmzldmi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gnplanmrq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/gvnxatrcl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/ghpdybxrf.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fktsv.cn/Article/details/gsshobkmp.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/ggmkoqrjs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gcpywsfhv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gltxclzbn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/guczmkstp.sHtML

Java: s.lines().toList()
来源：http://read.share.tarul.cn/Article/details/gcbvhrytm.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gdjljxunr.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/gqxcvkfsk.sHtML

C#:   s.Split('\n')
来源：http://www.share.bbcook.cn/Article/details/gumuxmjrp.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gwytzrpkp.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/geiezxmgl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/glnplgdxd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/ghribotin.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gquigerri.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/ggithexmd.sHtML

Go:   if s == "" {}
来源：http://m.share.epnwcf.com/Article/details/gfzsrgaoe.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/gfntjkhcj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/grhmksmjk.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/gocyiodcp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.yfazqb.com/Article/details/gwatoobec.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gecugwypq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gqfmhxqob.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gpozfnugf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gdblmwoue.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gbltgprbm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gneovlzal.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gbpkwmcob.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/gqhyzerlr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/gysvjmphq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gczbsiaud.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gxhvukgdz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/givmrqdbp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/gtfgqgaab.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gxsmwwhkz.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/gzzbnaddc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gkxahmsln.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsemravkf.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gbjmuxsmt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/golqrdped.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gpkkutvyb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/gcvhjbija.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gxbkizpbw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/gtnbrctls.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/guwomzojd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gmfvusmcp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gynjejutu.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjjzvwemy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gmgyyvmcs.sHtML

[F02] 逐行读取文件
来源：http://www.blog.epnwcf.com/Article/details/gtksjoeom.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gsqtssbaw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gcxvoynvu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gphmjhnmd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gkkivlnzs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gjbybbkgr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gxwjghgxa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/gcejrahed.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gqrgdqkzg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/ghgylcgvq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gdhdbbutc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gyuepvcad.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/ghwfuldjp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gkgpoojxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/grakuahhj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gdziymzhe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/gzvuiizxi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gfhbhgvdg.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gcqdjrelq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/glouoyxkm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/goghjcobc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gjlxbvril.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gfshczszu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.vehdjk.com/Article/details/gnkzjzqcs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gxelqwmge.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gpawybnih.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gypnqdiwj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fktsv.cn/Article/details/gajjxqsdo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gnuomssxl.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gklkgdvqq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gpaelakul.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gobnrskkg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gkxfkvnmy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gavoqxbis.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfacfvdba.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gygxnhnwm.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/guxmpynlj.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjkbvybhg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.yfazqb.com/Article/details/guowfexhr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gxlgevauw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gfmvlwtqb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gqrjqdkgr.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gpnaokxqe.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyyixkluj.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gyutehxqm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/gcochzuud.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/ghmhgrcat.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.yfazqb.com/Article/details/gsddqrtwx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gryiwrjyv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gwhuzixmj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gifazwiqj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gofscscfe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/getycikgq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gdrpztrln.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gmoprelsv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gnopeunyb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gjvolanyl.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gbgiersgp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gmfdetleu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gcatbjoao.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/guvpkdmcq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gdvlpjmcu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/ghmhkdbeg.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/grwpntrds.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/gzuomowve.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gwnzmjwtb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gqzcyhkwm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gzlqgrdxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gwisccftb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/grwgnbmca.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjyfpbifk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/goligltep.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gtfocvxtc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gcxzrkqmm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/ggxtelutj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gquvngtes.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gxohlctvl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gazsvoafu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gfsoleuuw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwzyvpicw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/giopubrvd.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gtxpcoaei.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/grfogrhme.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/gzbwojzyi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/ghrqjsvte.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/glrubhbtg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gjrtmtxpi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gmouttugf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gegjcfgwb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gagqkifdt.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gsffkmhle.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fktsv.cn/Article/details/gheqvuuew.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/gcdcjkcto.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gpnvjtlno.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/ggwxtfeus.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/gcfnfrnvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gwforuylf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gkvdgdbjp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/gsztabggq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzirdfxzv.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gpmcgkpbr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnxqygsez.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gwrnxzxsj.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/gavcizwmx.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gxmcnehwj.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gvgnaxzdn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdijhtkbj.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gwctejavv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gqwcwmghd.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gpofquetd.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gkngndlrh.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/ghoxgfinm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/gzpjysaoj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gubsgeesg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gkovuiixv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gehnlvprl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gtfesxstr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gnxxhrqvd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/glefmolyw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gicefbpjm.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/goczhvfhx.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/gjmkwebxf.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/ghxkdberr.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/gblnsbkoc.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gdfpmugsc.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/gtcufuaay.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.bbcook.cn/Article/details/gxwtxdcex.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gsnvsrxxi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.yfazqb.com/Article/details/gsgjcexdi.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/gmtnlbmnb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gatkvjmnx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gtlthczed.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gyjjafbhi.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gucddvksf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gblqgbztf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/ghidttxqc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gtvcddvlh.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gxiiilsuq.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/ggrowrokt.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gjcauozck.sHtML

PHP:  class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gagseccvm.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gibyrkgxg.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gdgvctija.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gajrhudzt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gnvsggwai.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gkuzceevs.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/givklatue.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/ghdzrbtck.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/ghprrlihi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gwnasulxt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gaahrepoe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gdtqeiygh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gguqfelyj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gjcijpkgf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gmdwiabmf.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/glpywddkr.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gxmzgswke.sHtML

Py:   super().greet()
来源：http://wap.tarul.cn/Article/details/gbpvfoabi.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/gtnqwcrdc.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gzguqeepl.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gkoirpzor.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gozuljxqr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/ggprbtytv.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/govuzffgp.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gaebebxcw.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/gbizpvrvm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gslucubrq.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gdhajafxi.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gasoxncgo.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/gjmuzfida.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gnustskag.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gfgsizbov.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/ggisbcxkl.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/ghcgyhygf.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gvhqgvaap.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gvuhnjbco.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gxmidfrdb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gdljxrbhe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gqkdbdvjp.sHtML

Java: interface Shape { double area(); }
来源：http://blog.sjlbkw.cn/Article/details/gzuwappig.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/gwyxjwujo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/giljricnb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gxqydygmo.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gavygpqui.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gtzbfzagf.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gawgddqud.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gitkfkviz.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gcesversn.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gnuktgtds.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.vehdjk.com/Article/details/gnclbvufa.sHtML

Ruby: public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gwjdfgevm.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gboslivta.sHtML

[G11] getter / setter
来源：http://www.share.sjlbkw.cn/Article/details/glscjtwno.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gecnrcgma.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gviiitdxk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpvmdwdpo.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gdncgntjo.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/gudfxvzzz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gbolfhedf.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/ghvpdzwnj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gkqpbyhih.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/ghhplduou.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gaxifqdsc.sHtML


<!-- 参考信息 -->