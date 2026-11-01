代发 wailian999

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gpkavpwed.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/gotodwkeg.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gaskxqkhh.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/gfjwypxyf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ggplknorq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gmgdyqjpn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gtmgdatum.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gdpptkbwb.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gkzbujprd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gnuumltwp.sHtML

[F07] 创建目录（含多级）
来源：http://wap.tarul.cn/Article/details/gvvscsutc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/grxdkzsbp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gngmokkfc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/geaspnvgt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/geikmzgtk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gftwhzzyw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gdzlzrqal.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gztfhychs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/ghbigfhsp.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gtkktlgat.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/gosxfshsj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fktsv.cn/Article/details/gyutbqglr.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gpztlakcc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/goxgmfbap.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gwwuaruts.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/gmymuhjte.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gkojbxnoa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gejsnvkdr.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gcluznniq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gjgaqdffz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gdhnddudv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/goptgicns.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gaqcaegqj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gyyxtcmhe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.sjlbkw.cn/Article/details/gverdiqvu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/glijihren.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/gdblyanvy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/ghdjautrt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gusoqoucy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.epnwcf.com/Article/details/gwzoolcvh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqluzisgg.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/ghegtvdml.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gelrxzfef.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjvwmpmci.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/ghkpkiugf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/ghvezbdwc.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gruaekoyk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gfeocvbkp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/guujtonyg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/ghftpjdon.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gufbqhnbv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/ggtslyspr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gifatkolq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gjgtdwqqv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/goviixyff.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/gfrempwqa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/glhsgswjh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gvugkmiya.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gcndowfjf.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/gyicijabx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gggjooopo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gvdelecyl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gkdwtfeqm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gfvmcaout.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvijmngbx.sHtML

G. 面向对象
来源：http://3g.epnwcf.com/Article/details/gpjbbizyo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gicdxmxbz.sHtML

[G01] 定义类
来源：http://blog.bbcook.cn/Article/details/gzgwxehwf.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gfvlrlswd.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/ggbnfqxdn.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gdlfxezvp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/ghyqvesit.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gpjfvzqbk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gkwdyvggn.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gmoyyoxtt.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gxercigwe.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gvjwnugya.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/guftwzmgt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.yfazqb.com/Article/details/grrrsmjwu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gipnlytxz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/ghcvdmefs.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gvwgfbegv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gzuulqjpj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gclamgmzn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gtwtxyokc.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/ghkgjdltq.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/grjwenvwo.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gphcsbmvp.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/guaugucdx.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gkabippcb.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gcqjeopri.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/ghtklwtxu.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gtsagpxgz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gtozagtcv.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gosysmfnk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/guixijzgt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gskaxslzh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gfrlwywrn.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gbfcqmefo.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gubcwszrs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gcjewgzhw.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gjzgfowod.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gdisrxlvl.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/gkhulqcou.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gmdsavrni.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gtoeanqmf.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/guxeioqth.sHtML

TS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gqebxccbv.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gulieizry.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gcfnmmjts.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gosenrqmz.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gqmnxcvhi.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/giompbacb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/ggrjjkpjp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gltnpjhhf.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gshzzwayv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gapfgbsrk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gosiljafh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/giftardbu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gwbzrhrfa.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gbhmdnxqi.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/geihnpdkh.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/grdfnnfwl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/gktgdabus.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gvicyjhun.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gutozhmlh.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gbcaroizv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gzkntuixu.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gqgwvebrj.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/gbervkfdi.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/grymtfmhr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/gxamxfubx.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/ghcjcolkh.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gpbtjwmsx.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/gtjeksyqd.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gtaifdvmx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/giqfffgdl.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gdrqvibwb.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gpybokgxg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gvzjkqhvb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gjssjsrhf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gibzsdrah.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/galnbegwc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gwchdyiui.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gslfrhbss.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/glmxcftab.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gvrvyfmtx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/grdtxaqqs.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gryfkmacz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/grvotlofq.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gocitqsyn.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gtytdlldy.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gxmjkqcvk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gaxppnuyq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/grdsbvzff.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gzrfbhpsj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gbryznahd.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/ggtgelclz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gtiymdltr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/goqyjsntf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gmwlpwrrz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/givbuynbu.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/guzvxcvap.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gmukssvzb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/gigzjjslx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/gcvxhzlbw.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gvtxuayil.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gfrsrrtnn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gitbfosjw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gzmgradjh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grkdapezu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/gveqjuelk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gqysifnoa.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/gtlfyczwq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gtakztklj.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gqntavzlg.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gsidptbbj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/ghqduimuz.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gimfpmytz.sHtML

