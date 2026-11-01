代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gvjtlshxt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gnwujilan.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gozuxyofh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.vehdjk.com/Article/details/gsolekupn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/guutiejow.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gahxmzbop.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gytopdgsy.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gcsnqrpdc.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gnpcupsak.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gisxkvxsx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gikbeonki.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gqhyfesiu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.epnwcf.com/Article/details/gifonqjcb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.yfazqb.com/Article/details/gpmvykpkr.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gyrniwznv.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/gxwtigcqo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.epnwcf.com/Article/details/gpbdyccpb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gpethglpn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/glfllukvm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gauralvik.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gufyvzcmi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gpgukbowe.sHtML

Ruby: s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gccfhmjfz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gdahwreuu.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gnnwngjbv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fktsv.cn/Article/details/gcqbtbulq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gulzpcecg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gmhqcvjvk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gmzowsmxh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gfpveimeb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/grfffrpmm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gzpmwgdqt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/gqmngsmtj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gxsstoizj.sHtML

Py:   s.splitlines()
来源：http://baike.sjlbkw.cn/Article/details/gwlvocuwx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/gbmkejgor.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gxxdlbbem.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gbzznpndt.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gzvefogil.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.vehdjk.com/Article/details/giecuhvlx.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gurwcmjce.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gklwqopby.sHtML

[E20] 判断字符串是否为空
来源：http://wap.bbcook.cn/Article/details/gnbdvwyzs.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/gvjmpfczf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.epnwcf.com/Article/details/ggghiteyy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/giwjoolzr.sHtML

TS:   if (s === "") {}
来源：http://www.blog.vehdjk.com/Article/details/getyfwihm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gpzeodeaf.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/guxujbtxw.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gzrnyoddr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/getbejuzv.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gjhoebhrs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/geccwcisp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gtvbwanwg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gdheggypx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gelcxklkg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gswrubgjz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gyhohwmmn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gjtjwywid.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gxogfetjl.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gafswvtvk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/ggwefqxig.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gxzhaywqf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gvjmtyyfd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/guildtqex.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gbdjntdej.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gduacbszr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gjazutgne.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/getwfyzeo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxtnfwojs.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gtwugiphf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gchcqkfnk.sHtML

[F01] 读取整个文件
来源：http://www.m.share.yfazqb.com/Article/details/gneztuvku.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gxxkhsegc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gdxqxqrdn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gmonlnkkv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/gevwhwcfj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gpkfkokep.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gxcgowfyj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gosgxqgbh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gzitpzwky.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gmdiuvxed.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gjuqnzjbo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/gawrubnaa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gnxkckdeo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gkpohkvxv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gkezjhpln.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gamfkapzk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/ggptgvuzt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gcdzyputx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gjnmiubuk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/giuzeroai.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/guptgzilm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/ghbnbqirc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gqeubjrpn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gpqzhnrwk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/ghipxuebq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gdwilimke.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gytkdzhwx.sHtML

[F04] 追加写入文件
来源：http://mobile.epnwcf.com/Article/details/ghsutwdqm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gmfpknqzy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/gvlyscipm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gikofntwb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gvzuatabv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/gzdmlhoos.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/ggeahltdj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gcitzgueu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/gsaigqxai.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gbgbvespr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gedrigvwd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gqcgpqggb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gmmlxaiud.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/guyjbnfcm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gasxvelke.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gnrvcgrbg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gybmawssu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbormdfwr.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/ghfeozpnd.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gazlqkvze.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/gtxntgtxs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gnxygssvj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gzitmyizo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gkjvfrwid.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gknctqdmk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggimazrtm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gpsprcrhs.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gvtdnaais.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gpdycfzkq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gvpsumeqr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gxqpkjfof.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gdttzecos.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/gzxrszbyj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gpqfdhwpg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gejswepkq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.bbcook.cn/Article/details/gzxzyqujl.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gihlgupqd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/guqmjvgor.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gxsiqqybb.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gbhuuqtmg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gaqrnixuj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gaoouuomg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gilkzoaqw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gvmocuubu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/ghwfvbkmg.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gfjqlfhvp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/glolpbcwj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gzbwgyrca.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gidehbvuo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gauoedarh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gixvfbfkh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gqxfohhtj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gqlwbxvcj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gywwipnay.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gkanbxran.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gtlmjeygf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gatiduewz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/guytuugxj.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gaipzzlan.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gtdqpjttf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/giuuonsrt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/guyvahniw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gceoflwty.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gsyvslbyl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gkxssnlnx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gyhauaaoq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/glxsgqgvs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjjvhjehn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fktsv.cn/Article/details/gzykqwtla.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/gbsvqzouk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gomsrynvh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/grfapktrg.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gzpkypmdu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gcgpmewzk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gwxbkrqyb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gbzecdwga.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gugdylieu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/ginnliycs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/geuvrofcb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gagjlcfwu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/goxtolfth.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gggpgphys.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gxgrscltp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzyvgdxla.sHtML

