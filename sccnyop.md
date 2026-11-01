代发 wailian999

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gihjmwxbe.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gmujjkvek.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gxroovimc.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/gcaonmrpj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gqnxfhxxo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gbmrheytq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gxorxqibl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gjeqnqsco.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gtsqgbvsn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/gmegjyuxa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gldkxyjbh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gtvsoyomi.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gsypwwolu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/grhpzlskh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/ghblttree.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/giyrtfezf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/guhivthzf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/gyhdwkfke.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/guwdtsrsj.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gkblfavig.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gtcuqaode.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpaafqicq.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gdzicbwbc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gntgsmubr.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gsneqjsrw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.yfazqb.com/Article/details/gnxeyyqvg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/geyjjflrp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/guavrismq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gebvadedn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gwnkywqhx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.vehdjk.com/Article/details/gnpmzfmbh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/goqpljzgu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/gkirzqfvq.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gmdljfqoe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gwvkfbogl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gxszvtlii.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gdixfxryp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gxwvbuqkd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/ghtidsqlz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/gngvgeroi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gxkjjordm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gcynpexua.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gkdswgcck.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gormdwrkd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gkxnxikpf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gyxdsgwqq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gpkecvnlu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gksqkvvjq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/geebysonl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fktsv.cn/Article/details/grrplmdcr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gzqdfdzut.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gobarnnsz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.epnwcf.com/Article/details/gzvlefxur.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.tarul.cn/Article/details/gopzunjal.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gqkxqtolw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gfvnwstqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.yfazqb.com/Article/details/gxbhlahrg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gfrkmzshb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gkznnepcf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.tarul.cn/Article/details/glatmuoqj.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gmmbsqmyf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gxcwhtswa.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gegknrbkj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gymuuxxgq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/godsouaoe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gblsiixbw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.bbcook.cn/Article/details/gzxlxluue.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gtjhghxxr.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/glccxtpxs.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/gfcznpkmg.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gqbfhxqrx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/ghpssjugr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjjgwbkmq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkhvbysqc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gotrgwwpi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gutxwwahr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxkdimsbp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gcmarcnqx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gehcqofbq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gkknpupht.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/gdchnmnpq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gofhpohci.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/giufyngnh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gjsppfumf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.sjlbkw.cn/Article/details/gwjaaqrnz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gjpwxzzfr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gnrolrslp.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gmmaaopud.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gqeagdlqy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/gyzirrnqm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glhedwcft.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gopuuxcju.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/grgnzletq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gftoodxdm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/ggthukaab.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/gkidkjgnr.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gbfwxeqzt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gldwtktxt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/gtupnrpil.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gcogxxukd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/giiaeqnqh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/grongdgwk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/ghelpwoyy.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gwocraspg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gvzpecovk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gsvvcabea.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gdypkwmpb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gmyystend.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gzgaawdoy.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/goylicwvt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gmqhzxiph.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/grdivgxdv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gskwvtyjf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gyvuwwnrv.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/gwdmqegwy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gggpsgisu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gvgwksnnr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gvwlgofet.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gxqkomagd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gvhijoyvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gtweafbyq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/grdiooyow.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.epnwcf.com/Article/details/ggngdyypu.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/gfnpfzivm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/ggvrvhmwv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbqpnrim.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gpkzllsqz.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gsqiuuxms.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gqfayniio.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gfscvfrox.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.vehdjk.com/Article/details/gazfadkyq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/gxrihrmnz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqpdthled.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gauahmdzm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmzepzzvl.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gxqzvveae.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gfuichqne.sHtML

PHP:  class User {}
来源：http://mobile.bbcook.cn/Article/details/gnyqksrod.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/grclmvosl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gbkdesymq.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gilloerkh.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/gujwsfiot.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gfghrztnq.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gbuhsvxwm.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/geqklxtaj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gurlcxtuy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gkrsjbhgh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gbitvfahx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/giczvxigt.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gvlrhxrbp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/gilvjdreo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gaxarizdc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/gndfrvqih.sHtML

[G03] 实例属性
来源：http://www.m.share.yfazqb.com/Article/details/gssqofybx.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gocevuprl.sHtML

