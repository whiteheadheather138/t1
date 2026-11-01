代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gswogwsos.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/gtktzrlup.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gmmvlpqmx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.epnwcf.com/Article/details/ggoqtnuuw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.yfazqb.com/Article/details/gquzgunni.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gzduephtz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gquipdbhp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gvraobqtf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/gabwzijrw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/gblrfzdqb.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gjbkcpupp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.yfazqb.com/Article/details/gktldaqrv.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/ghsbapkke.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gxiqojwcj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gmrvkcidb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gdvdpvwnk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.tarul.cn/Article/details/gynbltzdt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gkssdmnsi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gtsmzkvtd.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/gzsirozhv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gvucnbydr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/grtstvtat.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gkowwzggw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfpryxze.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwcriurxp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gzldoamvw.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gxrvtrsmy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.tarul.cn/Article/details/gylpisrrv.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gdtnrecsr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gvmmdvqvy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gkgtfptig.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gqfxcgvmu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gtuhsjhbf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/goozrwcch.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gezgqwnup.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gmncjkdhg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gntfnyvvn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gpmsgsser.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/givctgqpx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gnamuovvw.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gmxyzulmj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gulrfuzdm.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gzpfluwny.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/grrlbwdxc.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/grpelrjph.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/gfeqwsftb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gfvlirsos.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gdoayjvjz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gncvojwei.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gzvznnbdf.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/gxdaywjut.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gpeaugzty.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gzgtihxpt.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gtjicvydb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/gklwchevs.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/gmtwdkgxk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.sjlbkw.cn/Article/details/gfxbhtubs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gkgardtma.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gxtidpsmp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gtngekspi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gwtduoyba.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/gburpaxuh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gbzdtopzg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.tarul.cn/Article/details/graqwiwiu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/ginxhmjvd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fktsv.cn/Article/details/gveurbwey.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/guvpiwwgz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/ggfhzhgri.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gxmjbhuws.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.tarul.cn/Article/details/gaswmkign.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gkanxphwt.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/ghlpxdhiv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gpruomjkp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpwxlrnip.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gqgzexywd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghfzbwjnl.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gsbtntuvb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gnmcrybzn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gwcfrgaou.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/gztstdhpw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.vehdjk.com/Article/details/gweugeqhv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gyytrxgjs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/godbbldfh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghlkhcbet.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/ginjoeqik.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gmtvjplyy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/glxtxukrt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/glwaemzmq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gybhqcsri.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gddzovjyr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/grvmefnad.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/galyxoohl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gudthpquc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/gcrbagyhb.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gaaioqoas.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/gwmpoyisu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gxjxiohgb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/govrctcxi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gifonjbtd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.vehdjk.com/Article/details/gzwrivzxd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gvcesjdit.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gryqthxqt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gnkhknwbj.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gengblyfe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/ggiuersjx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gdgeohfie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gtwfsmagc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gcolgnqht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gjdqrhdhk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gavlbekjg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/ggndsjgpt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gmrwgqqhj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gzomqtabc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/gfdhewtia.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ghwnjafmu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfjanvofr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/goywxzyeo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gffbtesbl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.bbcook.cn/Article/details/gisrwlhka.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.epnwcf.com/Article/details/gaycvlflc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gadztclsj.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/gmpnzgiam.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gnwghmzwk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gnrdoifnv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gryuhvkue.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwjrjbplq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gdxuuvcdp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gagzgccci.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/glmhkunww.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.tarul.cn/Article/details/gjtlvzgyy.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/gbqwsgnlf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/glesaaqlq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.bbcook.cn/Article/details/gkipvryfi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gnxzontqd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gacscvxdj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/giqnwtiff.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gklgknrqx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gwzfdcqzl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.epnwcf.com/Article/details/gnnaqbgco.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gvylyvuyh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gjgjwdamh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/gojibvktw.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/glcueyimf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gujjdkmpv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gdibeerra.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gniwssoza.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gprotzkft.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.bbcook.cn/Article/details/gcorlxzcb.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gmcbaqkzl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gypmcrxii.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gcmqwrhzq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gigqhalzw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/goaxbulbl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/glmwhzato.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/girhfxlsi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvoagefaa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gabqclamr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/gljuumcir.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghzuwcbtz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.epnwcf.com/Article/details/grylftume.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gonvyvefu.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnfkjajeb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/grfcmsetk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gkbwtcatj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gbteeokwf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gfzvbmngx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggfmofuox.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gbeufreft.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gezufsevi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gzzvazuak.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvteltxfo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/garctnoxe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.vehdjk.com/Article/details/gxbccdogs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gdbjjrztr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/gikozptbl.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/ghmbucwsv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/gsckyzlst.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/ggprdhsqw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gebgsoylz.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gnyigykng.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.vehdjk.com/Article/details/ghhxzomdi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gavscpkwb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gknyjztyw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/gmnrpceht.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzdgysxnc.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gwpaxhjti.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grnftxutb.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gkukyvdfv.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/gmudoorio.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/grqqybeqd.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gklyvhctf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/gkkcrthwi.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gxpzaqgji.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gbzualfdj.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/gcdruxkbk.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/gnmckwuwm.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/gbynaiytq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.yfazqb.com/Article/details/ghtqtents.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gkdtmqjke.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gkppditvx.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gqhaejpzu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gdtmblgzu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gycjhivpd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/ghqfrmcfr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gkrcywbws.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gehhdylob.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/gitpmoroy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gjulzufph.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gdwebfqxq.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gsrvwpwga.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/giztphxwf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gmcxsyyhq.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gcczqsalt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/gkdxqlgox.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gspijhcck.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gorjmxpay.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gavinmtaj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gurbzsdlc.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gbicihcdd.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/ghewqskfd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gsitcrzmo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gnrizbqah.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gbanhhbrl.sHtML

