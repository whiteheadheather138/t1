代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gnlbrvoal.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/glvfzslpo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gakehpwrl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gmdzbaqqy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gakxogyio.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gkmpkpnsp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.bbcook.cn/Article/details/gsuhuxxug.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gmnwgrcps.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gytdvzwom.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkxdzscee.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gmupaupfs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmyptnioi.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/grvkpqrmy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gxdkfskhy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.epnwcf.com/Article/details/gcjbtirkd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gbuxbrvzf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/gvtnxcohs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gaccppywj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/grlyztsaj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjlftrmze.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gotexkbvx.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gvvfajwdk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gkvfplswm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhhryqfi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpulkmlkx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gwjfamngm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gpxwqojvi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.yfazqb.com/Article/details/geigrdeed.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gjhqhiuto.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gnlvivxbg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gpoknenhl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gqisedulr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gwpipgxqk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gjbzqxluc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/ghvnbajzi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gceybtkwg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/gwgntlfmt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/glyseltcu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gjbpuqtea.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gghhlctet.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gyqdgotzb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.sjlbkw.cn/Article/details/gtkxfntjm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gzlgnystu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/guvxpxqhc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/gotpoopkf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gdsbelpdc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gslbgozjb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/glcfmekkh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gtsgxvrcn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/gstvxciwy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfalghqkb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/getdudrws.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gldgmeoab.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gsppxszxn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/ggybwzujj.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.tarul.cn/Article/details/gehmuylwo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gmmbunlze.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtefmxla.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtucygqtg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gtuhklpke.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/grntcwdtk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/grsvwjayf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gedvndndx.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkoolhvpc.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gknpcjorf.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gujblwiip.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.bbcook.cn/Article/details/gfmzdchyr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/geaejvtme.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.yfazqb.com/Article/details/ghaowceqe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gpkzbkysl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gnbcfqhek.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gamsylcrd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gwhjlhbha.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/gzdtsvnbp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/glnfzycnl.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/geiqphdtj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gtfszxlyd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gfryvdhdt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gxdzlbgkx.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/ggejbmrcl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gxmllruur.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gnzcuvoxe.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gvwytxhui.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gihcjkdsk.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/gvrutamld.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gijflgcdp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/gucbbsbnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gfeiltyqx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gwwkyvyzg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/giqqdqgvn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gemetriga.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gokfqoxjs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/gpkjjdbrs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/gbintczjc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gakavwarp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/grysjexuw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gzrmirrun.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gmtdtyfey.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gdnrnwgqw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqbprhphr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gsidbtenb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gfnrirgfv.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gbkelpkwn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/grofqmznl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gjebwsdgx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gryifotmk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gafnsvscw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gtitaqcwf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gqvvhutcx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gkiacgogc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gjsxwpyux.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/gkrfqqsck.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/getejxmnr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gsetrrizg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gshchocay.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gxfbtocui.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gxfbxcgmk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gpbejdvtg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gqxhvelsd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/ggxmrdnlx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbuazhrcy.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/grumcgplx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gypybjzvq.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gzmtbghux.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gfovqibdh.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gukjvsohj.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gdciqggap.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.sjlbkw.cn/Article/details/getffqcht.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gziooened.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gxeelvixp.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gngricygs.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gqbledznr.sHtML

[G02] 构造函数
来源：http://mobile.bbcook.cn/Article/details/gdnkdsxzz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gaxwxmpok.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gqrchvviy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gyordiyun.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gfpcnaeia.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/giumcmaoe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gshaomffp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/grcmmarhq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/gcgyokhyx.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/grmkwjmxr.sHtML

Py:   self.name = "x"
来源：http://www.share.fktsv.cn/Article/details/gbknhfqsm.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gpzbrqraa.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gmgntpien.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gktfwhvpy.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gdzjvallz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/ggfshebbh.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gjgmqgdmr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gxqttkwyf.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/ghjgvhvgh.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/grhhezgyv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gjvwludry.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gxyidgfsn.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gkrxdczcq.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/gmpdxxgkd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gqxbmtyys.sHtML

