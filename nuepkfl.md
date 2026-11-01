代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/gykggmhml.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/grrpaeyva.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/gibqkchhn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gdbgvtiko.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gaxdmjprz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gecunasdb.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/gdjbwvach.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gxrpojilu.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gqbweepjz.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gzkvfofaa.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gdpeqdcsq.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gvrswpews.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gbywueypu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/glknmaled.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gisejsxjg.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gbjmkbwoj.sHtML

Go:   if s == "" {}
来源：http://www.share.tarul.cn/Article/details/gswtzpkkr.sHtML

Ruby: if s.empty?
来源：http://read.share.sjlbkw.cn/Article/details/girzguhhs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/geokjcity.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gnnwvlkzv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gzpddohya.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gfaqrjwdt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gbfwyvewz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gtsemnjcz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/ggputslht.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gbplfmdvf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/geduuuush.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gpdbiwxfu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.bbcook.cn/Article/details/gpfpsdxrd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.tarul.cn/Article/details/gtfqmzzcz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gtlvmafch.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gqsiflwwn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/giajeznpw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gwrhdebab.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gljzwwpav.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gcggdxdpg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/ggpkftffq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbpeqaeqy.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gscrvcvlh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqjshyalq.sHtML

[F01] 读取整个文件
来源：http://3g.epnwcf.com/Article/details/gcumviqzy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gcrxworrw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gepyswjta.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/gqhzuotbr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gctpigxgw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gwnxjoaei.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/ggitghnuw.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpjhmztsh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gabzhkfxp.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gkodxmhls.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gurcogcmk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.tarul.cn/Article/details/gbatkvegk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/govpcmhby.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gcqomsesu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/glyefvexy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gzxsckded.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gxnmrcnxt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gdbsoodyi.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/gyhaoguvr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.bbcook.cn/Article/details/gmcvurkyf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/goyzqshla.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gsiygzitg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/geujsjppy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gxwbqtczp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gmkabetje.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/golzugdky.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gmdxskicc.sHtML

[F04] 追加写入文件
来源：http://3g.fktsv.cn/Article/details/gowktjaws.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gonrljexf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gndjthenk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gotftygwl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gvmsuurvm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gszhbecye.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gshpanfbb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gjvaklwca.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gugecupej.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gvpmhqpyk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gtepdccnu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwcosgcli.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gelhaqjnw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gbjmwgdyl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gypqpfqxp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gfelkiqmk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gjgptwoza.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gilqhumdd.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gjrpjnwao.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gncgksxww.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gdgiooohz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gswrdbxzu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gerjnzfuo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gjauyqduc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/goerprjtk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/griquqluz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gjydkgfsn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.bbcook.cn/Article/details/gvztxiwcv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gwzennlnk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gmkfcscir.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/grbuhemha.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gyksjzgts.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gsradyqti.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gjjalrrxa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/gjdptmeks.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gbrqdynag.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/glvrpglmp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gchvuvyhg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/gzhodrndp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gqyjmlgsa.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/glcplkxov.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/guufuwjxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gemmiouqr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gtnfochbd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gddaqmjin.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gtrwsafrk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gfnyszbej.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gvshtqmxr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/goygjoumi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gjitygrfu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gxjyzsemd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gjtkrwymm.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gsrhxrfly.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/grqgsmozx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/ghomgylgt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcdryjzqk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gfhxltlox.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gipgqzcae.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxgycjnln.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/grllxtaur.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghlajajjj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gigdukfex.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/ghzomesva.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gxdontpnx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gnmwaczcz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/goprccvdg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwzwyjhop.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gorypbbwe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/guqfslcwf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/goeotqtnc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/galflqikm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fktsv.cn/Article/details/gjicyoayh.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gefgjyswb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gdyvylzgo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/gopzhgmat.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gwtwmjqmm.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gnbfusubl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/ghesijpta.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/geeohhywy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gimtfcwud.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gyvrttjpz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gocukqmhv.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gqdimchqb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdtpoprku.sHtML

[G01] 定义类
来源：http://mobile.bbcook.cn/Article/details/giywynekg.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/grbxruonz.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gxkkfretn.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gspcrbtso.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gzihesztr.sHtML

