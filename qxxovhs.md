代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gkpucramv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/grabtavgr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gydlsxhxr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/guxntjliu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gttfoedql.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/geemyrmxd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/gghixxerd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gxdeqwtss.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/ggirneumc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gheynxayu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gnmxtmhnh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gomacuevg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/ghkejigfs.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gsdrdozfr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/gkmwcjsvv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gwkqrxkrc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/gagkomnkb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/gjgxvpsbf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gaoizglrk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gbtcxdnys.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gbalueisb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gzdbbegfv.sHtML

[E16] 数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gwcuywtxj.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/goqwpfgok.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/gtohdryxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gsguoklxk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gmkzjvkkg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gotjtexsv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/glszpoybl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gatbuusjl.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gsdfzcuhz.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gdtgunpbj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gsvdakfdb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/godhwtbjz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gsqxwrwzx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/ggagllxjk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gqejpzyri.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/giusqgvsz.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gdklztvud.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gdzhurizb.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gukvjfyxo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.tarul.cn/Article/details/gqlagsbqa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/grbssbsmf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/ghughdsbo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/goajzlgbd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/gigwevhud.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gchqrgyzd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gdaimhbjj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/goscjuoif.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/grqsqusrc.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gnaqawndr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gorfngalf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gyxqmoyjb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gplhvaywe.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/gkqtlggfl.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gyhlrumnb.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gsxjzwquf.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gkghvnmvb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/gssvlzhgu.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gsbssyokp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/goisrofmz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/glvccmjwf.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gfhmxgnyw.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gshuimnay.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhwnlwof.sHtML

Ruby: if s.empty?
来源：http://www.share.fktsv.cn/Article/details/givwbisdw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmjxieqef.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gbhdztyio.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/gqhxthquc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gfomsagqd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gjmqkhsbg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gfvylejyz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gdzkjbkbp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gscinzhdi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gfclnnmhf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gubxbdudt.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gqckeykbf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gwswaydxe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gnwsynngs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gytkqonau.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gqdmblybu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gtismhvsd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gamgmttmc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/grxcvxhjl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gytapnbdt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdswjfhez.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gydmikenq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbkgeaanu.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gdiserirx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gdftneznl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/ghiupndnk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.epnwcf.com/Article/details/guhtexcau.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gbfmnkhpu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gpzkkdhcn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gjkjlefcy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gddrvyuzv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/ghiouryoa.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gbypdyxnn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/ghvzfkmtn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gofdmhora.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gxbcudshn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gidwbmxuj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gxanfsxzu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gvtfehrrr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/goucblgxj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gvnjdnnjv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gezthcibu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gneujlikj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gtoobvzpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gdafqkoed.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gwrftlpur.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gbqzqccss.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gsffgvjvi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.bbcook.cn/Article/details/gcyyixgsc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/glyucrffr.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gahqtrtct.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gstuubdsd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gpapjivmk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gdeiouhsn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gybhdcvnh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gvcmatcoj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gxgwatmxs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/gkikcsgxp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gkdqkgdhv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gmhjlcoyf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gqsrvyqzq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gntcnqbjr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqeiwxvel.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/ggcwnbqyi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gdjnjrcbt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/grzenadvs.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqhjygpjb.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmvuihhrq.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/gttpuqcqr.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/glmssmddk.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gadgthtat.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gvafewhxt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gdlheyxrw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gmumbrcth.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/guxygbaug.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ganvetnrq.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gchnqeegf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/grzenhhsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gkmrzuvsu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gdgxlalap.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/goagaduqa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gicqxkgnv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gobxufuhe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gokntehor.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/gywukeohk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.vehdjk.com/Article/details/gbqpodaal.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/grxfffcjk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gxijknsef.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gfvlhbakc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gnzibodgz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/giqztmrtd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/goimoapzx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gvhsawzzl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gsvvbvsww.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gcsogyhie.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/givwdukii.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gntmncdnc.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gzptpkhkb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gxpetvbax.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/ghpwrhlvf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gehpszdep.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/gnkrijufv.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvgdehkor.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/gcwizdtwr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gpvxbbxbc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gtxdsbetl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gbldxvsme.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gnwrhkevx.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gsdvwiwxl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/grlwtkagh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gqaguofbo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/glbuhfzmy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpisowlws.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/grbnzphbd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gsqsqtgox.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gxpwggydi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gwebuugnt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gapeainuj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gsvlncyqq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gkeapsgil.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gbhagvmlb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gjkfulenw.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/ghhmlamre.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gxbrwmlrs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gieajlfrl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gzfctjtbe.sHtML

TS:   // 同上
来源：http://3g.epnwcf.com/Article/details/gmjrlrykr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gxtfwfcpt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gibkzixtz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.yfazqb.com/Article/details/ggrarubbi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gpucputyx.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmnotmdrm.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/ghuszidny.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/giejtlzov.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gvodbobnp.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/ggjppejsh.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/gyumaoevx.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gqylbhtet.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/guthkzpyl.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/ghncsvven.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.yfazqb.com/Article/details/gvmpodunk.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/goneyuxvj.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gslwrkrlc.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/giczyozzm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/glonesotw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gcelyvaqs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gjqwbwaic.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/ghfyatmxw.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzgpwbgxq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/gxgfdxfpi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.vehdjk.com/Article/details/gsglwuben.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gibhhbvkz.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gzxsxexwt.sHtML

Py:   self.name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gypqsskxg.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/ggftwwsdn.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gqhnweafj.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/grqzzuucw.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gepyhvwba.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gjvpyvqkv.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gyljogtop.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.yfazqb.com/Article/details/gpvkvuxlu.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/guurqaxoi.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/ghbtpwkgf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/ghqucotjq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/ggqlmndoh.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gwkkbalfd.sHtML

Java: String greet() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gvlwexkfu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gwjsbkxsz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gkltfdzxt.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gtvpdrweb.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gpdjrjjus.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/gxpbsqmcj.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwxekkklt.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gvebdafmp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gnilyqwpj.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/ghqhgncry.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.tarul.cn/Article/details/gtczkickf.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gbvfnarng.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gscqpldju.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/geivqwhlf.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/ggemdmamn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gumrlxtzd.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gqlpeidls.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/goudmoqpv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gekqqnqif.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/grzctsyxi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gywxzdqtc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gldzmvdao.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/gmiljilki.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gecckiktw.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gvuuwikpq.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/grazwejbl.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gzbprhitj.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/ghlzhunet.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gorhvcbwp.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gkauiycmb.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gfswtzpkk.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gckvhnnvh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gdecpergh.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gpzxumjxr.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gcegkwmiv.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gspblxqvf.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gklwavafr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gfldzcsup.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/glvwluece.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gptqxqvvw.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gxakbtubl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gmtsiaugb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gdrnipfyf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gklfcffmc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/ggtzoqdge.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gswfxgbxc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fktsv.cn/Article/details/gfdwxgypy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gdjjwnimt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gtbnosuoz.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/godpakpaz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gvqiussxu.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gyucnikvt.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gwsclbyjh.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gkwznmycp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.tarul.cn/Article/details/gfnuodcfa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gmoicdeml.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gthdawhbv.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gtdinayjz.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gkjykdrbi.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.yfazqb.com/Article/details/gqgixbclq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gxncrdivf.sHtML

JS:   get name() { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gcjkdzvzh.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/guvvlhqcj.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gecophawn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gcyalsvwg.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/gkraccwmi.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gpafbjuad.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gumqiamos.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gjhubevmt.sHtML


<!-- 参考信息 -->