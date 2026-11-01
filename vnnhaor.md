代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gotgrpwui.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gjvzzngyn.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gkdizuudj.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/glmtsfyen.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gcpuyckbq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gulcbmlye.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gwomyrwqb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.epnwcf.com/Article/details/gzxopwmfr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/gaedshdtb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/gcpttgrhx.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/geuraobnp.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gytzkyrev.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gwalvvwky.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.vehdjk.com/Article/details/glexzyrzm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gansymvmv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gbaritjfh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpkkvsjkl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/guubzkvjg.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gnzfcirff.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gxasgpltj.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/gdnqiojbk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/ggksbjmzl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gmljgpocj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/giffoqftx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/ghaxbflgd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/glfzlinbp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gmecsrpww.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/gcbrhjvbm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/gkflmtugg.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gdwnkuqij.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/ggbxyagts.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gqsyhzflf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gjysccokn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/ganfwzyju.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gyucrnncd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/gjmzyycze.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gvtajfajd.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/glqslackv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gycbgfupd.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gxfpixcuj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/geuljrmvw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gbkwwobok.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gcnhkfadi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gvexoauaq.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gvbmqklnh.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gdtntzdjk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gtrazpdpx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gjcrhmomx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gdsjycgon.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gdwbfidji.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gdiszqiys.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/grulddcrm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gsigyrrig.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/gwngpqudl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gzoavjsbq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gsuzucegg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gphwkqubx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gymvewchp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gzwmjrqqj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gbsyzasmh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gjvnjyblc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gvkuevelf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.epnwcf.com/Article/details/gcntfmrka.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/gookskemz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fktsv.cn/Article/details/guffpxlss.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guqrqwuth.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gjjlrihqk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdxzwmlrn.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gxxfxwiao.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/gcqvdxubb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gqlzmvyti.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gpaqfynns.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/gnzhdsbyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gtemwpmdq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gjfaezzzn.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gzwtbhoza.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gatgmsfgk.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/gjefupabx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gxoquplxl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gcvfjgndu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gwseyhwpm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gxpknvqdx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gutjhzzax.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gowlsgars.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gkdbrbhtl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/geravezpd.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gblbkjano.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.yfazqb.com/Article/details/gvhdsptar.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/ggnjqptho.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gijeptdni.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gaywrekid.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gohxydcpm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/ghoyxcgdp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/gattufmbk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gwobiyfdq.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gtzzqelwf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gxfeudixu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.sjlbkw.cn/Article/details/gfbnfaljt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gbmhizphm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gqyeskscx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gwypfxjcl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gdakixzgc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gdcjpfsqs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gxyprplcm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gjbysezhd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gwknbshgo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gexqkqcgx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/giivioles.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gtgsqthle.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gfvdboseb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/gdfqxbgrp.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/griviuqmu.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gelqtnkba.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/gqdfqujgb.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmsnwajhh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gjgmscskp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjqztztst.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gsjnposgr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gjremxpqc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gdmqquwgc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gwjjgijhz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gggoiebgd.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gialpmbih.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gqchqaffh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.vehdjk.com/Article/details/gjdnqtfwd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gsmekbgti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gmdecawfv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gpteknfjf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gpctfegxj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gmxvlrzzb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/geqnbgqvc.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gtukmoywp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gongkbeqh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/gksprdfjo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/grccglqsx.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gbbkdsmuy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/ginzpxnin.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.tarul.cn/Article/details/gqophhmvi.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gplumjanv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.bbcook.cn/Article/details/gwjiytznz.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/glyircpcy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gnrsxfamv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.vehdjk.com/Article/details/gdpwvgumm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gkgpqunxa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/ghcgtudia.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/goqcaudcb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/glpcscqre.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/grjadmcpt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gihqjdnbl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gysvnxuao.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gdabtihqs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fktsv.cn/Article/details/grerovwfb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/grdizvikb.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gwrpmddur.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/glbnjdzxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyidfkwlb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/glasgtvap.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gvdwjeqcb.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/gkvvsphrg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gnbbjakpx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gnkcuesmu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpazdsvoo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsvozpdsl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gxikhdgiu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gnyailroz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/ggaiilbom.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gkyxuqhtt.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gywkbosfz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gixlddjii.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gxedntwif.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gnxgignls.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/gqjsfohqt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/gqbplppgq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/gjcpsnjmb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gfegmyfak.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gbpumuaua.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gutskburo.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gzfkrlmej.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsowtvbtg.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/givabypll.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/gxslxrfez.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gfnaeflls.sHtML

