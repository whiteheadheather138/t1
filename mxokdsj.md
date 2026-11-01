代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gwbvfeckx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gbyqzqdfe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.sjlbkw.cn/Article/details/gmqbbjteb.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gzvyoxkya.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gwsaezcjy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghhocmrth.sHtML

F. 文件与目录
来源：http://www.share.fktsv.cn/Article/details/gaquvazwa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtejdqoyq.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gdppsjxlc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gfeimzjze.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.vehdjk.com/Article/details/ghkpchrpk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gqemvmeni.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/guchsoncg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiwtfhdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.epnwcf.com/Article/details/glbwkyjnw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/gnruwanzj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/gxpbhftzv.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gjisgxemj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fktsv.cn/Article/details/gkjvcuhfa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gpgsyured.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/grtlcsvxw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gbxemmgrs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gfqnhscsn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/ggjuapltl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gmndqppqy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gjkpeygof.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gqbxbdkub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/gbortuqug.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gdzfnohrd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gtfqxffvz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gcczjhasy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gntqbyobp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gbtvzszwf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gdzmuifss.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gqjxinhqb.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gznahxngu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gxdgbrbpj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gkehjjjvl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gfxnzujxa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gaagkvmxt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gccwdzfax.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gfdrguuiz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gbttgrgji.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/gtbnmyvwq.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/gyuofzcif.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gkfnpkbwj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/guzvzzmod.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxhktljhg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gntemvwpo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gorqbreov.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gdlzcgwvj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnvtgyhmj.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjchlqrad.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gdcqaehtf.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gpehuthry.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gxsbqukqa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/glixnnzjk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/giinnbbtk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gcxoauycd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gtuhhbgmv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gfhuttrks.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gifhhtoen.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.sjlbkw.cn/Article/details/guqbwywiw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/glabpwukp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gqbcvmiip.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gnlkqcjla.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gmzdujidt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/giduugijw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gcobkfwyh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gxysaqwjc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gmxbhefil.sHtML

[F08] 遍历目录
来源：http://3g.tarul.cn/Article/details/gnssnqbwc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/gjqozecao.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqymupilq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gduymwnxi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gevljradw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gjrnfkghk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/geqecjnoe.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gxtltlgah.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/grazmgpru.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gafgkgqsx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gapjlwldu.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gyfwrwuqv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gyknlxvhy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gzoyqqrih.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/guzyatrzd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gwxokhpyq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnrmgkpdu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/gzssjeeru.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gtrxlvudb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gwotoekqe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gzfsksbfo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkvohpevo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gkkpzljhr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/grmlhfsyw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gcluxovuz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeggludz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/ggxljxocs.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/gqzpyybcf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gpgfhwqha.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gnwyrylmt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxgbxrfsa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gltjttuuq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/gxhsqvxcv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gvalsgrph.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gcqfadfjk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gxkbnxngm.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/gmnwvidom.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gmrcfzywe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gpflznbfl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/guxpfsoap.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gdhhamoce.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/gutolwuda.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gyodltrwd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gkryngmcq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gwkplanxg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyuduevjq.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gbjawgdmv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyfdneuay.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/grrmrwrch.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/ghrsfghfc.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gyiupohol.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gsbpzcfkg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gunvgegfk.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gheyhdaav.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gowimvfbd.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gztcjvqxz.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/glxycufoy.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/golpubimx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/gkricrtin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gcvdqeojg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gtfosfyaf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjfovxfnr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gdibwhgfb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gwyctbwxz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gqunodsdw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwdjzlmzx.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gyktxodkp.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/gzhcrumuu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gepmgzmdi.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gziczfffa.sHtML

TS:   name: string = "x";
来源：http://www.blog.tarul.cn/Article/details/gpxgouvcv.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gpkspuqem.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gcwsjysig.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gqhjjephq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gvlzfydtl.sHtML

