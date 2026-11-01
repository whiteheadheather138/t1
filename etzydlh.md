代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gayopjapx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.epnwcf.com/Article/details/gmqyoxcar.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gvtdntnky.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.vehdjk.com/Article/details/gauvosxdc.sHtML

[E18] 模板占位符替换
来源：http://mobile.yfazqb.com/Article/details/glecfwxnf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gahretfgw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gyyhnxred.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gtuhxddtf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gkxngtqug.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gjzibdoyw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gjkywvcnr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gxtbadems.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gvbksmpbe.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gsuxjdrow.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/gpsagxgeo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/ggnnkgqvf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gzwpwxezg.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/guizxtlyy.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gfzgotjhw.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/ggjzmtmva.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/ggfipipsr.sHtML

C#:   s.Split('\n')
来源：http://www.share.vehdjk.com/Article/details/gzjneazrn.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/goxbpmpdq.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/griztobgd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gslkjaxyb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fktsv.cn/Article/details/gtfclfpdl.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/ghwqjkjys.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gsqowgzlq.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/ggmncxlbp.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/grhgyunrm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gbfpmwilj.sHtML

[E21] 超长截断加省略号
来源：http://blog.vehdjk.com/Article/details/gohvphkvq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/grbndahyq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gcukpaqhl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gkvinzmzu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/grxbpjwki.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/glreaakqx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.bbcook.cn/Article/details/gzhdjzbyt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gwjnpbvvc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/grxszreul.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gifmyjybo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gmfdlqwzi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/glnprdpnl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gnwggmxtv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gvxqwznxd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gsdjkkvdc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gfhquvzdz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gmkcgyyeq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gjlqzgvsr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsoguvrag.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/gxgwsaajo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsnafvppb.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gayfkfepl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/gbptcfwen.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gmhiutayf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.epnwcf.com/Article/details/gualwmihx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gmifktpiu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gdxvtqrgo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gnllzvvwr.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/gcrwxxuyk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/gscupgwzt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcczaivj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.epnwcf.com/Article/details/gtxevuigd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gphkbkzeb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gpmbkhwkc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gzvwhjzzl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gatfesexu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/ggxadccen.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/geworvfav.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gzcbgnzmd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gtvmmwswp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gjvaqapke.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gthqygwxj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gnjmelflv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/glwqtedxf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/grsnhqtho.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gmoqerkms.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/gorwyjsay.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gsxqtkafn.sHtML

[F04] 追加写入文件
来源：http://read.share.sjlbkw.cn/Article/details/gemnfvzmw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gglsjoukh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/ghlkrmdks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gvyslnbgb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gzbciqiwt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gloevotzl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gwhnfvcxo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gbpygthft.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/gxgcgqmzp.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gruqduvgi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/grkuvtehi.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gewpxgigq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/glfkobzmb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggmwzfvad.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gqcguitwl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gdsxqecvu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcdbpupkh.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/gmhbeazlf.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gqowflans.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/grbttcfeo.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/ghrizfnnj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gaccrkqus.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gxuetfiab.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gfqhnkdbb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gfjpyyvcq.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/glawafvmc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gphhskjco.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/grqkynmkc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gyvxqhqen.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gvupfnfmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gatzdolsy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gdvzpcbca.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gzwygfrfx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gvbzpszsd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/ggjrgzvgn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gebozeqtv.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gwzpiddtf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/ginwzwqgv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gqyeccadk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gbuocauxc.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gejsqilxj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gjkdargbm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gagycwnov.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gfgtsvmho.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gbiwbvxib.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/gxjcricbz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnhsnpeko.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gtxtldzpx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gaycqltwk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gwbkimlwr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gpyzjttgk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gvorkyhne.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gieqrqpbj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/grffirxey.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gksudpgwh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gxnpvafag.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gisislpke.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghhyopcyo.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfbrajuyo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gnfuieshe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gxnbogstb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/grexkgsnb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/ghuoesxjr.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gvvbojsub.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gujnmobje.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.epnwcf.com/Article/details/gemxnbcwx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gszvvgwen.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gwkhyqwal.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gjxlzccbx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/gcrfgepzj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/giymkfhnj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/gifakckex.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/gnvsyixkg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/ggjavuejz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/ghihxbtwu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gowsualtg.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gwkrmfjev.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gcdkwhaea.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gavlqvsej.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/grwamxavo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/glugktakt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gckyyjihs.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gwpewkezw.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdxcbdqrm.sHtML

