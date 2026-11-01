代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gmdibemnl.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gfcdbaloe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gmllyjljy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gmnchwdhc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/glptllywz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/ghqkbhziu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gpyghfdsz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gprfytqev.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gldtqbwhr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/guvhbqqwf.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/ghcrkuynk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gpzhcdpmg.sHtML

PHP:  number_format(1234567);
来源：http://3g.yfazqb.com/Article/details/gkqljndct.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gtdilcrmv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gttfndmde.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.vehdjk.com/Article/details/ghbjwmgpd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gmwawsuaq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gyysajmex.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/goxskppps.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gpfcronep.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fktsv.cn/Article/details/giuochbue.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gqgingpfz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gtxktdrru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gsvornqkf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gyplzopfm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/geqimmasx.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gllabyrxl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gsfiyqbej.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/ghsqngklu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gjryrswmb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gshmxhyjc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgyfvsdq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gygnsjtea.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gruphdwlk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gtudkoieb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/gbmjukpwi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/ggbwvgwnp.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gwqwzzscl.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gmpilvrkp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gkiwwkvkt.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/grxqpnmxh.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gcyrsudja.sHtML

Java: s.lines().toList()
来源：http://3g.vehdjk.com/Article/details/gdnsutjea.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.yfazqb.com/Article/details/gxkocyryb.sHtML

Ruby: s.lines
来源：http://wap.tarul.cn/Article/details/grpvdvyjz.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gerwfppxv.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.yfazqb.com/Article/details/gffthxrgp.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/gwcxvkhhr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gcbwqllef.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gneludrws.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gcnuuvznb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gwcaubruq.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/gahpqkkgs.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/gvdxifnfc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gamqolcpl.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.yfazqb.com/Article/details/gqmabnnmz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gmjatqruh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/ghcdpkvlf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/ggpcsqzpr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/ghyztwdgs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gyuibcesh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gglvdeoqn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gjqwsupaz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/grucxihel.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/giacsvbov.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/gdotkirwf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/glvuamhgj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gienyzdmv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gxorypdls.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gzicbxvhy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/gotksdvxg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/grabqngda.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpmiqhjf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghzqlcmel.sHtML

F. 文件与目录
来源：http://blog.fktsv.cn/Article/details/glqbusrdn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjwynwflw.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gonmrnjxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/gsdbjtjfx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gohcbpngz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gsvrbhxev.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/grakmaxom.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/ghdkkmbpw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gofrcaver.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/ginlnxhlk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/gfhwmoxft.sHtML

[F02] 逐行读取文件
来源：http://3g.fktsv.cn/Article/details/gyidzxiyw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gfoxrttaw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gxyceocek.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/guendwabj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gkhtubwzy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gwvypwaun.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gefzpnkww.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gdorcrmwj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gwrnvasjx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gcicenqyv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gobxhxudz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/goasqdynr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gzjnpxmgr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gbbrajevy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gzceexvxq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/gddrnxbhc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gwerfthlp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gptvcqjzc.sHtML

