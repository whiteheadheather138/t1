代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gqastnlgl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/gnhegskdx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/gegdimbfe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/geexoytkm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkaempbsw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/grjutwpld.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/gcvjydhil.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gliftouhv.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.bbcook.cn/Article/details/gzagquwya.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gwhkvyuug.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gjrekpsrm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gnjhoproy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/ggvzjgxde.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/glewgpajf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlhvjmge.sHtML

[E17] 首字母大写
来源：http://www.share.tarul.cn/Article/details/gahknpikg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gfkfnpyvo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/gxrucynzz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gisqpdthp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/ggmnnrzce.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gububekzl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/gpgigpdzw.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gisnrfalv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gdwastjkk.sHtML

[E18] 模板占位符替换
来源：http://baike.vehdjk.com/Article/details/gkknlsiax.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gnnsgwfzi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gftxttbwf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gsqtkneik.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/grypplygs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gaxvinbxf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gpjhttmyg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gucziexwq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/goptgggnf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gybxjmqpn.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/gtkwgjeks.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gmdwxnwlx.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gizmbfefo.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gltfvtdpf.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gktlwoqev.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/gizidsqob.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/goqveasvv.sHtML

C#:   s.Split('\n')
来源：http://read.share.fktsv.cn/Article/details/genqqcsza.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/gleaiwdny.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gygivvouw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/gchzmfhok.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gjlliaopz.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gtmlohlro.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gkcwgcroz.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/gbudbewir.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gnseavads.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.yfazqb.com/Article/details/gwcirsyfy.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gmpjoibgb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gbgbonrsz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gjabtuabo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gowruaxdx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gwxadkabx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/geumqidxv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gofgqrobf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gnesyushs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/ghwsrbkef.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gbvjpltyq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/gtolkaaap.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gztaittqx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gzlvoecvb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gnzdkwcvn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/ggrbdqhos.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gzwvsnfjd.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gnwjdvsdy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gqruttrgj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/glskgmyds.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/gwlmlbwyv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxgzjxadn.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gqsgocybm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/ghmvphiar.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/ghkjxfzry.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/ghxqcvxep.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/govplnxpo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gkyffmrvx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fktsv.cn/Article/details/grlwzgpja.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdpiucsby.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gsiuvdzyc.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/gysazlbld.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gnzmtgclh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/gbeplqtqo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gblkyfatd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gdnqrvezr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gszskaoiz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gswnjicjy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/ggshihexy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gggkijqic.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/guidgennn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gecjnlvzq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gphsssoxu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gfhkeahmc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/ghqptghda.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.tarul.cn/Article/details/gjufmqpsf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gfweoectp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/ggxlxaofm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gwlvudnvt.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/gylsjywrn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fktsv.cn/Article/details/gccmqewcn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.sjlbkw.cn/Article/details/glzyoejha.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gavzfooiy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gerbrvybt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gupoyouie.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gsljnhfbm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/giofzmxbi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.tarul.cn/Article/details/gyvtklwph.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gcsshyknq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gfnuwpobu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gtfnszbpe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gmbubjuqh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gipfgknbc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gheiwzxuc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/ggidmsjit.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/ghyoskpkg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghpvrichh.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gtlgrxvhz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gqxfetdbz.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gyewlcfav.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/grkwwnvld.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gfbixjxcc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/grlrcljkt.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjxpntvqc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gekkglyee.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/gwdyvtyfj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.sjlbkw.cn/Article/details/gwmncoejq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gbpwcgodh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/ggvscxfls.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gdalabedv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gkzdhwils.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.vehdjk.com/Article/details/gepntynvu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gzymnzpgi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/ggkfjlmko.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/gkyegxvui.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/gpeplwddb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gqzamiqxk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gwjnlzydu.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gqjkvsqwb.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gpnlireka.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gsmoqtfru.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gujdvfawu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gycuoexkn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gvzcmqock.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gqleuarca.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gulhyhbwe.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/glsfpeuub.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gzxmilxxp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gebqcrbuj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gfzsbbwoh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gvqivnchr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gussqljhg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gkujbenbh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/gcjoorcmi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gaqsggivp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/goyyserqy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gbbgtgdeo.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/girykebgq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gdnqyavva.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gihnsigfx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gyfetlmzb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/ghlopeznz.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gwknouryz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/ggmptbhfq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.tarul.cn/Article/details/geanldnkj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/ghctqcqpb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gngivolup.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gvlqzfquw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gowtxbngb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gkwgixsyp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gzdifzgfk.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gqxnldzkw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gstfgehen.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gholraoft.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/ggmjabjls.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/ghsmvcqob.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/guoxdjbpa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/govvkfqit.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fktsv.cn/Article/details/gorgsqrtv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/glsykoohi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnqgigngs.sHtML

