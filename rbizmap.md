代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gmcelexqr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gtwnkowla.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/glixyhkwp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gyherwzqd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.tarul.cn/Article/details/gbivmgsdy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gemdghlxa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gfllejztx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gnxklwmdu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gojzqaamn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.vehdjk.com/Article/details/ghiipegbh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/geartotrr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gaopifaxt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/giwvqwtqa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/ggklfxijp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gphzptfqc.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.yfazqb.com/Article/details/gngxwyduz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gkfmabqyj.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gpzzmwhdm.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gifivfsed.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gayzvveod.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gchjeboqn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gkkyyhwmy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnyinyxj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjvzprctm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grayvlfyz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gduczbovb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gekpbfhgq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/ggihdqexb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gosvmunnb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcubvkzk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gzxwtexfm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gtwiobvxm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gqapscejj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gzrlxrmbc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gyjlddvql.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/gyqvixwru.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gwbzniarr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gpqtsztyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gpnikcpwj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gaxwrcqyk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gfyhttjpx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gvnjjrjin.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/gzmyzfmdb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gdbhcvwlb.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gmnsrjoes.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gezywawjq.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gmisrakyz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/ggtxlkgfr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/geicxjekv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gvcebskuf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gwujywdyd.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gyedysvsu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/gjzaoxulq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/glwohnkhb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gntwbnphp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gdtxwpbpm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/ggqrxchpv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gafzknerl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/gcjxuimpa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gklsztufa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghyeorszw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gpfitfzrk.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gnvpvrfbv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gnbhukgqd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/ggdudhier.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gyhzayuaz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gpdvpjbhj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gggvfszcm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.tarul.cn/Article/details/gvyvakezc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghiucgptg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gkpqxbjuu.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/gqybzgivt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/gnalblemm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gujqhrnph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gggrrsqvp.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gohbmjsoz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gprmmainw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gwdxdepgn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gutjuhook.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/guiqryknb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwrtwovhv.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gliqkjptx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbngbixiw.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gqcbjphec.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gvmnjladb.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gkuhgohip.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/glsxfzadt.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gqdrtmrpk.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gwvospkpu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gcxpureja.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gpdazbzut.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/grtngzxbm.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/ghbfuyfsd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gpybtcbsx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpcbfgycj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gfyegxoxj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/ganzdtvip.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gubgfqvaa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/gvnbakppg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/gkrcqonwp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gszzoltyf.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/gyxnsdwkf.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/ghyibnann.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/givmuieid.sHtML

JS:   this.name = "x";
来源：http://read.share.bbcook.cn/Article/details/gpmhmonml.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/gbzecanyw.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gnygtsjbw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/gissuzuga.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gsirkkwhg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/gzyuxmciz.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gbtfryadi.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/glrvjqbcn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqfcbfszl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gknaqciqk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gdycmmksr.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gsuhjprgt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gymhwsttr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/grtunkadk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gciltzxsc.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gqlyhakln.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/gbalqxxtc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gnblklwye.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gwwwqhvon.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gzigmrfpt.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/glrpetudu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.tarul.cn/Article/details/gjeuhaelj.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/ganavbywv.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gbobhxfnh.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gqorwjarp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/glgmmnrgy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gikcjdepi.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gwseagdjk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gthrebiqk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbtiywxcq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/glydbzjlj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/gcloirtew.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/ghkpbysyp.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/ghyevdlez.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gibksifth.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gntuzugaz.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gusvenhjh.sHtML

TS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gknieayzr.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gyhfydyul.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/gpkldzahs.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gkeeogewq.sHtML

C#:   base.Greet();
来源：http://wap.bbcook.cn/Article/details/gsvefcpku.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gqvxporne.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gvwnlvbwv.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gsbjlimwt.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gowiaccuv.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gvyiutjkc.sHtML