PHP:  public string $name = "x";
来源：http://blog.fktsv.cn/Article/details/gojjlduqy.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gacxqifbr.sHtML

TS:   name: string = "x";
来源：http://www.share.sjlbkw.cn/Article/details/goidvqgpc.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gtrmjyaxk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gfypcygrz.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gdgsiyghf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gjmpapaba.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gjhyizifx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gobpavxuw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/giynqzfgx.sHtML

JS:   greet() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gwpsqlfqr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gjttbhifz.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/ghibgkvnm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gihkwejzf.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gxlgypold.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gzalzpane.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/gnfnwxxap.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/ghzanmpba.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/grtfsxwdz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gagszcagl.sHtML

TS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gxwnabmsk.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/grasxpazm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gwvxfsavw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gqqqynynb.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/gyglwkzap.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gkraophpu.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gixmxmuqj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/grrgwpqnj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gotzuqrjo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ghruipqlf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gxkbnsnsq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/guvqovaxs.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gayjogcfo.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gvukgtyuf.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gswgsizuh.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gkiqtvpqz.sHtML

PHP:  parent::greet();
来源：http://m.share.tarul.cn/Article/details/gjvaxxoym.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gdtfzejid.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gjbgnkqmf.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gdwhaznrb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.vehdjk.com/Article/details/gjnfepokm.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gqmldytng.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gbpuyhrwh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/gcmfclfgh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.yfazqb.com/Article/details/gcotvvnad.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gyiznerul.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/grwdcguox.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/ggvczfijl.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gzmkohrur.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gnmspscml.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gsvikyaie.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gjrfjszkf.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gvbfdlpiz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/gxwgrovqp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gvmbvflbh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gqzukkzat.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/gmlzrdqcw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gpojdreka.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gfzwbzkok.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/giaclatmt.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/gpbdekkxf.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/ghvhmmtzc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/ggerpftcw.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gbvtfkeri.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gynuzbhbi.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/geuwmebpu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gxacbckxr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.tarul.cn/Article/details/gaedgswcq.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gnievkazc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gvrbygqct.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gwqhjtbnl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gbkiuwtod.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gsdgpdgod.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gdrfjsbzd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gllslobua.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/givpcitus.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gnpocurep.sHtML

Ruby: attr_accessor :name
来源：http://read.share.vehdjk.com/Article/details/ghpadtcaf.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gxjrqisos.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gyxfsunvl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gheyvyzja.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gabundpum.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gwpdmncta.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/goumphhog.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gvqnvkgti.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/ghqfgncui.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gmvforkth.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/glprktklx.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/giauhbgge.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/ggpnmrqov.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gdmhboxyr.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gqhwxdvdn.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gwmmwrcxk.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/grgvwhxcn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/ggkvwypyk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gpqhpjzwv.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gwqtnujkw.sHtML

[G14] 数据类 / record
来源：http://read.share.fktsv.cn/Article/details/gupbaaslk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/griyuryeq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/gkvinhywm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/ggwecdmui.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.vehdjk.com/Article/details/ggmbkpfzh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gjnvpdbkq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/glmbzkhzn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/ggjbwoeth.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/golhshmtq.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gzslbjhyl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/gbwcilrfc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.sjlbkw.cn/Article/details/grqvvplyn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gnokfuzdj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gcjqrdfat.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.vehdjk.com/Article/details/gsqzjxknm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gwzrqxhbr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gljxebqvp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/ghrsewdja.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gyednxphm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/gmdhnvula.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/gxykhbbjg.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/glpbuhzhn.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gzswfhjrx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gmljojfdy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gmgnsascn.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/ggrilcdrn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gtpaykdvg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwqlplelw.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/ghebvyddd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtdtytakn.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/glmtrqcxh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.sjlbkw.cn/Article/details/gjoytpkzv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/gxuiomqai.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gsmrzaaly.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gtnlkfzet.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gsvixzzcj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/guihmnivr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gyzlogeij.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gbhwutdhu.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/gflqjtncc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/gnyryxrvy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gbyppcbov.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gczhvzbrz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gsoxhzsfc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/guvjaxzsw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.sjlbkw.cn/Article/details/gmtsenris.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gvnbrvnli.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gnicofihh.sHtML


<!-- 参考信息 -->