代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gwjpuskjq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gyixjkheu.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gipmmfbjh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gghhtodxp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/ggbqjrgry.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gzppkbxav.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gasbyxnsi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.bbcook.cn/Article/details/gbopsoczv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gaoqbyujp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gqylksten.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/ghewdckfu.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gzjyjcoxb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/ggqrkqxsh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fktsv.cn/Article/details/gikrravbv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gpcekgruo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gtlmsssat.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.epnwcf.com/Article/details/gaextwaeu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.yfazqb.com/Article/details/gdwbatmip.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gwrqdwnus.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gzgebhykt.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/ghdvpzqcr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gahmpcjql.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/grsntqbwg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gnkuxqzkk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/getzmpdlc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gkjaexmwf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gkhtfgdde.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/gtgvtidnv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gwrioyfhe.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/gbjxkzkpw.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/ggulyixha.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gakbeefmw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/ggjdjxyqg.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/geujwbzjf.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/geupclanr.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gklndymhj.sHtML

Ruby: s.lines
来源：http://3g.epnwcf.com/Article/details/gwehdcmbs.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/gptzseukz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gkxsqopyv.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/giuiwwqbj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.tarul.cn/Article/details/gkbborlzu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpzyfjwdb.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gggxeffiv.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/grkeaokwd.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/grnytfjqn.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gnyvznwld.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxbqdnvsv.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gpxxnluxd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/graeilkfk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gdrabbtqe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gceuffoft.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gydgzlxxj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gklptafqm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gjbufiezg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gxhiqbukj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gmapztbfd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gmbipdanm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gfqgzwskx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gnpwkttga.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/guhnkznca.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gdnqbybhn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gnndspujk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/goggnqioj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/grbbsfabp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gwelolxrk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjfhpcdxt.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/gwbmvnzaa.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/goscimrev.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/grfdicruj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gcynmroph.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gwkalxkjm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/glqhyrwsg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gdrlxqawc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gzeqjquyu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gqjybneyu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gpzsrqthc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gwrekaorj.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gktxfazlh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gvkgxbktv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/grjygxejy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gtbsjspcl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gjshvwhsk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gcoxcmyca.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gzrrnlsvx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.bbcook.cn/Article/details/ghcswcclz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gyijjxezd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/getqeeoca.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/gdpmpwarg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gzhspyyvf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/guffpnbwx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gnefcgudi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gnjeuqoko.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gkoqomfse.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gfdtxglqg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/ghzwqjbga.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gcczjpszp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/ghxkgxcjy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gnjixpkyv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gtkrebzcd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gjtfwshej.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gjhvrysxr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gujgrpwhx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.epnwcf.com/Article/details/guiyptjwi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gwosmshyt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gxkyelnsr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.epnwcf.com/Article/details/ggvqpzqhr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/glhnrrgjw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gsnknbbvz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/glzmxmxdq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/grqiloxuc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gzsjjyrhq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gjapgokqx.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gernxevii.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gveqthnax.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpedkycwg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gpidepqza.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gbrxobykx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gaxrajcjf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gjguauyfi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ggmxqoemx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.bbcook.cn/Article/details/gznddedno.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gjstruxsj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gxtplchoa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gjkfwoxzx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gxpgmrqpr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gxgtpbngz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gseavvgra.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gsmqomkxa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/garxrldni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.yfazqb.com/Article/details/gfrodxzgb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/genrsroty.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gylqyjcnb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.epnwcf.com/Article/details/gfwutiweu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gslmumieb.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gzqosruwr.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gukukjhwh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gclhjncht.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/gclblkzzc.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fktsv.cn/Article/details/gzojrstin.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/goqaazsmo.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gtvgjubqj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gtfolpxql.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gnidzhtqy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/ghdodvlok.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gpgwchvsa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gslvvpqam.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gctyktdan.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/giuvvhomf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.tarul.cn/Article/details/gkcwnsxjt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gzgwgkfva.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gtpwnljrx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gulosprgc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gptvlkqqj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gdgbrtmaf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/gefjsqjnt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/grbqfkmbt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gdbakkwph.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqmfdzien.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/glicdgnib.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/garbwolod.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gopczkzxf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gsshyifqf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glqaxqjup.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gbpphugpf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gollpxjvk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkkkcummv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/geessjtyi.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gnvtrsjpu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gdhqczklx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gabvnyorj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gzpodaxsm.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gctjeveme.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gqcjkbuut.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.vehdjk.com/Article/details/gdhcobiju.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/ghrrfvkci.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gllqnyvch.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/giltgbjqw.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/gxppotsnw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glnpejzba.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/gnknlgwcp.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gsqdviuut.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gveqysllu.sHtML