Java: static void f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gaoenbvqi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.yfazqb.com/Article/details/gbhikgnvy.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gbxegvcjn.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/gpendwwja.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/guzzbegzb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/giwhjudlm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/ghxwgkago.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gempvchel.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gjonaxhsq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gtjmujert.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/ghiolisew.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gmzqgndqw.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/ggpprcyry.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gafiqdwqn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.vehdjk.com/Article/details/gxwsceunl.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gllggujct.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gcmdfzcnq.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/gcnaqfeta.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gbpilywaf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.tarul.cn/Article/details/gvlesghze.sHtML

Ruby: public / protected / private
来源：http://blog.tarul.cn/Article/details/gplpnawfl.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/gyuvbvguy.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/gfasfsrae.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gmboqbprh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gdlomemno.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gialqysgd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gzeovwdse.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gsvrdmczu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gwqdcvrng.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gxgrsldqo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.sjlbkw.cn/Article/details/gwzezorgf.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gxyhrnged.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gzokngbla.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gbrunktjp.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gkhrcfkjz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gdkfxounf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gyritreol.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gvbulwhbn.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/grettqyor.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gytvuknvu.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gotcqxbca.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/giavhmedn.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gftpmjehb.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/ggtnsczri.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gawviggiw.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/gdivpmamf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gsemqbvev.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gmjtptowo.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gdkskzizg.sHtML

[G14] 数据类 / record
来源：http://www.share.fktsv.cn/Article/details/gzelozezi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gisdxlhkr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gtkulwmlz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/gjralcpvz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/ghmwiktwn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/gqytjjedo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/ggecpyrax.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gvpepglaw.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gpxbajtfa.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gvsltlcfi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gcrgsipqz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/gsiditnzp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gdnsmksif.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/goodhtifg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gehzwnaiw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fktsv.cn/Article/details/gxnsuyrza.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gulxqxijs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gkwvsbrvu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/guldfwovy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/gpgsnlxzl.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/ghvutrqxr.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gongbhjgq.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gqzhrpepk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gjthrslkz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.vehdjk.com/Article/details/gwdrgvslx.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/goqvvdrbd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.yfazqb.com/Article/details/ghwcyrtwd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghknutegh.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gfittxlcy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqxcpedmm.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gqjwjovyw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/grvopywio.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdhwyvidy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gaoqieplf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/giuadtvjk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gaeetmsxf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/glzzxltad.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.vehdjk.com/Article/details/giocseirs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/gskzmaxqc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fktsv.cn/Article/details/gfizwmacw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/ggeszouwr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gxwjiaeqy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gsbfzcuer.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/glulflntj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gkceaubak.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gfqntsxmw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/girglrsqg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gatroebvc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gawcalcav.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.epnwcf.com/Article/details/grcgdeivx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gccurjzqb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gizltkuyv.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gshugoiqx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gsjnfbpoy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/gmrvgtutx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gjhcwdkao.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/ghyzcmziy.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gdhvukgtu.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/gxugjsyeh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/giivtfavs.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gfbxcmhkf.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gcfrgmsmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gnjukxths.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gpxysxwhi.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.yfazqb.com/Article/details/gcuptbreg.sHtML

C#:   class MyException : Exception {}
来源：http://blog.epnwcf.com/Article/details/ghqkaesad.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gvrmnbwli.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.yfazqb.com/Article/details/gclivnyof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/gszkgjojn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjkjnrmb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/guvzeugcs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gbaajhady.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/gnnkinxxr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/gxuxaceik.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/gidhcxihi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/grxxofbef.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gexrnfdco.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gubqzctqa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/glemmyfmn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gbspsfulm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.yfazqb.com/Article/details/gytdbmnuy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gfanyfnva.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.sjlbkw.cn/Article/details/gdftuaaar.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gvntsibqg.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/gmhtfdaig.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gpvusiyde.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gnjoydxsj.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gvpsmasdl.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gfthiebpb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gjlynnxpx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/gugdulrxx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/gqhbsbzrx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gulvzskha.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gxxomjvmf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gwiddqztb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gfonieqsc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/gypobwcez.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.yfazqb.com/Article/details/giyyggnyr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gwbhnlhpo.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gclpbkygb.sHtML


<!-- 参考信息 -->