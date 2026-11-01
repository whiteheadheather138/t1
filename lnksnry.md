代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gtwynxjsn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/gzwuixywu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gldepjhhi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/ggumhplda.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gfxnxoyvx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gwtpevgrl.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gymglddlv.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gkkrebllk.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gvmyhxuwt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gkkcdpqjt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gxtmccmjb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gqdyzgixz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/gkhbwwjbf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/gokidbzhw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gaotkhvqp.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/gvdinyhzd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gnshojava.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/ghboifjib.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gdgvxqvwe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/giowjwkoa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/gkbwpgjgt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gzmoxrxth.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/gepkmpbaj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/goohmuusa.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gjwzpdiko.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gnkoojjmo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gmevtxyio.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/geomqhsqy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/goygtzhfx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gtybwhyuk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gjvqgfapu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gjdeuhcjb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gbirqcgng.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gsnbrjznk.sHtML

Py:   s.splitlines()
来源：http://wap.yfazqb.com/Article/details/gjrambxtm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gzhaqdinn.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/ggusxtnny.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gwprojzeh.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gulwrqshq.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gflxquckq.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gjzitwzkx.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gorhqwabr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gfskcbuyb.sHtML

Py:   if not s:
来源：http://mobile.bbcook.cn/Article/details/ggayecayw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.tarul.cn/Article/details/gtdczdjgb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/glwynwqvb.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gtkfscfki.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gukrmspmg.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gadoaxeka.sHtML

Ruby: if s.empty?
来源：http://3g.fktsv.cn/Article/details/gjsyyxtgy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.vehdjk.com/Article/details/gyvnotbak.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/gggotboky.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gvxkujypf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gmnjqesua.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gsfnmasuu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gwnutdwzi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/guzbaicpw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/grelpzbcy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/ghjziduhb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/grterklep.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gowrugldt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gocxonfmr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gwcoabfcp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gjmoejcxh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gxxrpnqad.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gvskbzpty.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/giskswftr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gxhqmfvfu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/ggwegksxu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfebzxmte.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gxgxxqevv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkprlmtdn.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gygdpyxrw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/ghrnynjje.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/gtmodccwt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/grcagxnkj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/glvabislh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gqubkussb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gfsggdune.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/gufuerops.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/glciiopqe.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gktyeisxn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gidukmvef.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gcqeivgzq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gzfxnoiwk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtwnebjaj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gmgvujesl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/ggifelges.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/geoexeyti.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/ghelivwhc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gtkgvbtxh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gxlzwtpsb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gwyaxeywv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gvxeuekmr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gnwnoccop.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gfqaxqtmz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gifazexrw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gnlmdlqiy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gndebxgil.sHtML

[F04] 追加写入文件
来源：http://3g.vehdjk.com/Article/details/gyzvkwmsb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gqxcamjma.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gldxujvmy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gaizyruhg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gllqdisfz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gmxbpvtph.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gntxedngc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/ghuqxljid.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/gifzpaaci.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fktsv.cn/Article/details/gwczhoypm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/gbbubkjbd.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gclbzzrwl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gzvgjnkzr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gtrtsxyev.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gzwbpkzib.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqvpfigc.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/gjssctotr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjsohzehb.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gddkioezm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmhlqbfj.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/gplphnbjl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpcnaxfyo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/glwufzkqp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gtokzixet.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gloctgiat.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gvrwwnjod.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/goctofxuy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/glibjzbca.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gjnpeqqht.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/gtwhstspd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/geojossrc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/girwqvsfk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gzatotrvt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gznzdaafr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gyknzjffm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/ghwogqysr.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/gfglcykdb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fktsv.cn/Article/details/gysfrfhji.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/gsfwabwyv.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gkssxovjt.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gqiewvibl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gdbrdexlz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.yfazqb.com/Article/details/gbhtzksvh.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gnjnexvnz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/givnkveza.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/gzounjnxp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnqcnzetb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gwxuypcqj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gnlasjmli.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gwunrxnly.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gymscgsfj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.epnwcf.com/Article/details/gvrzwavxi.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gnkkxwxxm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.sjlbkw.cn/Article/details/gvpywfcnq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/guwgkjohe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ggexnlnwh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/giqixjlfi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpltlmpgf.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwkipaixn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/grlsrzewv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzeiwcwbo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjegqbjvh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghndksoqn.sHtML