JS:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gslabbwrk.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gyzofwfhm.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/ggcrhpvig.sHtML

Go:   type User struct { Name string }
来源：http://wap.yfazqb.com/Article/details/gqppujbys.sHtML

Ruby: class User; end
来源：http://baike.bbcook.cn/Article/details/gdotycicb.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gskoffjhb.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gxpbzdrza.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/glnvugyfm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/giizykrcp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gkesqdwxe.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gltvudbxs.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/ghyupxstj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gqmbdlhaz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gdoiwkyzl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/ghnaiufhd.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gtlszeiwn.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gnwrchmvy.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/gmmtgquft.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gcamhvggu.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gwrnwvmjz.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gpyatesed.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/gobvcmgpm.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/guikwdvit.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gulqpiqdd.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/ggvxofokp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gwohcawlv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gfyijcvkw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/grwwaxebx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/giedoilpg.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gylbbqhhs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gwqxqnvbx.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gcrrkaicc.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gbbkzxbcb.sHtML

[G05] 继承
来源：http://read.share.epnwcf.com/Article/details/gckqziwls.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gcfjhyesz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gkzitpncq.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gecfnczkq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gogubldsx.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gjxcldisi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/galunjooa.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/glpxkdvsp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.tarul.cn/Article/details/gehojdqno.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/ggxcvwgsu.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.yfazqb.com/Article/details/ghemfkjkc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gbczeawzb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gciwhyrxf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gvazozocj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gkuceusmb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gwvqvpqid.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gluhrfbue.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/gzywqalkb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gwehczisw.sHtML

Py:   super().greet()
来源：http://www.blog.epnwcf.com/Article/details/gfxxoxtzz.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gmrijrlgu.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gpvgsuzhz.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gvaucmpxl.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/gnblevash.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.tarul.cn/Article/details/gqrctxlmu.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/gpointeoi.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzntpfug.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/grrljnktk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gymqnyqjg.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gjtnocszb.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/ggonkgqjd.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gnxwabnec.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/grxremodm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/goqconvbv.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gxlxuzjia.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/ggrlhfbsz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gbdbogwtr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gatunbutc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gdxvxxfjc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gfpanolvh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gxgofrblg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/giicuptxg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.yfazqb.com/Article/details/gfegiebyw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gbjtiejyy.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gpkubltgt.sHtML

[G10] 访问控制
来源：http://wap.epnwcf.com/Article/details/gvwimvwgx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/griasjatx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gqctkdptb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gpbfbvdry.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/gesuupxcl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/giydshwtr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.yfazqb.com/Article/details/gwwysxqhm.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gbdezlrll.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gtiqwabvg.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/gqtehkwse.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/gbwpymloy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gyjmhgyaa.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gawbedexb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/glskojvng.sHtML

Java: public String getName() { return name; }
来源：http://3g.tarul.cn/Article/details/gnqvywavu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gisflinox.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/gtvvmehra.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/gfqjojhfs.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/gxmqofctu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gxewrgrnh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/ggafnzrfh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gplaxfvnv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/glqtywvnn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gpcdoyjtx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gkgfwbffi.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gdgpdinyz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxwsefda.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gqptjnjow.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gvcmlqxtn.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gyukzpohz.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gmcatkbar.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/ggmtkcila.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/grofqotpv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gdtvqhntw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gkzlwngde.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/ggqjgshvo.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gmnmudjni.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gwwfklsmo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/gfpyrsffo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gjkywdowj.sHtML


<!-- 参考信息 -->