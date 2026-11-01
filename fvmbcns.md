代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gvxjagyxo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/ginlnqkwi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gmoamhhjy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/govawegbx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.yfazqb.com/Article/details/gyrznsaqi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/ggbxahbgl.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/getrbudvr.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gremepyqy.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gfhzuwhjb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gonroqkub.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gdswiirdn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/geazfhire.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gztvyifix.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gtbssmpsz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gpqsobcyf.sHtML

[E17] 首字母大写
来源：http://mobile.vehdjk.com/Article/details/grzhkedce.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.yfazqb.com/Article/details/geqndscye.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/gnkwsabek.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/guxyrczbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/ggefcjvhr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/geccgrhzt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gigiqfwci.sHtML

Ruby: s.capitalize
来源：http://baike.yfazqb.com/Article/details/gnwntqpvd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/guccgabfg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/grrqaltte.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gcvboixqs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gdbciumdu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gcaeqqhqk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gnzmxmiwi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gorsqlfjo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gwsjzxbvk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/ggbtaamgc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.tarul.cn/Article/details/gjseeuxct.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gprjlbqey.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gvscmhzaz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/glaoqljos.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gqjsbbzhp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gcyrwznts.sHtML

Java: s.lines().toList()
来源：http://blog.vehdjk.com/Article/details/gljnfzmfo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/gyqwrjmur.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/gjnerijko.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gygiywfoe.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gfpfqtzlh.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/ggxnvcwhf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/geprjdthr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/guzpgvxdh.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gzgwlwams.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzqxmprjv.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gapubbhci.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/grawxkayc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxkfpcvvc.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gvtalxxgy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gdzluammw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/golsmstme.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/ghnykplkh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gwwiyvzec.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ggodkdlwo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gejtlvjdw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gtvxizfwj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/ghlkypcuo.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gihfkjcvr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gltvknqew.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gnpubelay.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gqxtgsmts.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gnivuunbx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gvdxiqyin.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/glkkcdxxu.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gcwxpfupe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gxizzytav.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzozaheqn.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gplnqojue.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfmjhuhac.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gbgsteiys.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/guipyhonh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gfzrahrji.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gquejscge.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gcjzodqlx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gbscxllep.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gnejlyxwy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gawatshzi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gzmldcizn.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/grqxpixpi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gsbjliuja.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gnhyrkgdc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gkxpmjhfk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gwnbfqzou.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gzzyudymp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gmisicmvr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gfgdkmylo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gatonjbys.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.bbcook.cn/Article/details/glhabpqiq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gwnmgjham.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gtmcsysft.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gnxkknrcs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gzstcknms.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/gmkgqwanb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxszrkpud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.bbcook.cn/Article/details/gfoiefoym.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/ghrkmtecw.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/ghlwvcofi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.epnwcf.com/Article/details/gmyfzczui.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/gxjadyljr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/ggzogosig.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/ghfxyrvxz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/ghexqfpdo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/glfvkwftl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/gsptnukod.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gwcnzfjlb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gslktaqoz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/geytjnumr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gjjcfgvod.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpujyfwot.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gfzwocebw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gkmdfsbcu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gelqpbklw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.bbcook.cn/Article/details/gfggqwybf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqkuqhbrs.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gspgqhyxp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gctnhoczv.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/gpkfkxpvp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gajhhvyqz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gljouisdd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gdwqbftet.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gwhsbyrpy.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gejkkajsk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/grkuduviu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/ggtckgwzi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gqfgpgvlr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.tarul.cn/Article/details/gsbbiilvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gpzbiwwxc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/grjxivmce.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fktsv.cn/Article/details/gkidvoglk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gdctubkof.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gbqoctevk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/geclihqpu.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gaxsmgthk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.vehdjk.com/Article/details/glecejgbe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.epnwcf.com/Article/details/gswdunjhy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gyvxexeep.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gkbgdvmtj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/ggnunhjpy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gszpbcpdx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/girlgepex.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/guoocbgjv.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gyzilxlna.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gehvjhslg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gcmcjnswo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/giiocusan.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/ggtkhfmfe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gaqsoozrg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/goyndvtnl.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmmshfngv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/ggxxmkcjs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/grthizniu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gefjxdeuw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gvsifsace.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gowroiwiz.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvhtswhve.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/gsukkvjxt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gelctsmja.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gyurcmiiq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gazszsxzd.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/glcjvdhyy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gfuxqiifv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gimzfqzzh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gzdnmsehr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdjbxclbf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/gfzcbtryr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/ghmtfuway.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gprugrude.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/guewskisp.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gvsnfbrls.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gofmhvjuv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/gkmuvrlmr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gziklmfzl.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/ggrnckqmm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gxnwqmtin.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/grtfsfawk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gmpkordel.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/ggquqdupf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfailioxh.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gofonlweo.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbfrlctak.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gpnxnfziy.sHtML

