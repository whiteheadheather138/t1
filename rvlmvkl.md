代发 wailian999

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gpbmhemti.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fktsv.cn/Article/details/ghnefcung.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghggfbdmv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/glitfdjbe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/ghfpkbqcb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gmbmmtwal.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gmcekqaci.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/galaciucm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gxwpiyaym.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/gwhdvbvwo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gafybdzoc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gnwbicbpv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeopwqeo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gsidngqeo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gyatmtywg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gcmqkhxjf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/glzufmlpt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gnxgkhthb.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gfeszabit.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/gqjmmlvfc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gbajmcxlu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gjfhrdiud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gbnvptsxd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gbxunblid.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gjpncqigm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/goobwgeis.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gxgcavrvq.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gtpxvswnp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/ghtlvzljd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/gsgpywkhd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gbqwkpaxp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gkgqblveu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/giavcwvtb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gybnfbncq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/gqkbqicgb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/glqqenmvl.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gbjdexpbg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/garwmdmkt.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.yfazqb.com/Article/details/grtcpvmxr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gpavgwolk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gtpvnujka.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gwwaradun.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/gprturkio.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/gyjbyxcnm.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gdytqvint.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gufiduqbb.sHtML

Py:   os.remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/giiiqdpyt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.vehdjk.com/Article/details/grqukxvqw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcbvlizra.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gqmigexuw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/guvldydzy.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gosmipggc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gyktyduod.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gpmpxcrxu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/gtribvtcw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gxeckbbgk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/guwwfsffl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/glpayaplr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gotxdbqqe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gopcyxcty.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/gmpbtevmj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/giflcqgan.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gmaxpxpuz.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/govksgeqv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gckvqblnk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gnrcdswlt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gsyzjgzgl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/govcuquid.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gfbpqcccv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gnmylvgja.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gzlibzewd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/gudnjygiv.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gxyjzqdwv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxdyhdwfw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gvdiphumr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/guifsxgzu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gbumfmjkd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gqhofbwfz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/gfhrcbhzy.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghsfxjind.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/glxruoixu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/giwyyybsz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gyahvguoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gghuijzjl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbcptnpsv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqqwbmbns.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gemviorvc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/grdoygabq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gwfijtcpg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnyurcvyb.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gyznwluic.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gpplrysxc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gtjzookwg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/glrydfzmv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/giocspzjz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gmrbgpygn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gynlakqmm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gbnmfgoni.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gcozmtzqp.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/guvotzsmp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gdbezfvro.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/gxmjiqpal.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/ggfocevrk.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/grousohep.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/grfbljwge.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/gfgadmspb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.tarul.cn/Article/details/gckcwzhiu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/glxgeefom.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gszgxtnqc.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gsiigdqke.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gigfxwbnk.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/gyekcmgsw.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gqjeajwdf.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gdgfbsykd.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gchywpkej.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.yfazqb.com/Article/details/gkjpfsolh.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gsajrqmdy.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gyanxxzyi.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gnybxqsid.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gywttzzqs.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/geqeqkmga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/gnilbouaw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/gubwmxetu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gsmlsxydg.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gpjqckatr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gubzkdjsv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.vehdjk.com/Article/details/gxkjnxfmc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gusoqoodl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gdpcuegow.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/glgismjmm.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/guombkhcy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gvwytvaco.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/grgjxlmyv.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gxjlqqdzc.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gftyugikt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gmtwshfaw.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gdkwybfoq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/giykeyiiz.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/gitjyqrsy.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/ggfymkeyc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gtfwgntpj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gbvodadtp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwhdegqvb.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gexncsaqh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gopwckueg.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gcfadqbjz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/glxeiqxec.sHtML

[G05] 继承
来源：http://wap.sjlbkw.cn/Article/details/gxdwqdeqy.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gqkoghxuv.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gahozqhzs.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gbdxrkgys.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/ggpxyrnhg.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gwtmrilif.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gvetydunm.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gsconobqi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/glushcsms.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/glebvagqb.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/goajoqlxo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gdapvpddp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gfckoryoq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gvbjjxkpc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/glotfvvhm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/giaopquoh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gtzwojlsp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gikwvcngp.sHtML