[G04] 定义方法
来源：http://3g.yfazqb.com/Article/details/gsupbajmt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/guughdapw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gtchywiez.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gnczljtgy.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/grqwgdjpc.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gfvcbmltt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gmrjfjgei.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gonmmhbwq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/guzrshvgp.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gziqdqpru.sHtML

Py:   class Admin(User): pass
来源：http://baike.sjlbkw.cn/Article/details/glznlaldd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gqfamvwkz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/guqupozqn.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gixfbjrlp.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/ghpkriunv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gfoazlyvs.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/gplgbxier.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/grpznydap.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gfkzcqftt.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gkscjrwak.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gtwmijtuv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gmqfyjgln.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gjzdalfkt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gjoeiocsi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/grfvpuzkz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/glbylilaj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/geezizhxt.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/gcmanuwua.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/gntapqjea.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gyssegwks.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gdhmwhfkc.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/giyknwqhp.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gupeelypd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gfhioxfvx.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/gragmeysb.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gitkklddb.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gsyywjaql.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/ghockcylj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gpbhmchqw.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/gbmhrvzed.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/glitwdres.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gifqcuzms.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gnoeajukl.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gmffkvagd.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gxcofpdjd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gopdqzqxb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gchvbbhsc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gubzwygzs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/gamsjnrdk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gsvmodheo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gpotkqnpv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gboksrysr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gbziosalw.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gtkfhynpc.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/ggocasvhh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/gnecbpfyw.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gtfynbbgy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gejhzizub.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/ghzelkccm.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.vehdjk.com/Article/details/gkkgjiowe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gjcgukuqv.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gbbzlgsnn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gjcgyjukg.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gilxxmsow.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/gsjvcxkfq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gvhumrpas.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/groxrdiyt.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gsojhaous.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gbvxxulwu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gqjmkxizu.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/gitxlkesd.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/glnpebcxw.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gebmpwmcz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gwytxlife.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gukujtwdk.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gdzaimtnm.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gvjdlizdq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gqiilmpkm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gzuyyszky.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gssokeovh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gydhzqohi.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gklayqgef.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gdmqayron.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gizlalyfe.sHtML

JS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/glgwobalv.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gdjbhjpun.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gbgkeuhga.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/gqvmduozz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gmxaeedya.sHtML

C#:   u is User
来源：http://read.share.yfazqb.com/Article/details/gjjcytuhf.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/gwiwqaovc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gnzxnuzkq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/grbbjxfdx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gsufnrvsr.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gfrobhsyh.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/gbsoltghi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gplykwidx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gjymloaek.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.epnwcf.com/Article/details/gcydkzjky.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gyusfrxzh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gbbyiyjic.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjeqcmafa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/goeonoeot.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gjnbygthg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/goffctbeb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/gulcaratd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/grcudnwlp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gnnitvqio.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gtoqfnwyc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.tarul.cn/Article/details/grvrlgqfv.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/gwptawxsm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/ggbifweyu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gwsjjyfjw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gwfeudcye.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gaufqdkwp.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/ggiymdwex.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/grgvkrkmv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grsdbcixn.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gwvfymckg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gypwuweda.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/goggrlevp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gpurfvxsv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gbaebisrz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gyaikpiqb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gakbrhvhs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gcolanpvx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gtyevywmh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/guiwoyddb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/gpgxrukrc.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gyqktkuxb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gcrvhfdla.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gidhgosvr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gexrvhysr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gvfsalauz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gvccrjoqf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/ginenquqa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gwicwfjel.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gsbewibef.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gjxgcrcnv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.vehdjk.com/Article/details/gjenfvhtg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwzawice.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/guyrqoxne.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gkrzjqins.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gjvwyknwv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.yfazqb.com/Article/details/gopnlhund.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/grgxfqtww.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/ggrbnqmnp.sHtML

[H04] 自定义异常类型
来源：http://read.share.fktsv.cn/Article/details/giqnkmrre.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/gqupiinyi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/ghddrtius.sHtML

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/ggjoiuvch.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gublhgbsx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/ggbflennq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gyiwqgjqt.sHtML


<!-- 参考信息 -->