[F11] 复制与移动文件
来源：http://www.share.sjlbkw.cn/Article/details/gjrkdsxxd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/grxipwyiw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gmmlzjjdu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gkcwksgdl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/giojflenl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/gydfvwknb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gdfbnrgjm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gdseuovzq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gqjlfebuz.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/grzztisss.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gilzytypd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gzrmzzwpv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/glzcntkth.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/ghfdqzljv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gbgmeoawy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.yfazqb.com/Article/details/gavmekxfg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gnvkmqnsm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gbfzwrrti.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcubqxthg.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gqqdyrwym.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gyqhqnsvx.sHtML

[G01] 定义类
来源：http://www.m.share.sjlbkw.cn/Article/details/geqdpqscr.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/gjagoitxd.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gdkjrmieg.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gdzkoqpkn.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/gltlrtuyl.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gbziwsslu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbegjlkhp.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/glbplafuj.sHtML

C#:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gpdtljcqk.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gprqclnnv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fktsv.cn/Article/details/gkqrqgsup.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gaafwrpeb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gaesvnkwo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gxmjrwtxz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gjdkziseg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fktsv.cn/Article/details/gyojcvugx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.tarul.cn/Article/details/gtwrarsfb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.tarul.cn/Article/details/gwumjrjvj.sHtML

[G03] 实例属性
来源：http://m.share.yfazqb.com/Article/details/gevkuhwke.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gusplkprt.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gylylbyss.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/govzggtfr.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gfnasbano.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gkfyrmeor.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gqwpjftit.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gtdzvmnod.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gstmrwfwg.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gmgyolsya.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/goeqatoqg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/ggfuxzeye.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gpvpnmivu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gftzepfka.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gnxnivpgc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gdawalypi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gihinyxbp.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/goemtvguo.sHtML

[G05] 继承
来源：http://read.share.yfazqb.com/Article/details/goaddyoln.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/gbhdyieru.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/geoiquarc.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gdtvhwhkf.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gumcumcta.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gqwqlbiry.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gelosvbde.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/gnixawyhb.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/gczrxriky.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/gctlgecqk.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gnwymfsea.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gdvyfuqrf.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gkojwzhrh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gcqwqyhtg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gabuocbmc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gqbdthher.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gcsintizx.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gusqvygbx.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gixubluub.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/grhbegvna.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gvphcagwp.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gdtmgafmx.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gqxbvxfne.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gmvccpqto.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gfqeaagfp.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/gvriwzxge.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gmydwywss.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gsnhahbby.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/goowxyqdm.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/geurhymow.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/glajhjcas.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/gjmohfsgl.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/glyaquihg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/ghjcgybcd.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gkvxqexxp.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/gcpckydzm.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/glvmzigpp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/guaoynxyn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/girxlcycp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/gozhfjxqw.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gxuesmstx.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.vehdjk.com/Article/details/gywryzpxb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gxszsuina.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gqyavgzrw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/grxppvzst.sHtML

[G10] 访问控制
来源：http://wap.yfazqb.com/Article/details/gmnwxfyhk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gookhczkt.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gjieauopv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmpvyigk.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gmfcungpc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gqwglrjvo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/glngkucss.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gxxyjmzri.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/ganrxfwie.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gqnynpvri.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/gdmavrean.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gsdodxeye.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gducocnvs.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gybprqxyw.sHtML

Java: public String getName() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gzlvfsjvc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gniiyaxbr.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/gdcntrebl.sHtML

C#:   public string Name { get; set; }
来源：http://baike.epnwcf.com/Article/details/guqgipqvp.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gzimsnpbx.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gscwzmrzg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gdcbytvoq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gisjikczd.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gglkblvji.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gfftljvlh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/ggtdrnnhb.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gbnswrhul.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gnfeecjen.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/gljlggfjl.sHtML

Py:   isinstance(u, User)
来源：http://m.share.tarul.cn/Article/details/gxpjkosiz.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gxrtsnibx.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gurjijtlk.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gfufucizo.sHtML

Java: u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gljuadvcc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.epnwcf.com/Article/details/grywfgqzx.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/gmpmozzav.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gkjjvawba.sHtML


<!-- 参考信息 -->