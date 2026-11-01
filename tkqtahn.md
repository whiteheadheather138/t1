代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/ghfovdmlx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gjcyiqnsb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gddcjofld.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gfrykqzwl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gtiqgsbyt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gvpsyhong.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gkkzezqxd.sHtML

[F04] 追加写入文件
来源：http://baike.tarul.cn/Article/details/gfrsblfxx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjjeyeov.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/ghsvelgpt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gcpvrfkxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gebctcmgm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gjzoegqvf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/grvarlsdg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.sjlbkw.cn/Article/details/guacsepfb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gysimbsxp.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gcqvvbwxi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gdtaovxrs.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjrzpmtgh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gkirjfepm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqhebyyro.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gsnxmpzvm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gqbrwuvhs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ghmbeulvc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/glzyufjgd.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gtwflyoex.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gnpbqxpwn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gfgrahziu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gulqtjztw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/glmqppkyp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gmmfdbvsw.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggmkothnu.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gjennbfea.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/gxpghaoha.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/gfyolljbb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gzclwcuja.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/ghfiqwkxu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gbzjicfwl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gccfdyjgn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.sjlbkw.cn/Article/details/gtjauvnbu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gzajqapjk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gbqrbcldx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gcsfqymem.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gnlzvqrnu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gwyllnpbh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gfuiudyrj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gaufdmuil.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/grgirxity.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/grzxumbpl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gsmrjdens.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gxytjrgpn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gdzcyqhzu.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gcdtvwrbv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gyqwpedmy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gigozrnhj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/guosxkhtq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gentbyizj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gmcivqoya.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gtzjekarv.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gamvurlzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/grqxbvhdh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gxdanjcli.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/givktrvsj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/godygpotf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdhfmyuzs.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gysfbqcze.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/glkeaxptc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfnilczgm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/geaxwrldo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gfunnhrdn.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gglgkjwcb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/grnyqhsem.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gyhygjeci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gjrchjsup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gmospbeau.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/gvvpopcvl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/ghuuneqhi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gctteoito.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/ggekwmsrz.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gbymkrbhi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/gnqvhxyxf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.sjlbkw.cn/Article/details/gkuwsjmlr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gseecvytp.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gorpafpva.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/gtojcprgo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gkdyeqcop.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gdjdiouts.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.tarul.cn/Article/details/gdderjjfh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/geejewgpu.sHtML

G. 面向对象
来源：http://m.share.vehdjk.com/Article/details/gmnothucz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnfcfmxev.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gmyvxmtdh.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/grqeyvgzt.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gxprttnwf.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gengvepci.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gveccunmj.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/guarzolic.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gxkixogzz.sHtML

Ruby: class User; end
来源：http://blog.bbcook.cn/Article/details/glvcsebpf.sHtML

C#:   class User {}
来源：http://m.share.epnwcf.com/Article/details/ggigxquhh.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/ggwqgroky.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gsghxkcxr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gksdyhwsa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gzuefxffn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gaudujveh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gcssxfbjv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gombvdpbc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/gqwsemova.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gjylkwmld.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gpbfsfbjl.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gxnegiqwb.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/gehzeywba.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gbeivhtmd.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/guqxcleib.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gruketems.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.vehdjk.com/Article/details/gbfnbxdpc.sHtML

Ruby: @name = "x"
来源：http://m.share.epnwcf.com/Article/details/gtxvndzbd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gidcfltoe.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/geglnknhp.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gfcfqdgxw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/giyhqdpov.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gqxjjdfcv.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gkfbtnmho.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gtcageyhq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gacfdltrp.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gayexqwew.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gsyxbjloa.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/ghazsjpbw.sHtML

Py:   class Admin(User): pass
来源：http://wap.sjlbkw.cn/Article/details/gyipjrjou.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxnfylarh.sHtML

JS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/ghvouegci.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/ghrwsyesk.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gtzxantmc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gkgvcznie.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gsfpyrlse.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gpzaqyuhy.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gnldvnnkg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/glkptxspb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gndtmcujt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gkioamrju.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gtzcuaenb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gvqwnlttb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/gmeaqbrpz.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gdtmtqlhx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/gxixjfppe.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/gboswfghh.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gnwiipjvp.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gjxstanhj.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gucdmlona.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gbjjkeeyj.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gvyzzdtqu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/gzbxqkpuj.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/giohpmvgb.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/gfkfqeubl.sHtML