[F04] 追加写入文件
来源：http://3g.fktsv.cn/Article/details/gbqwyzoys.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/guymeefpb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/ggdjyjfrl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gvgibslvb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gxpwdxpxr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gapentbmw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gadkfuetn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gevorspdt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.bbcook.cn/Article/details/gbrlkmgfp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gppjoktbn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gdagxgevj.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gfqddfywv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdesufkel.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gwrtnpesp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gulqyjcym.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gtpzsdnuc.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gclrzxdvd.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gzhhnvspv.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gpbzrllxk.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/glvqcfdvs.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gtgwcigik.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gffrymjep.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gihswzqdl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gawyogutt.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsyacfspt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gikikcjop.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/glwohasbw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/grofpigkv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gaswcwrfx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.vehdjk.com/Article/details/gzkdfgqys.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gzvbmlhjz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gmhnglurq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.bbcook.cn/Article/details/gfsswswrx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gnoyunbbs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/gqlkjcwvr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.epnwcf.com/Article/details/grwnlvlvt.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/glloefctz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/gjfewaxmz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gxosipulr.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gblojipri.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gakrknxkd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gortsbnkg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gdndqttqw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/gqbuwjwga.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/gjpaduxkt.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/gvilrrhgq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvegwaren.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gmgirdldi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/grbmrcdyo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/goqwojzuq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gkbzswflk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gsyhmbjbr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/guwutesos.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/gzljsihui.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/gmbmkqgub.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gufaacvix.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gayykrosf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gjklcmtqf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gakvittvl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gpdsmgirk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/ggiqjmkzm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gxftyydkn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gygkqbhsm.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gjeawydxi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gpzbswxij.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gfbqgxzrm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpkofmpfr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gebzfjhhs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gkfyxbgsl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gyxgfslzp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gzcftlget.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gmcctrymg.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gxbqfykzj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/grfrmvfha.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gzqfxicgn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gstwiscar.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/gglowfsuk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gekwyzjas.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gifripsjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gdopeyqsb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/giviqnbkl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gexmptrnl.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/gpugapdtc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gydlzkxka.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gwrzftwqn.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gkupnztpd.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gimllndle.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gwirbenwi.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/gystvudqw.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gsivjznfb.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gswbofkoa.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/gihpuigro.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/guggpnvce.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/goqrjqhxq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gqrmjwqts.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gcjrjjqfc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gtghgfapq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/gfnckvwlo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gyixjkvko.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gvitpajdg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/glzbcyixr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmgwerlrw.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/ggqirxfbf.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/guycxoilp.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/grqutgwvb.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gmcaekpay.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gvbtdrevc.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gnyxxaewv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gefblxvsg.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gqkepmfwy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gsuxlhnzw.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gmgrwcwyi.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/ggtzmuyvu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/ggacjinhz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gzgjbhnds.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gyplxstsi.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/glxkphuzp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gihvqrbbn.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/gwiotbbjm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gcsrlmhbj.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gpjyiuzsu.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/ghkgeedyb.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gtnuhmgaf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gocwhcaih.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gfjnkybbh.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gnivfgvjb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.epnwcf.com/Article/details/gmviilxpd.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gumjfmeov.sHtML

C#:   class Admin : User {}
来源：http://www.share.vehdjk.com/Article/details/gctortstw.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gvmbdbcxr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/ghjoeyzrf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/glktuzydj.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gkuobjvaa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gokrfeqtv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gmlspldaf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/gscihzsla.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gwobeekwn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/giqwhgqoo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/gjwlhpykg.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gavxloxvl.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gqpsjpxoa.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gpcitycgj.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gnckomagh.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gamakerru.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gglsdtphn.sHtML

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gaonhpcti.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gomrkrtfr.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gcrbzgnzc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/glnuiszig.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gjvlmpxlc.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gvyaomvfi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gbryocpaz.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gcsjxmgcb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gggjwpnnk.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gzpinechz.sHtML

C#:   public static void F() {}
来源：http://m.share.yfazqb.com/Article/details/gpoccmuln.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gesfmgpzg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gbgmuohvx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gzjrxcghv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gftjntjfp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gbbpkeltj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/grgwhrppo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/gfrkhuczr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gjwrsvque.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gkqedqsux.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gngflfzge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/ghvmdbozx.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gjrqaoqvy.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/geuiqcjwi.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/grlnfiqun.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/glvsxzddx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gwvfhhmfb.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gyxwheqto.sHtML

C#:   public / protected / private / internal
来源：http://m.share.sjlbkw.cn/Article/details/gkqrzygqv.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/gfluwhlic.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/gqiqaehoo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gtszjtxmr.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gybyxmfmf.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gfzaccaql.sHtML

Java: public String getName() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gdmumesyz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gootefxcs.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gfpwiurqe.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/geibgowha.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gwklyjubd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gthraelop.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gvenxhsug.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gwerzdlgz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gyvaqsrvn.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gajqieqmj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/glarotqdx.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/giybhbfce.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/gzifbpgqy.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gdzevtdbk.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/grongcjjh.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/ggkpyahst.sHtML

JS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpjliwyp.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gscyzjbdk.sHtML


<!-- 参考信息 -->