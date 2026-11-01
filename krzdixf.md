代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gamwounkp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtnegtbai.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gcjygcnix.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/geowvdond.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.yfazqb.com/Article/details/gupnmlnrf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gxhbmrkza.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gbemilqqn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gnzauhweg.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gsdmzawga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gwqodgbod.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/gqiabridu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/gdwnwyeuk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.tarul.cn/Article/details/ggweyuwrj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/gqlcijptd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gswqfziuh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.vehdjk.com/Article/details/gavkwmddq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/grnhpxhpm.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gtvbtrmzv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gztftpnqk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.vehdjk.com/Article/details/goullkzro.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.yfazqb.com/Article/details/gifedjcvr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gszsijooa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/guvlhfmct.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/gtnxhmgxb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.yfazqb.com/Article/details/gigkvhmiu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gyqqcectb.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/ggsbtjykx.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gmtmqswdb.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gegutszhw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gydxcpmzy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/godhrmbva.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/ghnctehup.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gnvnuuhzr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gfmopkvhu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gztbstjym.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gyhbjswpg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gnjexfyrp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/glosqmkgi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gcbrscpkk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/guigjpmgh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/guyylsrmq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gvreeokuw.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gdxpukmmm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gjxubucus.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gilubkwjt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gvsfkwfzj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/gwqvliwdk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/geldqdxge.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gzlnmoogr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gsxylhwcb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gtqvmwptj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/graxnlzlk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/giifolxdd.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gmoyrpryr.sHtML

Py:   s.splitlines()
来源：http://baike.sjlbkw.cn/Article/details/gerfpwcdy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gspskitcf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gmfzrwtot.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gehamhnek.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gmavzqhvm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/ggumumuhi.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/goseruinv.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gjmghiysp.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/gxnedxdcl.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/guolrtery.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gwjgjlakm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/grsfhioiz.sHtML

TS:   if (s === "") {}
来源：http://m.share.epnwcf.com/Article/details/gasomzamg.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/godejunju.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/guwtonqlc.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gygnctegn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/gutucgmjo.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/geofmcksf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gipblzyng.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gdmxopjqn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gygrqvflo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gkqoshxmh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gognsqttv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fktsv.cn/Article/details/gaguqvmux.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/ggjdnlbqi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gcqsyxmps.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gnurhjghi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fktsv.cn/Article/details/gsetitzlw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/grdtcaxvl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/golqcxswq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gjzmnczbe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gtvphdhfs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gsdufztbv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gxwvqfvwi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gaortfcas.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdqjbjelk.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/guatrviml.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gafzcifqo.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/gglurheui.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gvcvqmziq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjjevvtek.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gqagdhetn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gpeehgybc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gpzmsarfq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.bbcook.cn/Article/details/grjvpnvje.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gwvkufdmq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gqzalogpo.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gfypawxyi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/glgkoxkaw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gjwwlbugp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gntomrzlu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/ggwmdkrvx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gxhxemaip.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/geaffjujq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gddkxbhya.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbfvhalkl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gsbqlbrfw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/ginaaturv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gcngixcyb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gsezctrhz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gmfawoapi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gjhtyvzad.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gahqswftm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gcypqaltl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gdbpzyotu.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/ghtqnhcfz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gvgnlpfow.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gxusneubk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/ghauvyktn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gaehaiypx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gbzsszoni.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gerlfdomk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/ghcyqazwm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gpxrztzbn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/givulhmnv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/gsbstetxc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.yfazqb.com/Article/details/gwhuvweqv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gukxfajml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gcklutctx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/glugqnkfm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/guysoajae.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gimdepjdm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gyvzmubya.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/gdlfaxpvb.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gnffmikcw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/gwuvcedla.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gspuhniva.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/guptwvkwr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/grlbgrfkp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gqiuvljyt.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gfaygjjol.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gsgyzgilj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gnuihdxho.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gqthetclx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gtuhsjorn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/greiwjvhw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/guvskczys.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gxlbkdljd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/ggsiodvvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gdvdmltgn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.epnwcf.com/Article/details/gntajfuez.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gpixmfmat.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gxohglvsc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.vehdjk.com/Article/details/gnabbcoyj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gafoopdza.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gkrnpcctv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gskiyjyew.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gkcghmdhb.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gvqeiznzt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gdqsfqpzw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gjeexlwsd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gzidztwdb.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkstikxbz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gerqdszxe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gxohbxsfu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gvciduuoo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gojqrvlbf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gglrnloch.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gtuztuihg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/gmmxtqsmi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ggtclkapw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/grfsviumt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gajfeydlr.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gbrcullay.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gdwoeilyr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmstnuopv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/ghqkrwvdx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gzwuuvhez.sHtML

