代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gfcowkfpw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gzuaqgebk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.tarul.cn/Article/details/gksaojnff.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/gjwkitpyz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gfqzafdib.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gvlnbdhmv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/grirbehth.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.bbcook.cn/Article/details/gyubnpqei.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gsrfoehjg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gqngmvtzh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.bbcook.cn/Article/details/gwoswaebc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gnccdgeng.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqfffgfvc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/gnadjglrt.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/gynxinxte.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gbwgyoakx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/guwxojjqp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gfftbeyip.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gouvxtqls.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gtfqkeyjz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gbsnpjaia.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/grjbmxtsf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gctclbouu.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gyyqdbvkc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.epnwcf.com/Article/details/gjgypgowi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.yfazqb.com/Article/details/ghkpmldcd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gofcgbxqt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gljijucuw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.bbcook.cn/Article/details/gyybyhkzr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gjqhntbqh.sHtML

Ruby: s.capitalize
来源：http://baike.yfazqb.com/Article/details/gtqrhmtym.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gpprkalig.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/glosagpfh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gjxrkynlx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/ggznnstia.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gvefibrub.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/ghwtthuyn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gxgyujrzz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/ggpembkke.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gfpemvykt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/geevxoxtx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/ggeseiqht.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/gilsscxgf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/geymogump.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/guwuhsciv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/grvbgncqh.sHtML

Java: s.lines().toList()
来源：http://3g.bbcook.cn/Article/details/gtibosdgw.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/gkzyemonv.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gnrrnznnk.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/glbimepqf.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gokbsiros.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gsszgalrk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/gdboypqnc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gkynyfmtv.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gksmzwcxb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gtpziyjna.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gubiehaiy.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/giojbjtqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gsncilqac.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/glqcsvbcf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/gzlcqeuwb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gzowzobok.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gtxqznopm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gvifdaqdf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gowtlcohw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/glmmpfelg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gqylvavdd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gffbnhcgk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/guvaqrtfo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/gbftnsxlj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gsfxxjsdp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/glfsdvukf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gvisaapwb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/goismzizt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gbkhcfqbb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.yfazqb.com/Article/details/gsnzwyhfd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.yfazqb.com/Article/details/ggaqprjmy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glbdwnblq.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/glbbajykg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gaoddivab.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gfgsnbkyi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.sjlbkw.cn/Article/details/gnzpqlewg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsigbjzhi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.tarul.cn/Article/details/ghnxgrhee.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gqjrtylhh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/guyybtyga.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gfoqettez.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/gopvttrcu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gtnlvvbkg.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gqxhynkbc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/glnmuiasy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/ghlvxsozb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gpbntdywa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/glgshgyhk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gbvezmmer.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gqlutznkv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gsxsxrlro.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gqquqzkar.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fktsv.cn/Article/details/gbdqpqnao.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/gxgcmfclz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gbfdcrenf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gqaabbnzo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gxcszyoco.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.vehdjk.com/Article/details/gfofbbmgu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gghjxodvb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gdjxvijex.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gfuyecmdl.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gedlwrgen.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gsilotnrx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gurbnnspi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gyobkzmyb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/glkqjdlen.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/ganbzrfzz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gklonkxwi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gdqmxsbcv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gntkblkpm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fktsv.cn/Article/details/gkvqmfozd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/gxfltokzu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsaoagqnj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwykahbly.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gfxcogopt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gjnqbbdye.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gbzgprnac.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmsmodoko.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjezzvycc.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gmrryfrbp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmxorqvab.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gaxmcpsgj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnauiprde.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gephssepg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/govxahmoj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpxqqbboi.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/glubybuhh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gfgmqxufj.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gcqiudlds.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gsgcuxaux.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gyuitmcqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/galkuwzev.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/ghggwjhum.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/guyihgepa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/giszduqkt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gexpzrubp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/geiavpfxz.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gjzoggxky.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/ghzeugppn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/gckqiptcy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gppdbppuk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/govpieshk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gfmzymtal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.epnwcf.com/Article/details/gljflyuzc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/gvpzjpoig.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/gokzhpglg.sHtML

