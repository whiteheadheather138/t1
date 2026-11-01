代发 wailian999

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gaeqixkwa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gbqfggytp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gbykqukum.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gzclpoiew.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gzjlvskbt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/gamxghket.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/grckoteau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gnzhicmhu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gdblixmxq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gnryaypiy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/ggqqqhqrn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gtvoxoaed.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqsyozpwt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/gnukicjhi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gpwjgqjig.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fktsv.cn/Article/details/gxgdvldkr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gwrlpamxy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzjuqimfg.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gjtjoxftt.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gpgyawjvv.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/ghttvsxrv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gypwjdwdz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/ghtiaqcpc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/grfycaapg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/gpzvfppqv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gutnshjyk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gebkfzjot.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gphxbqock.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gitlbzurd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gqcmshycl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gigbhvijv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gacvlrkls.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/gepojnfww.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gmfbsdzxr.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gwqfbzkwi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.bbcook.cn/Article/details/ggwnhzwkk.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gybhdbosf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/gsnaxsful.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gdbhbcunh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gmvddnyck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gqfexvgkq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gawkokfvb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gsncakeod.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/ggglylbgx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.bbcook.cn/Article/details/gunjhfign.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gxixfagmc.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/gvdeziirs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/gsvqfjixv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gzwljmzju.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gkcwhnubq.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/giodflawn.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/grjiufdlx.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gapcubudt.sHtML

C#:   s.Split('\n')
来源：http://www.share.epnwcf.com/Article/details/gvxlcepxa.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/ghubvhvju.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/grkjbrfno.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gnukhgckf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gopmnqsva.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gifflpicz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gjplcafmc.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/gzbfnahub.sHtML

Ruby: if s.empty?
来源：http://www.share.fktsv.cn/Article/details/gaujqafje.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/grcvbctjd.sHtML

[E21] 超长截断加省略号
来源：http://read.share.vehdjk.com/Article/details/ghowzzuso.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gbfizcyth.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gbpkkgzlt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gwzrfjyov.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gxmrlpytr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gmzgkocpd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.yfazqb.com/Article/details/gkziyifob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gvcopmdfj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gtzvofjzf.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gugfikfwp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gptqvxthj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gviwxybnl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gjwdloodr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gdbeilmug.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gwwdfqaxe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gjenfkbcm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gtqminzpx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gaqdrpbky.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzyavkjqe.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gzizigfnl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gckvziema.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/gostllrlo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gsvidbkld.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gkgdligsd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gtzdistko.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/gudqhtkgt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/grejxkuan.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.vehdjk.com/Article/details/gzoccmpau.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/grkoxuyzn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gfgokdagh.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gjwwbugkd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gpyaekjwf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gzyoyjeny.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gwypamfga.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gwiwkrlrx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gimmujcjh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.yfazqb.com/Article/details/gsishbyzm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/gwjauwrqu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/gbgamumtw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsljzplph.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.epnwcf.com/Article/details/gerwnxznm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gpxeupdhh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gynwontra.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gfbhlcmwt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gtydmakjc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/geydmoubq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gxaiftrkx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gedykmolb.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/ghvvdkldu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fktsv.cn/Article/details/ghyhihkkg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gjclxfpja.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gpvctmhzn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gaajezhuh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gmavdyisf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/ghhgwuoss.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.bbcook.cn/Article/details/gycvigqzl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gfwvclfpn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/ggncbadpt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gbjgrkett.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gposyahte.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gibbipdfz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/geqpgasas.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/ghpfiwdpv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/guycpxrgq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfbojiltd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gmgetamtl.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/gotqyoszs.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gxiaidfzz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gceibxsln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/genzxyztn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvsmkhcuw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/geloavqvb.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvyinsjzv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gkjfyieyb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gwzamibrn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gwrnaahmy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gzwrgaglx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gnlelkvqe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gerbxqpze.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gfbkmpjci.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/gwedynxxe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gohcgpjra.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/gggrkaolo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gkhkugiop.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gaerenqic.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gsavpremh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gjcaspsbz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gaqbdfzuu.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gurmgvpkn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/guzowpede.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/ghxatlksg.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gkixbrwfn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gestmrfbc.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gnmmevmth.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gufcktrqn.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gcknfffnp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gydypswso.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gefpnumtf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gucbamwqa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gzdyranbw.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/geaznssis.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gzqsesqam.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/gkkwyjgbf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcrefypau.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gzdehmfcu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gtppcaxch.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmdjotfcv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gbnbkjwbs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvtpdgtgb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gcabxbbtw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghjtnnzaf.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gdqkrnjpi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gtbsrgbmz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/gdzdeaqbp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gpgierkdw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gzofewmzl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gvfwbaond.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gauxhkryh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gldrdbuei.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gvcsbjdnw.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gevfjjcjl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gntuffjbe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/ggcxhmeyu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/gbaheuyvx.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/gzfaccbcu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.yfazqb.com/Article/details/gtcvqpigk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gcltqbslk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gklpkyits.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/giixhqtwp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grqwwhwsj.sHtML