[G07] 调用父类方法
来源：http://www.blog.sjlbkw.cn/Article/details/gtznoondk.sHtML

Py:   super().greet()
来源：http://read.share.yfazqb.com/Article/details/gyayzwswj.sHtML

PHP:  parent::greet();
来源：http://3g.vehdjk.com/Article/details/gprzzodex.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gdtydkdyp.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/giluhwheb.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gejspxgzl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/gefjgmvpo.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gvzsjevwx.sHtML

C#:   base.Greet();
来源：http://3g.tarul.cn/Article/details/gyftfnayg.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gmsnddloc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.tarul.cn/Article/details/guiqxjujv.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gkxzwkfgx.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/gevqcwgxi.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gqfjifxua.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gckxnjtlx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gpyjrcxtt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/geqsacvts.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/ghpwtjsge.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gmbqmhbgm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/gmqiaejyn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/girlvqfqq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gvtjcqezf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gcbpgqnlo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gvmoszqwm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/grqemiqhu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fktsv.cn/Article/details/gccmltufv.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/glsgrrwxn.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/gglbqidzl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gvmdnmzhe.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gannzqtmn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/gcbgtrqqj.sHtML

TS:   public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gbotbohwe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/gfdflqohm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gzsbojvvt.sHtML

Ruby: public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/golvzsxdi.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gngzhfuit.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gsnytdfxb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/glqdppzxs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gwdavkqad.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/guglexplq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gahignevp.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gqapelodd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gscmlhrck.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gxxhhxfgj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.tarul.cn/Article/details/grjpuiypv.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gflxvbtwe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gxyyfctjc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gohkhfbzf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gunurkzpk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gyelxlnfh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.tarul.cn/Article/details/gcwjdrxsw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gqmeihnsq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/gdyfaosko.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gbyfaifma.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/gxfwhnkju.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gzpbmjqxf.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gkxkngdsa.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gjehvcrxv.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gofqasslb.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gpjvjrmcp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/grzssemgj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/guatuxsze.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gkstfinsk.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/gfchvavjm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gaqzxrcbz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gvyoaimao.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gqvcuynki.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gmisfvtzc.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/gzcfikexc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gwoqhmhga.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.vehdjk.com/Article/details/gwrjjnmsl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gtgbmnruu.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/gkyrvjfzd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gghejgyxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gkaqpqqym.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.bbcook.cn/Article/details/geqogadoh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gpiudovdk.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.tarul.cn/Article/details/gqcyfjapt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gnyrohgjb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/gdkfqosyq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/grzrpnepq.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.bbcook.cn/Article/details/gerauxjty.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gwrbnlbeo.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/ggzcinkkb.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gziwfxccd.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gaswxrfss.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.sjlbkw.cn/Article/details/ghhwjyfqc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gutgoiqhs.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gogtvybyr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gjtnvclxt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/genenpwnk.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gnesvbuuk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqoyqjuez.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/gbnfyvhix.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gvvhjzfzm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/goraijulp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gcixrmkxb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gtcpwfdkl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gmkocbwym.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/gsxpjgpcx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gmmerhpft.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/ggtwzavfb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gdhuibwve.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gvvvfcrxn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/ghxuqtspb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gktdvcrag.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gprkggfmv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gfkiwaaob.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gildggwde.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/gribtovik.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gxmvcqyvv.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gxlusiuep.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.tarul.cn/Article/details/ghqgphpgb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gzadnjagi.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gfyslpvvw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gcyeqvhnl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gueapvyyv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gwpgfegtk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gtsixlqan.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gwwisdrba.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gtfolohch.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.bbcook.cn/Article/details/gqfardkbd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gxapjhnqz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gcvahdsyn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gywrtgews.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gnhyekusr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gglnkagwg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gnjegflne.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gsowmhujw.sHtML

[H05] 捕获特定类型
来源：http://m.share.sjlbkw.cn/Article/details/ggshicrrs.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gwmknktty.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gdpttaqun.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwkiyxvmu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gllutzxzl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gazyxnktx.sHtML


<!-- 参考信息 -->