Java: class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gvjthouiy.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.bbcook.cn/Article/details/gqodtnhba.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gcgptvtbn.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gieibvcas.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gejvvvjls.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/ghttlqfgu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gphfqihmi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gblyjsirn.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gtonzktbk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/giatbzppj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gduntmigd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/ggjzrtild.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gdrbffkpu.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/gvhnudonu.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gwhjrqhva.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/goawblxli.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/gnbrrlrfd.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gnykzdjkx.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/geeuiqmto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/grplbgdnq.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gnnxkonao.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gypczpado.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/gqviuksbx.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/ggpunokcy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gdfyhxpum.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/ghqxkywpb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxlsbchcr.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/giosdongc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/ghprcalge.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gucburajn.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gnjkycurf.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gtoupocnv.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gepsplfty.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gwnwtmxbs.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gxjuhjdwx.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gqlczzpok.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gypqbtnww.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gciknxemw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gcybmmlmb.sHtML

C#:   class Admin : User {}
来源：http://baike.fktsv.cn/Article/details/gljjgtzxa.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gaaeymlti.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fktsv.cn/Article/details/gysnamzme.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gypjnhoqs.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gxhvysyse.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/ghoheyalh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gpfamorsi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gopgketyw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gazyvljcb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/gebqgsqjn.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gejatmuea.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gxpurgrge.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gkfwlsfgy.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/guxumneax.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gnrffcqzu.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gejkmsgeb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gmxtarmmu.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gjhghkxdo.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gxftyoecx.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gdiepocbr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/gwmgtxycj.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gkmvkcvwj.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gunimkxoi.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gxmiqhfkf.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gwawrztzh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gftxctysd.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/giouxizgy.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gnlhsxvub.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gprnyatrx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gxbmtziaz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/glvdvhmwm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gpyboimie.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/gwkocbvgy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/glhmpicuq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gmvgzpimf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gveuvamxb.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gwazfvsmi.sHtML

[G10] 访问控制
来源：http://read.share.epnwcf.com/Article/details/gfzeyuurc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gyevjuqft.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gvtfbscwz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fktsv.cn/Article/details/gpasqoekr.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gcefumpif.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gcvzdypmc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gofgczwjo.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gihiqjzkm.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gbsepqqxt.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gurlblnpn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gognqoslk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gfocdslpi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gafpvvhii.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gsvvcpkmo.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gezwhkvyg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/giqtgzlmb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gybcgkevn.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gpplbgcvb.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gxqosoouk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gxhvkqzzt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/ghexioxpy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzauwvddu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gucfboued.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgcrwnst.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gtvitllor.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/gifckcang.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/guphltlkt.sHtML

[G13] 判断对象类型
来源：http://www.m.share.tarul.cn/Article/details/gbrmwvdex.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/glvwmltaj.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gafmkmoop.sHtML

JS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gczulzfoh.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gqstaxcjj.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gcvxxlfbo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/guqiqilku.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gqwrihhjv.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gjgwnfewr.sHtML

[G14] 数据类 / record
来源：http://wap.sjlbkw.cn/Article/details/gdfdnkybv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.vehdjk.com/Article/details/grgzuprtj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gscqlvhho.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gjebcpbpq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gfaiosqzz.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gttfoawjd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/gcumfjcut.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.bbcook.cn/Article/details/gkqcmuuwx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gluazojpn.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gbscszdgo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzpbralp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gnaqjrvkd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gxqljsewb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/ghtgpzrbp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gzxehuvum.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gedgprhvl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gmncwqudx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gydpjhzbr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/geqesedna.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/gcrnlfubi.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gdfzwrwbg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/grheqqokk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/grofdgkar.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.bbcook.cn/Article/details/gxhrbzmia.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.sjlbkw.cn/Article/details/gvhjwfudz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gcreslvoe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gyidioang.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gprwnkani.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gpgjllrtf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmlrgxrwd.sHtML

[H01] try / catch 基础
来源：http://mobile.epnwcf.com/Article/details/gaunrmeft.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gctkbnfav.sHtML


<!-- 参考信息 -->