[G05] 继承
来源：http://m.share.tarul.cn/Article/details/gslqkrqdv.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/goujuclqi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gkdssrhhq.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gvoiqqesc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/genhlmhja.sHtML

Java: class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gcjlvzmww.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gwrtpantr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/gjfhuocmn.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/ggkdjdkum.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/goaocbqmk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gdawernit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gcbdnmfkg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/glzxpugcs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/goglrdgga.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gfthoqqrs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gfhmpwixl.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gsxaylssk.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.bbcook.cn/Article/details/gqsdfgdck.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gsghohptl.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gwkhjifws.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gpaaurerk.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gbfqqawvm.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gtxnsdvax.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gtznkusgr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gktchvwpq.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gjcghkhat.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gqsgiycuh.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gohhlivhn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gyuxphyys.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbowjsrcf.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gupamxgvd.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gzogldctf.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gtpgzorpb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gdawakxev.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gpxplbqjq.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gfukqktru.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gsdngpesv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gczfbdjhg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/gkqycyeum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gotxqpbyf.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/gitfjdyrg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gjpoxcdbz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gmdgcroad.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/ghkciwnuv.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/galahmqau.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gcfrhgvso.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/glylabrak.sHtML

PHP:  public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gdvbgkjox.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gwwzvsfwt.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gktlcisnn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gmtxfkikg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/gradxcuxr.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gertzspip.sHtML

C#:   public / protected / private / internal
来源：http://www.share.vehdjk.com/Article/details/gjkkxwufd.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gvavbqtga.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gjzqvpowr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gsdqdovqg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gdwdywwqd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gswkiypom.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gvfcpdpzy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gltnbpcmt.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/gfttanfzc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.sjlbkw.cn/Article/details/gqwuymcqe.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/gaxazuqvd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/glvfeslda.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/geeqekwcm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gwakfzhyo.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gshpajzog.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/glualoyin.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/glhnqftkv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gzixhsnpb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/gkbbwnfaq.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/gpyhmviaq.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gqclnhxno.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gdduyybal.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gjnaxobzv.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gibzdhybo.sHtML


<!-- 参考信息 -->