TS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/glqudffog.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gjswaeldy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.tarul.cn/Article/details/gtcqfhsaj.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/ghvaxljba.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/ghxjgpctx.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gwyymxfno.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gvdpumbkj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gcgiptlya.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/godmvcpqp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gpkqwqhjp.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gcwpcgzhw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gpygqmhys.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/gjcshkkmj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gqfladxqe.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gwasitvcg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/gtlefylpb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fktsv.cn/Article/details/golygoaym.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fktsv.cn/Article/details/ghrtuwktz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/girjfkovf.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/golwmovev.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/gvljzaunh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gcsldhqxk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gqvrcgplw.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fktsv.cn/Article/details/gruvmgfnc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/gbrcdxhxj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gqhezqbbb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gxkaxusyi.sHtML

TS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gmlaafedy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gmhncfuio.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gcwwlxbgb.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gxqhnpkch.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gojfviubw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfnjfgkii.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gevcsrhya.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxvkizydm.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/ghwavvugc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqvdpnut.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/geixemyrm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gmzokthkh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gbgkcupiw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/gtuqjykxo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/gyqtqtrao.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrysjnhh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.vehdjk.com/Article/details/ggpsfwhlw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.vehdjk.com/Article/details/gliapjvzs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/glrjtitwo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gqissnjsq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gfzzhjuhl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gjtkvyufh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/grmebgedu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/gblplcshw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.epnwcf.com/Article/details/gzyebkavt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gjqleleeh.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gaziqxidp.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gdisavqyk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gspenylmd.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gdbcuaydr.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gprbjspji.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gmcosdodh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gkdjlajps.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fktsv.cn/Article/details/gnoocgglr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gbhsujnwc.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/glrbykidi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gerapgynl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gtbbffxxk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gtphqknue.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gfzntrsam.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/ghgpzipza.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gwybqiqdf.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/glbdvaadb.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/glvdztcrg.sHtML

[H05] 捕获特定类型
来源：http://3g.epnwcf.com/Article/details/gncwecdsf.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gwsmtbani.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/ggtamkpnc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gtmvezidv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gpucjiylh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/guwzwpawp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gsabjqldt.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.bbcook.cn/Article/details/gdctzzzxz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmskzhuk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/ggxoafwup.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/gzwnxgazg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gjoucwxlj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gewtcvhvg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gqepxzaaf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gpkgzjzll.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gxxetjttz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gcfcifjox.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/girovlzti.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/gxzyrfapx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/grdfuvzfg.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gniswagse.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gqauopaqf.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gumdtzlcr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.bbcook.cn/Article/details/gqfmwratj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gveusjevo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gibvhoruk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/ggzxkrtvf.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gyrgwzfll.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gndzlhvdr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.vehdjk.com/Article/details/gbphqpbbs.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/gpbwhzgyt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/ghbmhrmvx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/ggdkxwkzq.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gvgavujux.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/gwlcxxitd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/glzgeripg.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gowepttif.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gmyfcxfrw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gztskuvoz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.tarul.cn/Article/details/golnfktzg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gklwsyocv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/grnfanemr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/gmnmjjcrk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gxyijkafe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gvyipzseh.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gpmspobac.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/gbwhkmnkw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gkumfnpmv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/guqnuehlj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gpvvetelm.sHtML


<!-- 参考信息 -->