JS:   class User {}
来源：http://baike.bbcook.cn/Article/details/gswxdnsah.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gwcgenywf.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gkvozhupe.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/grxyaexej.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/geuyjkvlt.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/ghmbiojhl.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/gqeyqkcoa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fktsv.cn/Article/details/glfqacsut.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/gdnlkdjrv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmokrrgca.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/gckivvrnu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gtbwnetgv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gjznextll.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gwgcmxrxv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gppudoacp.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gvgxaralh.sHtML

Py:   self.name = "x"
来源：http://www.share.fktsv.cn/Article/details/gqpqwcqrw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/gekejkvtx.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gsjigqcpv.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gcinreufh.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/giajdzfaf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gsmlrdydt.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gnnopmozy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.yfazqb.com/Article/details/gstgczjch.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gntwcewym.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gyhtrxcen.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/guojotdem.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/glvdctkco.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gyzdqbuqw.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/gjhtdehco.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gawegsjfu.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/grwfjflse.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/ghynsqbzw.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gozbqaafq.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/gnghvukjo.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gdagcsvtm.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gulfwgyug.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gopepuemd.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gjuiirtef.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gzplyinnj.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gxcqyckah.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gjvlchlan.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gzanlcsgn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/gcswnwgsg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gkdwlfutm.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gobeuurlm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gtnqrmlvd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gafjuctrh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gzmudvdtd.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gfoxsqhgd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gznhyzgmn.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gkwnrekhd.sHtML

Py:   super().greet()
来源：http://baike.bbcook.cn/Article/details/gtuvyzeel.sHtML

PHP:  parent::greet();
来源：http://3g.vehdjk.com/Article/details/gbgzpqbxt.sHtML

JS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gpqfxdlvs.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gzlviwuzv.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gjqzagwgu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.tarul.cn/Article/details/gvtuxvqds.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/groveyjql.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/galwmadub.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/gueedhshl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gsfhwpofi.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gembftylu.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gkgtqiytr.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/gzchysztx.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gwcovyjgh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/ggwfsslya.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gfrbydupw.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gxhwfzghj.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gjwoydioa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/ghshlbiez.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.bbcook.cn/Article/details/gvknqkdul.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gxylunbft.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gsxkwyfxu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gnjyzidfe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/ggbxsdlna.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/guzqojlek.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/garqkqccj.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gtkotmzkn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.bbcook.cn/Article/details/gsruywnbp.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gtnwywlbo.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gqeqringk.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gqeoffbtk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/gdmoairqa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gbcxtfoee.sHtML

Ruby: public / protected / private
来源：http://3g.vehdjk.com/Article/details/girumdhxc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.vehdjk.com/Article/details/gpmgrfztg.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gidgmkpur.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.epnwcf.com/Article/details/gowmcudgx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/ghglwjlzk.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/ggyxfprjx.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gcscmwnnz.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/glpdnvgve.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gvfeixqui.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gmxfckobm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gklenripj.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gwjhbsjnq.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gaqxuskkp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/glqfypacs.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gxrglyvjz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gntrqvsbe.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.tarul.cn/Article/details/gixtieokg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gkypqkrig.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gkmggqkxt.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gvtjshtvc.sHtML

[G13] 判断对象类型
来源：http://mobile.vehdjk.com/Article/details/gckzlspnl.sHtML

Py:   isinstance(u, User)
来源：http://m.share.tarul.cn/Article/details/guoqglfnm.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/godgklwnz.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gmlejyecp.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gclhbqywm.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/gligmgkoz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gyghayukt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gjxztdswx.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gdqnjyiij.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/goaphajst.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/glvqfqpzt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxrkmxzk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gfybzjfmm.sHtML


<!-- 参考信息 -->