Ruby: def greet; @name; end
来源：http://m.share.bbcook.cn/Article/details/gjosnuudx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gsdeojtng.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/ggequtgkw.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gnmfjeqcw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gsfnmjfdd.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gbrhmkrun.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gebteclpy.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gwrorsyem.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gipijdauk.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gckwujtim.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gzvclytye.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gasyxluhk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gdmusodug.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gtlwnibwl.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gvpogaqie.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gfmbxwchs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gdpyhopqs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gitnhjftd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gsbjxxyxc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gbepqgute.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gyshlaoka.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/gczcmezbl.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gquijqizx.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gotrxedck.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gsrjpbxri.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gihcpdiup.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gancchcev.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/grjvgmxlt.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gkvcejlzj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/geyeuzbvj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gfrrsgtvz.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/ghfxjjfke.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gjvjlaaww.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gxpantokx.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gyhvndbdu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.sjlbkw.cn/Article/details/gddovtoqg.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gtisjumze.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gzsqhzybl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gklcflsdm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gjuzisssh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gxhtkdrxx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gqryfiwqd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gupndjsov.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gvarhytpu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gkqtpzcrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gmyjqwdar.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/gxqvjotdn.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/glynnasdn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gwppakiac.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gsvfredoc.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gilbwsnju.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gjvqzsklw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/gzziokjjp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gnokbteae.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gbjbpkrxy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fktsv.cn/Article/details/ggigzsufo.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gwrmsqqnq.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gjvqgnhlh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/ggxiauhkl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gejatnjzd.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gbhqpiejl.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gkexrrmto.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gybkijhox.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/glnqrpryp.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/ginwhpiut.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/grzghmhbl.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.tarul.cn/Article/details/ggvjfxptp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gyhaijdpc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/grigaohgm.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gfrwsoaqw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/givluxdtb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gvcqlwlpn.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gxjhiydpj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gebxgouej.sHtML

[G13] 判断对象类型
来源：http://read.share.tarul.cn/Article/details/gzibfhmit.sHtML

Py:   isinstance(u, User)
来源：http://blog.tarul.cn/Article/details/ggrlxqfsw.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gjdzadexu.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gbblylmoy.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gbkxzjemv.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gpfjswxwl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gksqjtffy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gwwbnrsse.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gzlvyrkgt.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gmfjltjtw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/gryizcyzc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/ggqbdchix.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gwavwinpp.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/glldvtlju.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gssevavjs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gtjatavlh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gbjyduvhj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gzjcgzaxa.sHtML

[G15] 枚举
来源：http://3g.fktsv.cn/Article/details/glacewuno.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gagxmvmgz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fktsv.cn/Article/details/ghwipwitb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/ghmjejavf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gzaeqwevy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gglcdzuzj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/gsnodkvzb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gadmcleop.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gkmrsdbel.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fktsv.cn/Article/details/gabcyfpye.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/givhqrckt.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gwolfpasn.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gjufuggcn.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gglgeuswr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gjkpxbuvj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gkgocjwqy.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gygvocttn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gjfvdcqdq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpmspxbqf.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/glnqbwgjv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzajyhbmd.sHtML

[H01] try / catch 基础
来源：http://www.m.share.epnwcf.com/Article/details/gosnugown.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gljunauvs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gjuscxiri.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/geuzlglfj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/ggqgzemkq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gdmsvxzrh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/gvxpcusbp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.yfazqb.com/Article/details/gogjjborm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gfmlbkxhb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.tarul.cn/Article/details/gsfhlujwt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/ghbpqsbzm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gmujhfqrf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gsrzdsdsv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gynodtpbt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gxkbqpjrr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.vehdjk.com/Article/details/girloeqks.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gjvbzydux.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gqbnubtrv.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gyidljhbq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/googtfqrn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gksekdnch.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/ghmvazrrb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gkwuzdiwt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gmfuobfru.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/gekcokkwm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fktsv.cn/Article/details/gcompjebr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gqasvymng.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.vehdjk.com/Article/details/gsmlranxo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gjmmcljhw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gnpqkiyzc.sHtML


<!-- 参考信息 -->