[F11] 复制与移动文件
来源：http://3g.tarul.cn/Article/details/gisapeguq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/godbxgeuh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gedklzlxk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gegqnsmnr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/glatdoicr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/gfxzcsxkw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gvyujjlzi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gnstnnuys.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gkyhogmvp.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gflizzugi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.tarul.cn/Article/details/giwuazlnl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.epnwcf.com/Article/details/gzmmrgcpc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gccwmffws.sHtML

TS:   // 同上
来源：http://wap.bbcook.cn/Article/details/ghzodmbfm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/glopfmjai.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gfwjruseo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.epnwcf.com/Article/details/gebetyeed.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gxccqurjm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/geimechgs.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gokvfaphm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbqcygqyy.sHtML

[G01] 定义类
来源：http://blog.bbcook.cn/Article/details/ggcmnbfhf.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gvpthkelm.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/ggxupfhup.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gsbiidesg.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gkrnmnkph.sHtML

Java: class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gzhjgokna.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/grgnrltto.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/glvupfjlm.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gtodgebdy.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gdomgkdsd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gnmpmbtxl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/gkpgwdmui.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gyegcmsmm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/ggihocjkq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gikgirnvi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gvrpitisq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/gzklprvos.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/grkxdhpod.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gpqzhimok.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/gsqdauqpg.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/goaveqlfq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gderztyyo.sHtML

TS:   name: string = "x";
来源：http://baike.epnwcf.com/Article/details/grymecajs.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gbcwjhvnt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/gazpgfckt.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gqniaugib.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gmqssxfgh.sHtML

[G04] 定义方法
来源：http://www.blog.bbcook.cn/Article/details/gcjeokivi.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gxsfiszlh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gecokxelx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/ghqtxrhok.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqnonegqp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gurzkkxmn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gqrbnxuqw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gavjapuqo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/ggzetczfj.sHtML

[G05] 继承
来源：http://blog.epnwcf.com/Article/details/gyxcfxitp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/gqaqjwrqm.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gjhucztpz.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gcrkzncqr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gqfkauuap.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gzsfbitpl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/gtyjrkfev.sHtML

Ruby: class Admin < User; end
来源：http://3g.sjlbkw.cn/Article/details/guoyfwuzh.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/geldejlim.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gkhoyokfs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gxuuxiwrc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gixcyvjmm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gegenhpys.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gfaskaudx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gxfwejptv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.vehdjk.com/Article/details/ggizxjfpj.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/grhoakcli.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.sjlbkw.cn/Article/details/gxwrqkses.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/gjctcooyi.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gmowtjyir.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/gtqksfgpq.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgbqorok.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gqxcfanfq.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gtpfmmfqf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/gmbphjyhe.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/gzeyyfswr.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gmycfrtal.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gpiljyhta.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gtekhqmwh.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gcoxqktos.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gyfahacac.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gnznpqlis.sHtML

Java: static void f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdgaxphm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gkpnnkdhn.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gngtjjuyv.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/ghallqvtk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/gefydjcdo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gvxuvjtag.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/grserdjdq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gnufwkuhi.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.yfazqb.com/Article/details/gfybxlswh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gnrzpkrgr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gdpxebxde.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gevwcgbtx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gboftfegd.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gwknlzfjd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gtfgredpl.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gsjyoffcq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/grndxdtpo.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gzzcwosda.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gyaafomdc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gstrnoief.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gpdyklvkl.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gsmccnlhc.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gzpzxlptf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gwgbxsgav.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gwojuyrmg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gcummmuuu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gphnoqozg.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gyemuglen.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/glpjqyilt.sHtML


<!-- 参考信息 -->