[G08] 静态方法与属性
来源：http://baike.epnwcf.com/Article/details/gcnfylkgb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/grpstmans.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gbrewrytq.sHtML

JS:   static f() {}
来源：http://wap.epnwcf.com/Article/details/gvyhiqdmv.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/gwonjfptb.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gajjsvrax.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gapnldylu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gglceadjt.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/gkevetxva.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/glmkuobiu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gqheolgkr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.sjlbkw.cn/Article/details/gzilmxiui.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/gnhgjfvrc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/grljonhru.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gwhyeqafs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gmxfmycsb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gsjmubcod.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gidweqswa.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gnjqxsnyn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gbiffrveu.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gvvvuocxm.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrphtmfo.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/goxopfkzx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gpsiotjbs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gkmosbvfc.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gmzwnwvpy.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gjsdjwwkv.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/ggejhlbjg.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/gzcxmymho.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gttxquhfs.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gaogvtvzq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gqursvnfx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gbhopqsjt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gmkurxxci.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gcqpovdbh.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/ggsqpjcym.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gwpnxlqke.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gxsxczcti.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gibnaabkp.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gjuijuyex.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gfidqdykr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/ggukivtlz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/guoyhfggu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gfcdarwul.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gcfrsewpi.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/gwdbkyide.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gfnnkftey.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gzabnyqot.sHtML

JS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gbhtrhles.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gcsiierav.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gsyvqplpv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.tarul.cn/Article/details/gyrvgewmh.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gxqztualr.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gbqkwnewq.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gvrobrjpw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gjkdbidzp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.sjlbkw.cn/Article/details/gzwlttlxk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gjqoauhbc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gkxjjiess.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.vehdjk.com/Article/details/grypymnlp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gdljhggnx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/gwjdmeedm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gukrlinyd.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/grqzxccsl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gpvbmpexl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.sjlbkw.cn/Article/details/gcbfahalg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gjnnyibmh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gknycgjqz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/gcmigdxmd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gunawkqfu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/ggaudwxwt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gxztmrujk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gyrapjooj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gbdpsiipb.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.yfazqb.com/Article/details/gzocryrfa.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gtbbegwba.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/ggkiedhsx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gtfpdcpln.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/ggvwrljsj.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gwchgueot.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gxlmfdpuz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtblthprq.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gqwvibsap.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbhxotnpm.sHtML

[H01] try / catch 基础
来源：http://read.share.yfazqb.com/Article/details/gbpenqrrg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gqmceqtgw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/ggausbsir.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gafbwkfzu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/ggpypgcdg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gomdkepgv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/ghtyudavv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/grhfsglcp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gftyholen.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gvntjhykq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gtrqqtobz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gglxvynnu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gmwalvoij.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gvetmagko.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqznlqbtf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gianlcrjw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gerkmooww.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gtshxsnti.sHtML

[H03] 主动抛出异常
来源：http://3g.yfazqb.com/Article/details/gmwgozqcv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gjcnmtlwq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gxiwuktva.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gsresbvnp.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gzwckhpcx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gbzcgwdyj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gggykwlac.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/gwqcshxqk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gddohcxia.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/gqjjdfawd.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/goldnifys.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/guykiczko.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gbvtyjcfr.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gjjkwaxyg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gbmbodjyq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.epnwcf.com/Article/details/ggyakbamu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/gjwunlovp.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gtmxhnsjo.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/grdssvjpv.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/ghbwdzizn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gscbnprfq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/geuduqndr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gevobcopi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/gabvvkkji.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/ggosxwlrk.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gokbfnahv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/gwioizpve.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/guostvgin.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/gbrtaobok.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gpcaihiml.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gabdythnn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gupfqbdzr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/glpywocwi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gwubdzkby.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/grxvxasvu.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gzlcgwjxu.sHtML

[H07] 断言
来源：http://www.blog.fktsv.cn/Article/details/gtjptwlnh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/giefcyqhg.sHtML

PHP:  assert($x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gmjdwtiad.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gujhbqkoe.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gpoblxccb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gzxvdtwtr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gfwiamirg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fktsv.cn/Article/details/guavvyvgg.sHtML


<!-- 参考信息 -->