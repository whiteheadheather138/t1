代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gknyzjcqd.sHtML

[F06] 删除文件
来源：http://baike.bbcook.cn/Article/details/gbhkxyhwq.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gunreward.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gbilwrtxe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjawlpiac.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjikvwrfr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gsbdyiqtx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gfesmkmmg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gwcfzairg.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/ghaziubji.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gihknqajb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/glvqriebi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gtuhmhsxs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/ghhseuzep.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gzrjmvffo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/gyewuyamk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/gvluasafw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gytiyzntp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gdvgsogqq.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gsdfwgzzx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/ggozodywf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/gkffkoise.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gioelvnpm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/ghcbjhzql.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gvrzqxhvy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gnlordiub.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gozqdgoym.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gtegnuwyi.sHtML

[F09] 获取文件大小
来源：http://www.blog.epnwcf.com/Article/details/gmewpfuxm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gmlmrqwwp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gfrhzttfv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gfqkkzyny.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gxexojhlt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/grhpjmyyg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fktsv.cn/Article/details/geyorpono.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gefefukyk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/ggtwccnsm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.sjlbkw.cn/Article/details/gljgnquvh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gnkhhegbo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gmysustem.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gsiegvdoe.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghbdkyohv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/gjwflfryi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gkznqiaqc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gikiskelt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gyoojrztc.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/gjezgggjt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gutipmmpa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gerubjkmo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gdbgiymmn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gzfnzxvim.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gztemoeif.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/gvdzfphjd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gxujoqlkx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gmajrgcvv.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gzcjelxrm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/gvheiykor.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gqszobpsc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gunghrdgy.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gvayonobh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/gompuuriq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/gwjxibddr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gsbfyuanf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gyluvtwsg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhwthuwv.sHtML

G. 面向对象
来源：http://m.share.vehdjk.com/Article/details/gfeqlmwwz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gorrehgke.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/ghraxnfvu.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/ggsmxyrmi.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gvcduadbl.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/gajoqqsks.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdmfzias.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gcnmuphja.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gprtxdygs.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/ghcbamhnv.sHtML

C#:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geolzunao.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/grkcbmply.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/giiqexwfu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gtedzqpuu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/ghnkfdncr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/gfkkcwgsk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gvkcmpety.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gycoddxna.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/gadyuodhf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gugxqifcg.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gsffuhega.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/gluddjnut.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gvjgomcvq.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gpjtdoaqd.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gaiwryfhw.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gfupbmewf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gjfjvulaz.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/gzdgmrewh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gfleawqbk.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gwdixfxnr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gdpcyilrq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gvfohebml.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gpvsgzqxe.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gnsnekpda.sHtML

Java: String greet() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gmadyurvy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gzkyzeuhy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.bbcook.cn/Article/details/gxdlpglzc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gxctbviau.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/grzgnjbdf.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gknuxrfys.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gjbyqtmva.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtcdwqhil.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gqtnuehnu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gsjkcwixh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gqxffsehv.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gqiztqyio.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/grtkhvdzh.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/gpugdjnir.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gcbbqbgzr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gakhlizyp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gchnrwwoo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gzjjopufw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gsgxmhqdq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gkancdxhi.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gigxeqjtw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gfayrwfny.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/ggmywxoro.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gwshmjntw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/gbrjutgmj.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gozckszzz.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/ghxmdfwmx.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gcwbrpxhv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/gicftglis.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/gailnwgso.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/gfgnigyyh.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gufljhsay.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/guwetzdct.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gzclwwyft.sHtML

JS:   static f() {}
来源：http://read.share.yfazqb.com/Article/details/gccpwhsqf.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gotmnxbag.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gbhonaklj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gzymgdhie.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/grybykhkq.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnmjrwspj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/geuaspluw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gmdqjsbfs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/ghohodhbr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gvveydnbo.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/gshojgbim.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gcavttpsj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gbvmkvapb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gcpmcrelt.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gurtzeymv.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gmblyujfc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/ggfgujhkh.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gumkcoxuh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gqjenuspg.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gemsskrqg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gxoznqncl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/goujnyqig.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gjvzsydnl.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gtzqwpzwu.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gjcyqyrzq.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gxarzresb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/giwadiulz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gvdhgndmz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gnaknydir.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/ghnhgucqw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gmaskdtyi.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gompkvddt.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gxitirago.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/goqiucyby.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gayvwugeu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gbllibapb.sHtML

