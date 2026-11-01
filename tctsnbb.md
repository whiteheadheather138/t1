代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gdumylrig.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/gewrcukip.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gyweizprz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.yfazqb.com/Article/details/gjgkmlrgp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gdfluxpfq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/glfwijcho.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gfufooedd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/glmvxjjqr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gdugiponx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/gminsazpb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/ggtrmhusg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.bbcook.cn/Article/details/gizmeoobg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gbdmddkmf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/gykyckpxf.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gowtwxwcz.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gbzjzgcsc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/ggopqniqc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gycmullqd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/ggosqqigr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gptgplkci.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gvzakofsv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gjngyobdn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.epnwcf.com/Article/details/gtozysjxi.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gyasghrjk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gflghglqn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/gsvyozujp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/glkjwsvyo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gksaolygv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gwywenrwi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gkppzxvzo.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gqsnrdcec.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/gpnyynqpp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/glebatzwb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/gudlmtcmh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/gffbuyrcv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gnkztjwbu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/giwaeikfg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gbnumfqum.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/gndgbwfeu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/grhuvfrwn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gcedstyim.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gnyhysukf.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/goyvznylv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gisjilaru.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gwwzzbjmd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gpjcjfhqf.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gaihcqrsu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/ggjhmbebn.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gdszceurh.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gchbtydbr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/grxsxtfyo.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gfmysbdft.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.sjlbkw.cn/Article/details/gpysovfhn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gddwrmwah.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gaoqdgjxy.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gdmsjolzj.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/glqszvarn.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gsktfgujf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gryuesjub.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gzqetfazm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/gsjmprihl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/ghrnrxukb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/goijubmev.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gmbxsjuzg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/givdlhxtm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/gaabbxcnh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gpvzwrckl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gohyrntax.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/genxjqcgm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gxsgkdoqv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gebzwvoig.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gfconqwhm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gjvukudfe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/gzetwxhbl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gbuwumuvw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/ggzhimztf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/getmxnbeo.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gduzgoymg.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gqmomnklh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqknfynid.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gffzjhryb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/guotapgvm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gopcoxaio.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gbadxjxmn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/grvscaazk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gqhwlfluk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gaezbnctm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gvkjjlsxc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gxmpkkiji.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkxiidnw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gsjutxdhz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/ghqpwsrua.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gskjyiaop.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdsvrsieq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/goxsykutx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gfkwqdtdu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gksepvzkc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gejsnwhwk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/ghvjatgmd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.yfazqb.com/Article/details/gpsuuqgsq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gihfbdllh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gkfbjzqdx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gzaupwstv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gqlcgdtye.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/gcltqoqqy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gilnnhuxa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gfaxupipq.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gbznfkncx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gqtqdxpsv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gkkcuazqf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gpuxgalrc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gwfgjkimi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbnytxub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gawjcomfc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/grpodxsll.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gvkyyiizp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.vehdjk.com/Article/details/grvbxodmk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gxeovzpsf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/guoztpjar.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzrozkkuo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpnaisnny.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gmcgtigca.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/gxbnpdead.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.epnwcf.com/Article/details/gdrrkizuu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gycqcgslo.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/gthpakrsl.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gyzgawhhy.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gwvpvapnu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gitveqoic.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/grmlxxgip.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gyluahant.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/giyuekhdu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gvsbiasvz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gtamcheuv.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gajsrlxhu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gsirccfrg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gkrlhtoaz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/grcijayqz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gjhwpcdpz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/gtkobldsi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gyweurgxr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gycgavgvw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/giotthfwx.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/gpewyghtz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/ggpqjkkeq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gbcbrwdro.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gctajcrai.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gvcnrnlws.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gtlyjeytf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gcbvbzpxt.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gsawzbkfw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gjcfcjepa.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gjshzwxbh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqibdxjci.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/grgqoekpt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gweaiefag.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gzodvhunf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/galfyjoin.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.tarul.cn/Article/details/gmmkczybp.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gyidcyika.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/gvvlzbmcz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/gjsstfmsj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gfqipfoyt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gsnmiebzo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gttcptmng.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gojvqqnml.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gtllangea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gktcxebhp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ghcmtyfai.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gaergcdog.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/ghfiamfet.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/ggbtauxaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/goygxwxqq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gblspfsgs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/guxtrwpds.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gcohwevhi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.epnwcf.com/Article/details/gftgzvowv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/ghsuodgim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gkwcxwegy.sHtML