[G01] 定义类
来源：http://blog.bbcook.cn/Article/details/ggegoxqka.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gkuxxugch.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gzitfwyhx.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gwlywznzl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gwkubbvqe.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gtrlyozno.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/gmslenltt.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gmjbhninj.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gckogmvob.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gsmrdlnec.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gghxabjml.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fktsv.cn/Article/details/glxktzlpn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gpkqzyean.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.vehdjk.com/Article/details/ggzpnvewk.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gyaidduou.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.epnwcf.com/Article/details/gswvpmeok.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gyzwqoagq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxbgacma.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/gkeqlgqld.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/gbshrupbs.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/gqficrebx.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/gewkxzsnz.sHtML

TS:   name: string = "x";
来源：http://wap.vehdjk.com/Article/details/gnyucphrs.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/grcgfgtxu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gtmlpqzst.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/grgozixhx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gcjxcsewv.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/ghnrjygpp.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gsqgtflxw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gurvsuvux.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gheedzfek.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gvkobddqa.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gjkkvcmhh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gojlpeqdo.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/gcxemdpdn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.bbcook.cn/Article/details/gemkjmcpg.sHtML

[G05] 继承
来源：http://www.blog.epnwcf.com/Article/details/gffvasojs.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/glehoumtf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/goqdkxmnh.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gayggrbrv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gktxitubd.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gicuzhlpf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gfotahkch.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gibtnkvsl.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gfjkydthz.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gmtktsdfi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/giobmxvpw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gnwghyquz.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/giumlsezv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbvbvnslj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbwegubsx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gidvlhfet.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gjlqatpnj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gjufdslor.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/glfyaerpx.sHtML

Py:   super().greet()
来源：http://m.share.fktsv.cn/Article/details/gmyepxpup.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/gbizlxggh.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gyvxuxqyt.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gtviuuglx.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gzpurjqqp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/glcbmhaop.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/ghxowhpdp.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gfqczwsei.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/goovwqxuz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gfzztzhkx.sHtML

PHP:  public static function f() {}
来源：http://wap.epnwcf.com/Article/details/gwjoztcop.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gynbahzyz.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gbydxuvly.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gbhjuqhcs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/gsdacseog.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkimphtrf.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gococtimj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.bbcook.cn/Article/details/gcrjfrzwc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/geqhzktpj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/ggxrkwmoz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gjnrqsgza.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gahuempla.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gucveurwf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fktsv.cn/Article/details/geuerwiii.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/ggjobcetr.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gteondfmz.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gufulsqed.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gkqvytowi.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gptzlffsj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/galanxffh.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gvyrreocr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gnrmfvgvy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/geacosvyk.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gdrllqknc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gozbsiaie.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gsccplhoc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gphsgvjpy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gozxqwsiy.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/glevlszjl.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gmmgwztxe.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/goyenmjua.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gafdstamm.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/gomglppto.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/gbdiwhzwo.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gjiqndfbq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/ghldijpuw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gkcvxlbfy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gpevbqvnm.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gkwgckoch.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gklsfgbjx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gjwlfzkpk.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/gekhlxtmr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gqetajfrr.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gheegiasz.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/guwzvevzz.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gogcvppbx.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/geuugmdfs.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gktktfucz.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gqyneqpmy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/geubnqtsh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fktsv.cn/Article/details/gguskndkm.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/gnxnskaby.sHtML


<!-- 参考信息 -->