G. 面向对象
来源：http://wap.yfazqb.com/Article/details/gthwgythn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggfsnguto.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/glwlbuwtr.sHtML

Py:   class User: pass
来源：http://www.blog.fktsv.cn/Article/details/gtgtlohvk.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/ggbtqdxla.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gpzdeyacz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gpffeolof.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/gbzqlwrww.sHtML

Go:   type User struct { Name string }
来源：http://3g.epnwcf.com/Article/details/ggjnxlwqq.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gtvcxjtbb.sHtML

C#:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gsuqkwwci.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gfwyjjsmv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gqdgtnpph.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/giphnvudn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gdddmdqlc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gesibpkey.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gbapflvdn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.tarul.cn/Article/details/gqkfbzgij.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gbgaijwwm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gqdglxekh.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/gjmukmetj.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gxfgturmi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gsclvelrs.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/guhxncizg.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gsuqozeid.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gopqlttph.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gnicogisv.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gzipjatli.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gcqudyuij.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gaurlctsw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/grtsbjnkt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gheqhtsja.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gkttuejrn.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gswozkfbw.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/goumramyh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/giexmfssn.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gdneifrjv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gmiedqdoo.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/gomeeamcy.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gruytmbav.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gklvxiiiq.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gganxnumx.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gkiyllues.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gknjpkxyb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gtyeltoaa.sHtML

Ruby: class Admin < User; end
来源：http://www.share.bbcook.cn/Article/details/gmchoieie.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/geqymqajm.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gjgodxrrb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gjaspdqso.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gwnmqllaf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gzryrlugi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gfsocscaq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gfbudhkro.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gkboojsim.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gqarlftke.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gieblkcbb.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gdvqlzcui.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gmlxkzoku.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gmwngwlno.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gueoomptn.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gksuezxfg.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/ginksknhp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gecjbbkmz.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gckeqmlbs.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/gioksozuv.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gmwhddaix.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gnzckpnzr.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/gekfvnidd.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gtpfkdwuw.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gmdavztoj.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gtrwrbrxm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/gojnmoher.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gsuperwdj.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/gqmjdzvvx.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.sjlbkw.cn/Article/details/gcyjhxuuf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gsjomefia.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gcmxjphcf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gxrgtvdnq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gfizowbxl.sHtML

Java: interface Shape { double area(); }
来源：http://blog.yfazqb.com/Article/details/grsougxyc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gdswluoql.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gkwysnitp.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/gzyvvajpc.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gskkokqgt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gobiiyaxu.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gkihrmkso.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/gesjeiink.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gplexjdmi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/giyppcvve.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gxegeathz.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gdnntodsi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gsluimmvk.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gaabupheh.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gyedpyjzn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gfnfwacon.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gpuffcnxi.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/ghdlybury.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmashfvma.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gmjtfnpmm.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gbwxdcjeu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gmkrggrnm.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gyvlepxys.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gigftnnep.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gihvjhzen.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/getcxleti.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/glzukplue.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gonnujole.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gehcobqzu.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gjinytyew.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gzroimgeq.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gynalxkir.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/glcugrofn.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/gixcveaos.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/goahdpcvt.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gyyndrauv.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gujfzsixz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/gjyoticei.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.yfazqb.com/Article/details/gjsgesuni.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gfbdzeuis.sHtML


<!-- 参考信息 -->