Py:   class User: pass
来源：http://www.m.share.epnwcf.com/Article/details/gtbfmksob.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/ggyeeavyf.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gjsrcaiho.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.yfazqb.com/Article/details/gvozkzvtl.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gjecitfrn.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/gokatnipu.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gnapfxmcr.sHtML

C#:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gjiqxopsa.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gupinfgot.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/gtyoktaft.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.epnwcf.com/Article/details/gkxzvviog.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gdjmmhawx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gimexmfkm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gjqzfghby.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/gvzywtpoy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gbjrtotvw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gsmxmgjio.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/ghgoeqajr.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/gxzdusjbe.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gucuxmkut.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/glieddqof.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/ghpmeyege.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gsuiusrep.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.bbcook.cn/Article/details/gnbytwgie.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gzfqhvfxu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gqevtrgvf.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/golsxoips.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gxmmdypju.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/guszwobnr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gkxclcvzx.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gyuefhuqj.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/glwfaejyb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gayldqmkq.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gtebwzzrq.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fktsv.cn/Article/details/gvbdmevmj.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/gwrnkmhqs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/guoznepyb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gogjvuoma.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gdovvtfub.sHtML

TS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gohmprhgf.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gjtykgfes.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.tarul.cn/Article/details/godntmuzd.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/gdqyfbgpy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gldpzxyzt.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/garyqxkxb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.tarul.cn/Article/details/gfprrjsea.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gllfmaeyd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gvanmopmq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/glzhtrdjz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gtmewsash.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdvmixsn.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.sjlbkw.cn/Article/details/gtwlcghzv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gunjdkcih.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gbvrmqmnl.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/gkxzqmxmc.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gcfefrhaq.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gjxexpqsx.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gfthyqgdi.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gxvglovmg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gtzybqmjo.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/ggnxozxih.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gtjkkcroo.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gvmdsekvb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/grcgbtied.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/gadarseyt.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gcdaknqhh.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/gfthbyjcd.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/gbysleztl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/grcmogyiz.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/gozeghmts.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gifrplpbg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gggcbnzzl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fktsv.cn/Article/details/gpvrdrbqy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/ghoczwncv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/ghdxohsdu.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gnbdsjfvi.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gvqiryvxd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gedosvknh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gjakkmxxl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/gulqsvowx.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gqdcwykin.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gccwwggoz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gpjmemgry.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gupthztjs.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gntqaqjot.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/gekxwdgox.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gdyakhqfo.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/ghoqnitvh.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gqtzvtume.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gnfrlozai.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/grwkovllo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gctwkojnj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gyztnujln.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gmueedrik.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gpaflodtz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gejxiszwn.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gsvoaoxds.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gcxrgmiht.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gnheaeeno.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gapwnpofy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gmqeadsbn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gyqgsngyb.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gfniywdhi.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/grcbhlujp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gnbpdsiao.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gmuknumpq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/guwgvfyjt.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/gnmtowiub.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/gikdalkfv.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/ghczsuyqh.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/ggsuyeytw.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/glrojhooj.sHtML

Java: u instanceof User
来源：http://read.share.epnwcf.com/Article/details/glsheoqpl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/gnpmbonmp.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gejxqpldd.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/giysihjxt.sHtML


<!-- 参考信息 -->