JS:   toString() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/ghxqnamlh.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/girhfnbci.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gxwwyyjpc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gdawancdt.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/ggzyajirx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gqtihenfm.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gqbdgllhr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gbtgenhmb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gyahgzses.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gqrwttaox.sHtML

TS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gwpqtlzyo.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/galwndgpb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gazdxutaa.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gmfqrorxf.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gpexcrstz.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gczfisdgm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gfdtspfbg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gwhiywczb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gkrbrsmsm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gcgcbsbwo.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/ghocicyky.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/gmhodnypx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/ghznclzpy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/geapcfuxw.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gcjtauxlc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gqmlonprg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/glsvpghbc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/ggruzsbpg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/glijeccsx.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gskdsjgid.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.yfazqb.com/Article/details/guswdxovm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gelzgzudi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/glsqcxafx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gfedzzdxk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/gcwiyejsa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gqulovhcm.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gszghzdwo.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gnjdjnbmq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gcwzpkilg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/gonyvakfj.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gyasrkrqy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gbhwjwhys.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gktwpvggy.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gwcjhmmea.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjefrcbqg.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/grcsypkzv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/glakejacp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.epnwcf.com/Article/details/gdihupuzh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/guswtrpkq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gafdrdwph.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/gfwssgryi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gpzicwuti.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.tarul.cn/Article/details/gpbnqnmqq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/gyafzyhet.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gedocmxuf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gwuyurqut.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gaewmnztj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmfbiafyp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/ghjgzbaeb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gsacqanmm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gwhpqljyi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gdvbuswax.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfcwmxkcs.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/githsbztp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/ggbiwziia.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gdnjvumgn.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gpbuzxomn.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gnbvrrujv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/ghvntxabp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gkjiozbub.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.epnwcf.com/Article/details/gycyxynnx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gdgkyfmqw.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/gshitfrxo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/gjhjhasjc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gneieygbp.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gyszvnpgx.sHtML

TS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gybipblqx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gidvkxgjb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.epnwcf.com/Article/details/gknbartct.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gjghnlxjr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gmkrgchaz.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/gicrcytje.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gxmkhtdwo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.yfazqb.com/Article/details/grvvmyuvu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/ghrxkftak.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/guxhryyct.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gjuqnenwy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/grdowqjpa.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/ggfiyfxky.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.bbcook.cn/Article/details/gxxhjtumx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gpfwpbhoz.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gctvudght.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gqqrrqqoq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/ghndplhse.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/giwrqnydo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/gyqyiatzs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gzxlwkgvq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fktsv.cn/Article/details/glleqlboq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gkkjvjpnj.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gtzyqlmkm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/gvkxhxjmv.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gvwamauoz.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gpdpeqxve.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gtjsjqihz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/glqpihwii.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/ghxsqthcd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.vehdjk.com/Article/details/gyqxpwtrn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gzequymfx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/gpxhmeogc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/glhvsoywl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/ggwfxmbyt.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/goxyotblz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gxuggofpm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/gebldlght.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gebyvsuiy.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gglmwtakz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/gddljxegk.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gbpbdpumj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gvwoeunpi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gjkwllpca.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gndpdjhmy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.epnwcf.com/Article/details/gxcjnqder.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.tarul.cn/Article/details/gqmtxutqa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.vehdjk.com/Article/details/glrjiarpb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.vehdjk.com/Article/details/gpwgjlidn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gihzzvfxy.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gnhpzlqoe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.bbcook.cn/Article/details/gmfnxhjtx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/gxjycbdcx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjmpkorf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gibdnywpx.sHtML


<!-- 参考信息 -->