[F09] 获取文件大小
来源：http://blog.sjlbkw.cn/Article/details/grzezjmxr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gllawxagd.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gzliiuyuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/ggsjnykze.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gepkghxwj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/guglbgcmb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gchrmrbxc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gfbiubpxi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/ggnbcivuy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/gkmohjtxl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gdrtgsswg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gkfuuegvs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gmzrhqnef.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gofwwcpda.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gjyufjruc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxhjffpvj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/geynuxebd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/glxjaboui.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gmtgclgye.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gfjzybfgl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gtcpgecyk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/ganwwwiom.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gafcfxswe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gcrxxsypp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.yfazqb.com/Article/details/glccyoicc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsjcfrrse.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.tarul.cn/Article/details/gxpsowwxa.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gtganvnlv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gnguqxunq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gupfihmgk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gqejbgndk.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/gkqjbmrln.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gatdmdarl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.sjlbkw.cn/Article/details/gkpmacxhl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/gjchduhnq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/gzlfhhvkz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glglvxwiy.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/gatuukacq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gotoezhfo.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/glnlisaad.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gtudsvvmy.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gjagsmpsp.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/gjnmbgnjy.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/gtaapbuab.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/ggzicimpk.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gvmraulhs.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/goxwwbfvn.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gphsictrr.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/glzvvsjbz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gukpfslut.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqixlcncq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gxkbrskbs.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/guynpoowh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/grgfxlvhp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/grofvprrf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/grxvhghsd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gaqmvnqqs.sHtML

[G03] 实例属性
来源：http://blog.yfazqb.com/Article/details/gmzqxikae.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gcszosugl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gphtihafh.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gcvrhvwzd.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/ggmnhzopq.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/ggetqzsyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gqngucolu.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/grcedsavv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/gijcfaitu.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gzhnktbqb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gkjmlfccq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gxwabcjjq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gycmukfyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gkarwylgn.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gborsslmz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gbqybcdce.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gxodjgdsf.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/ghmhcgjhk.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gwpabrbdg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsrksgjn.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/grwhrfbon.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gbwtzgxge.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gwvcpdfjt.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gddvtsznj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gurjittwt.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gjjesimfy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gpxrpuqbe.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gcykefevz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gcfddbmik.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gfskefgcq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtunmtzty.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gsaariiaz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gcntoptgd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gtjklyjbk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gjvlcodnp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gqxobyyxl.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/gzjzzqghv.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gsulcaiyn.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gpwfryoho.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/ghngjbbal.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gwjkpjrvi.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gjimocqlh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gocruajdq.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/gnguftvtu.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gqunniaep.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/grwfmarfa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/govfzzxmh.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/getqkteca.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gjxkbrmpp.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/gajsknwbm.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gqlyulccq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gbhkdynme.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/giqiomajn.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/gfhjxhpya.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/ggzlsqzyb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gzetbwblp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/ggqgumpnl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gxhqrzaby.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/ggsdyilvc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/grbysosdg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gsyxhgctg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gxbapqfdm.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gjyzvzyjt.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gatenqazw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.bbcook.cn/Article/details/gjrgbsarj.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gszzdqfuh.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmplcsru.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gytimxxou.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gespducmb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.tarul.cn/Article/details/gbuuxpipb.sHtML

Ruby: public / protected / private
来源：http://m.share.tarul.cn/Article/details/gsvygvvza.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gqotqnruc.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gffczgzaz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gxgiipmgx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gxtrizrmi.sHtML

JS:   get name() { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gmdzyjabp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gocosbfgf.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gcmwgalxb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gwhielubi.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gaudjwyvh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.sjlbkw.cn/Article/details/gioahliqp.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/ggcpjioul.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gndtnjeze.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gudvpnjqr.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvhywfwsu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/guizfhrak.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gtqiswnbw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gpjlwlypz.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gbixontey.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/glkujmose.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/gpgcsapdt.sHtML


<!-- 参考信息 -->