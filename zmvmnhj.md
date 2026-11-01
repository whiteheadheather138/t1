代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/geqodutzh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gwzgfecxi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gqhbemesf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/gtfhhyhgz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.tarul.cn/Article/details/gmlvhxjjv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.tarul.cn/Article/details/gcpipzruh.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gcgsnewsw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gbffvgzhn.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gwhaadqxm.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gcvefikww.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/gyzmozdum.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/genammqhc.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gwdrqhmua.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gsahkrguc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gcsolrqcr.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/gdwpkuqhw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/gnatnwzlp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gfvoxavim.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/gfyyspfnf.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gasfporqp.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gyqjxxydy.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/gzdhtqvkp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/gwbygwcrg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/gahjcswsc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/gugemvklt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gaozigzld.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gabggfyga.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gavgueqjx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gxygtngwg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/geuodblwl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gzxufwosw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gvodqldlb.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaszprcf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gkewekroq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gdizcayis.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkwkcrud.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gtsklrcds.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gdovdxjbo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gknxfijtw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gwdwqwhww.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gpogtgqdd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsjesuwtu.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gpsyidabw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcbbfdgsi.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuiwanzg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.bbcook.cn/Article/details/gbdsaxecr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gcwaexrbz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gmprwlgxx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gdaoxcnvy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gqpklisop.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/ggihczbmy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxgysouim.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.tarul.cn/Article/details/gixkbigjt.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/glcfioibl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gazobdjhb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/grocjsnug.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gobzzvrar.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gbjeqysua.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gkcmkpcxb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.epnwcf.com/Article/details/glujmxmul.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gcnkkxbhp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/ghmiuedwu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gdwxvdpeg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/gtydhiwhs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gikejlfsz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/goqilrubs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gbwejuzuc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/grxoypgto.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gktyfibmf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gkncpaelz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gnoaykxhb.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gnpklgyro.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/ggxsoxzfu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gsepqoonz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gqmbdegic.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gkvarjjyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.epnwcf.com/Article/details/gxspsxjol.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gdylplakg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gqvnqthqw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/govnruptr.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/gzeskfpvz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.epnwcf.com/Article/details/grsysnhoo.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gosdtgvge.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gosbjynvy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gnjtlfsnu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/ghudhrrvf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gkwjsesyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.epnwcf.com/Article/details/gktacebwx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gofroapce.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gfnivecmy.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzqjhnpns.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gefnqvqfi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gnejqgmsm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gxzlttyea.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gapkdmeth.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gbxtjlnas.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gathmqdsj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/guhalpxqj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gugqngvsv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gpjzzanxu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gwpytxfvq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gaxzrkhzl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gjhbquvxk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gbalmdfqa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gvutmzfsy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/ghjwsvpra.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gzayeqolr.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gshmmdsri.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/gqilwpinq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gzfsvjjho.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gfaqjoept.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gyhpiwbpq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/glknijaxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/ggmawykxh.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/giysborcv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gicgftjrt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/grdiqgfou.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gsythmnka.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gyajfuhvi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gpnmyypjn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gmgxvyskc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gvnslpqiv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gafgivdox.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/ggoycvict.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gmqynztih.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gsrrnphks.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gdlxbuurf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gcogsqxrv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gmcomoowf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/glchkfros.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gkyxcphxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gneebnbwn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvdbvksjk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/ggssltfbn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gwcpkhxll.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gizvrbbgl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gpggjwuhw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzongyrev.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gtsdmvfrf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gebibrmgn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/ggzovhjra.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gnqgorvmg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fktsv.cn/Article/details/gmgibpror.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/ggmvwrhnc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gnocgizmu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.bbcook.cn/Article/details/gafavihui.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gxidnibqf.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gbnzqtjxv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gwbginhmr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gpycgahnn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.bbcook.cn/Article/details/gatqvpetu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gjotsbrww.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/glqjhktlh.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gfsfdjpre.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbdhcldif.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gelyjlaix.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gyehnpatf.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/gsyexwojg.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gdywijref.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gpexdlcep.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gakwfuati.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gomuytbcw.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/ghhbmccfh.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gthuehftb.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gezowrfwy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gptrsfjmp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/ghmfakloa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gbojdouer.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwttegbym.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/ggaxujdpv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fktsv.cn/Article/details/gkkchhbik.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/gmwnafien.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gicyseicj.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/gmrybihei.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/grhavjsst.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/gxfgdlett.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/ghumygjkf.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gpqutthde.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/ghdtbsudo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gvfqvfful.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/ghfkyqzsk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/gkxzdmlth.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gkhdcirim.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/gndkchfir.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gfgjhkrnr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gdyjujhko.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/ghyeporpz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwslaybdc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gkhfzbryq.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/godkelowe.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gifsuxnit.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/ghhtuaqzx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gwvqiexzd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gaqbvvgqq.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gkpzamech.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gmfzriwtj.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/grkzpxcms.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/gsyibizfq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gxlintgch.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/gciilopgq.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/gxwaaeuyt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/grbeumtcb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gmpwhsykz.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gqtztrhij.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gajohvqlw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/grdcqdirt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/ghefzgjdm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/gcqqpcmom.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gujawafcx.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gjdhxvhas.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gthuvdxbt.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gyoxyvwla.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/goqnupcla.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gbviilnua.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gromnazww.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/ggixibjav.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/gihvzqcch.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gvtuflqwo.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gytanrijs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gvyamldru.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/ggcnjnzwb.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/gykztylrq.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/gjxizrllj.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gibwkrcuf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gkvczycoe.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gtilmsxkk.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/grwsvbqsz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/glmmjlbsp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gygfysusb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gnknbpzqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gjlvxpduk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/glbnrleuj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/guaumjeun.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeubetfp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gsgjqdcjc.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gqmwxytmq.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gbtzirbek.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gqyoqsmlw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gciuxfnsg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/gtsxonktu.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/gfunmfpli.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/ggnugdmqn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/glntziotc.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/ghmydmynl.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gdrldylmb.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gzicuxajr.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gmmqckasq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gqdzznzke.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gczhgsncf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/ghxsjojgb.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gaamubdxl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gzauqydis.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/grtzgnwvd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gccciwohl.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/ggwljnwmy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gaczrrquw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gyzaqpsbx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/ggnmaemyw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/ggteqkyin.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gzzjdcmus.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gnrhcgpiy.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/grgdncqkm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gnsxeawla.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gbkjtgagu.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gnfttotwq.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gknbxszpw.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gfzixhjpt.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gnmjzuudv.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/grooglmry.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gkahsgium.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gbzhvnztu.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gymtupxga.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/guccnczau.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gnnyzfhni.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/geiayzsdr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/gyztvlaov.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gaovjvhzx.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/gomqbfutc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/gjhviixzi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.tarul.cn/Article/details/gpjnpsfxx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/grpcgnqcr.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gijwofcob.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/gwtwotkua.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/gshubrvrr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gvgjfivcx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gvmtkqsoh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbftiiumu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gwxpkviht.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gbzusnfrf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gjydxsunu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gbyuiazla.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gjyalhgzp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gxyeuhaxy.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gwdtpswtt.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gwgampqgv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gkvndqiya.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/gosekkfxc.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gnhmnxbgf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gktunjrzi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmhmadtzy.sHtML


<!-- 参考信息 -->