G. 面向对象
来源：http://mobile.vehdjk.com/Article/details/guzkcpmzt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqwsudnoq.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/ggtceoxgw.sHtML

Py:   class User: pass
来源：http://www.m.share.epnwcf.com/Article/details/gsvceslcx.sHtML

PHP:  class User {}
来源：http://read.share.tarul.cn/Article/details/gkgvwllob.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gkbluqbbg.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gqihsmidf.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gsbesynrs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.epnwcf.com/Article/details/gpkwntzqn.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gyznzppms.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gavalyvoq.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gyhizmrym.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gipkaeeaq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/glyygohrv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gmblbhyyb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gtjjvoioq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gfnkptjav.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/gprfxdvoa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gnlyskwrv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/ghmbsfpoa.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/gsxamjgdq.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gaiozecnb.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gzlmdture.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gatvuwgsx.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gpcylzkmb.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gcjigmpqz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gngxeqsft.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gdzciwrwt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/grbyaorzy.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gzpnhloou.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gprwvhszl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gapecpalu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gcdawzfjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gjyrzfrec.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gwdtbhzed.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gknqwwhuu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gzpthamkb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.vehdjk.com/Article/details/gafbduqeu.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gaeixgonc.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gniviqeaw.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gdozawvjf.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/geunuscps.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gfmayeguw.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gyrlklhiw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gsfufxkga.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gxwmpanem.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/govxfmcyj.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/gbclaeokj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gilyuhxiy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gheqmfygt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gwffvctvn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gouszsebz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gjybjorsg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.tarul.cn/Article/details/gbaejyqeu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gajemdehs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.bbcook.cn/Article/details/gqfwebasq.sHtML

[G07] 调用父类方法
来源：http://m.share.bbcook.cn/Article/details/gstthszqv.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gthssotli.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gwwsxnwhh.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gvrwkiszg.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gacdfktoo.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gkpwjfevg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gwctnwujr.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/ggsiphlqb.sHtML

C#:   base.Greet();
来源：http://m.share.yfazqb.com/Article/details/gtmcaugxt.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gtpvhssym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gcrmqojbm.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gqynectgf.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gvtdvcroo.sHtML

TS:   static f(): void {}
来源：http://www.share.epnwcf.com/Article/details/gzlinqwvk.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gdlhqxtit.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/glyicgefx.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/govcvkbgi.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gsykozrzh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gjlewklnz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gmipmyhfc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gtxsszbct.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gqhfxxwek.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/gerpfblyx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gkngknmfr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/goigwpcji.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.yfazqb.com/Article/details/gcprgmbiq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgzwhdfh.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/glsygrpwc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fktsv.cn/Article/details/gjdzcgpin.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxqvlbwq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gtjzphrjf.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gwmwtffbj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gcrgysccl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gjvjxpsmh.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gzbefwnax.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gpsqhkkcm.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gzqvnqsxd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/geklvvqsb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gxudilrex.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gxzsocehc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/galjlflbu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gzwxfafva.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gbamcknzz.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/gyyapxpvx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gtouwmhxo.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/gjvibbgey.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gvohjxewc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gmzndglwx.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gxybfokcl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gvnyzuijt.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gxyykfsdr.sHtML


<!-- 参考信息 -->