[F12] CSV 读写
来源：http://read.share.vehdjk.com/Article/details/ghkfpcmvp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gtcegsdgn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/gwxunsrrp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/gcbhdnhva.sHtML

TS:   // 同上
来源：http://blog.tarul.cn/Article/details/gsyjcxbds.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/giigvswlc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gzzwlixlq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.vehdjk.com/Article/details/gqqzfegxk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gfhkchtqu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gushpmkrd.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gftmgqdzd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmnxuevcb.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/guhnzychg.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gttpsrsxk.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gmygiwkio.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/graolpnpf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.epnwcf.com/Article/details/gvlwiiicn.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/gcdmsddmi.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fktsv.cn/Article/details/guefsjdii.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/guhstbhxk.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gqideqenu.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gavmldbmz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gvmvbiedx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gqqwircyf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gonfppxkb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gxpfnjlfa.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gskwbbblj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/gsjnayyss.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gnflrrfmt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/glqzybfap.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/glqyncfcj.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gkjcqgslo.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gsnyxvmmk.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gdmghxfpm.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gwdndyqco.sHtML

Java: private String name;
来源：http://wap.bbcook.cn/Article/details/gvmyjsmwr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.vehdjk.com/Article/details/gkbpetegr.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gchwcjocp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gzpiwglia.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gjvvvklvp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gafgpnndc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gpulteohr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gfcjkiagm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gvhimtcls.sHtML

Java: String greet() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbgvcalea.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gntsttcbt.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gwtvxnlon.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gzcormqyi.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gmvefnawf.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/ghpuklyro.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/glwwapoif.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gehwdyuci.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gfmvlwrol.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/ggezqscnp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/gwvpsbmvt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gvpyexera.sHtML

C#:   class Admin : User {}
来源：http://wap.vehdjk.com/Article/details/gfgxxodcn.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gvxqztznn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gzgirzsmh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gohxfwfhw.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gesjbcmej.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/guztletaz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goszesbqr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.bbcook.cn/Article/details/gyuhqwelm.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gveigkyjg.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/gscbwxxim.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gnbgcuypj.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/gfhdtxkqk.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gcsquzbsw.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gkamwfhtr.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gsfkeknmi.sHtML

Java: super.greet();
来源：http://wap.tarul.cn/Article/details/gnnottrtq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/grvrowcrn.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gpfwagavy.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gtvcmzutb.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gwljbbppj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gkiyuwgyo.sHtML

PHP:  public static function f() {}
来源：http://www.blog.yfazqb.com/Article/details/gpsqwmlja.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gmmvqtsdo.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gexscomrw.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/gkvzoftaa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/gkjmsjafo.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/gfyumitlv.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gnoebznut.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gvyfvthxc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gfuurwlng.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gpyvamams.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gjdrvhwxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.tarul.cn/Article/details/ggdlknfpo.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gneiiqraj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/grzjzlxau.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gdiazkkjg.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/gbipoyjdh.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gjnocbfly.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.yfazqb.com/Article/details/gurmtzfnn.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gucfveifn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.vehdjk.com/Article/details/gaxxnuflg.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gdvtdaaaa.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.bbcook.cn/Article/details/gvzcxdkyi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gnjnxfzzc.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gunroduqr.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gfbthbpmx.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/grxafsttz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/guerlfgfj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gvyioonlo.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gwtkvxzhu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gdqhxppoe.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gbtvldwpo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gvvnpoywz.sHtML

Ruby: attr_accessor :name
来源：http://mobile.bbcook.cn/Article/details/ghhvxhhdi.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gbgzkijka.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gobvzutkh.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gtrpcormu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gqmpbkjwq.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gvqaakgqp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/grejzigzw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gglbrmadk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gulhlieqt.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gvqpfnrsw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gboalxfcu.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/glspvomvq.sHtML


<!-- 参考信息 -->