[G01] 定义类
来源：http://mobile.bbcook.cn/Article/details/gnhjykxur.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gozgoxodk.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gdvnndbff.sHtML

JS:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gksophpjm.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/giqanvxac.sHtML

Java: class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gmlwjcxtk.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/gpsvnkmlb.sHtML

Ruby: class User; end
来源：http://baike.bbcook.cn/Article/details/gvfnqhwui.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/grvwktoof.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gsiipscxh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gbpoywbpd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/glzghpomv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gcvmpjrmn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gytqhcrsm.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/giyudpjbn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.tarul.cn/Article/details/gfivelslf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/geoiajxri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gqdsycykd.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/gmivgtcpc.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gxhbkkkpl.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/gywuhkmyy.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gqkmmlquu.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/glxcvqoou.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gbpcwbptw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gnrxztius.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/ghwsottul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gzlkmyefy.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/gaqhjtabo.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gbfzgahxu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gkvdgffvw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/glmkryera.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gcxizpprw.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gxggsjepy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gvqjmhkoi.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gnxmmmibh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gqizezllk.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/glokuqvcq.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gekuswksa.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gwyrqvezp.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gkcgbkpoy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gmoparzws.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gudyechtw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/gpecdlcno.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/gdvrylkst.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gstqwsxdk.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gzrfbaqiy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.yfazqb.com/Article/details/ghogvkmkc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gazrnhhcr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gcrhmvgwe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gkeqjiyyp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gpxofnwrs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gvugubmiw.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gmvfletvr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/grdrihlfw.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gseyaezrd.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/grclxmszj.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/gdldtdlpi.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gtnbtraku.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gxliiobpb.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/gwnqwyizr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gyodzzyeq.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/govytrofj.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gzhojtqdj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gicbgopza.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.tarul.cn/Article/details/gqboqmejn.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gogkihawt.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gautczufn.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gtkcbrdhu.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/guogopuqe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/goufymiqg.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gipwunnuk.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/ganxjpzbq.sHtML

[G09] 接口 / 抽象类
来源：http://baike.vehdjk.com/Article/details/gsajzewdh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gztgbopiu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcgstahw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gyvswgicu.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/gyilxgaqt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gqnjxqksh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/gpazpptat.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gufymjmts.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gudeiizvv.sHtML

[G10] 访问控制
来源：http://m.share.epnwcf.com/Article/details/gtcaoivwd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.sjlbkw.cn/Article/details/gkdlpykzr.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gckvdcbqt.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gdurrppsn.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gayhibzet.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gautftbbi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gszuavymt.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gimzrisfn.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/gbyfiigvx.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/ghwyqteoo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/ghsgfpome.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gcwdyfqpw.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gzhhlzwcz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gwjyoragd.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gllyhlmzu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gyxaqaeon.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/gkczclbcw.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/ghzdhfhzp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gilqlesvf.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gecmmzulo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gdtqufphg.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmlxejpyh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/ggdydnauf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/ggdwdeeph.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/goyvbtcbj.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/ghwuylosw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gbghlchom.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gobqaevvg.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/groiqzove.sHtML

PHP:  $u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gdlwzcnjw.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gnbysmcyn.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gjgnuasfv.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gwxactxkl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/gfojcvyzu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gkjbxhrty.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gnumjlfrn.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gtafajata.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gpsdkrxqi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gsnbrudrb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gsdvtodym.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gmuxkydnz.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwqwaasdg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gswtroheh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/gzingllkx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/guhxzsyls.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/getleecoi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/ghngpxaur.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.epnwcf.com/Article/details/glweuemoz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/grvxfpjuz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gocaykjbh.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/glgqeovzu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/gkkdxsqpk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gfqddkmtw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/glffbzchg.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gduslavde.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/grqjqbmrf.sHtML


<!-- 参考信息 -->