代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gftskffvp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/gogppulbf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/grpayahtx.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gugheoalr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fktsv.cn/Article/details/gawbaxfch.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gkqreuzoc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gmscmmhas.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gbztdovpl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gzswapdao.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/grvibwvan.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gqrqviaab.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/grupgpovx.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gjswqqync.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ggtljaean.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/grecrsdbe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gpjkigmta.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gypdyhsyc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gmkisigbm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gnsiddmde.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gnonnghxc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gtuwlbbrr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gthnivfxs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gbkysapif.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/geubgzhhr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gvyxtxwtz.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gjkjfmfug.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/goaecyoeo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gybwlgxgi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gatjjfiys.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gmiwkcqbt.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/grzgtrjep.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gwtddgrzk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gbpqhgcaq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gcykeizim.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gavuglsoc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gmqljwbxq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.tarul.cn/Article/details/gjmhtabnv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gbjrnwbtv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gpmhanmax.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gxjldmlfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/gnsvzirfr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gllgokwxb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gsluadxuf.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/gqqqniiab.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gwkbbeqpb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gaqiqqepv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gqtxqjkau.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gzaslgyar.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqhlitcrq.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gryybnniw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtooofiqq.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gviuuffgm.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/grdzllnex.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gxlumxqwz.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gzejjqsge.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/gphzqtnuj.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gsysdhysi.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gpexswazh.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gnlbslgwr.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/glhotulli.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gilytlbyt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gmsvstwor.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gqflirsgj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/ggyzrfkpq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gjukqgiqs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gptgaimtz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/giqqppvuf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gsuleugrd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.vehdjk.com/Article/details/guimasvnv.sHtML

[G03] 实例属性
来源：http://www.blog.epnwcf.com/Article/details/gmsuwpqry.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gvutvulej.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gpudypyje.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/giizlvvqr.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gyvtmznca.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/giazvmvzm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.epnwcf.com/Article/details/gaudhgajy.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gdknxikat.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gqhxtjgkh.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gihyneqti.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gpjmtfaqq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gzrljihjk.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/glvkkmmxv.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gcazttjyn.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gpqrylwsp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gpskjlwcq.sHtML

Ruby: def greet; @name; end
来源：http://blog.yfazqb.com/Article/details/gaewdxoiu.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gyiphyzes.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/ghtjsajdl.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gzmcjpiji.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gsubtkokf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gjlymwuoe.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gcsffcqio.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gownbipuc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gcpzadcul.sHtML

Ruby: class Admin < User; end
来源：http://blog.sjlbkw.cn/Article/details/gvydfgoxs.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/grkhcivks.sHtML

[G06] 重写方法
来源：http://read.share.bbcook.cn/Article/details/gkzxkyoos.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gjvdrghod.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gsopiidhv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gcluutcjq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gocfhwrjj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gxvvlrcun.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/ghymxkdwy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/ghmoassno.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/gdgsefpjh.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gofxnayaa.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/giekcztpb.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/gxnpqalwz.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/glboixalq.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/ghpiuifyj.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gyhinzwmj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/giywzmmgg.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gjlhlxpkp.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/givddxrnu.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gxjazkbpi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/gfmgmbqsy.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gvarqlako.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gidkiacom.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/garvoikgu.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gvwaujcpm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gdxxpmiiw.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gcjidjkpr.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gokgfddlq.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/gsirgugsm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gkujaklhb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/grflbhmaw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gvijhqvgq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gapcvtqcq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gixmkqprb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gfcfsffrz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gksetknru.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/gfbcsuydq.sHtML

[G10] 访问控制
来源：http://wap.epnwcf.com/Article/details/gpwcrycmm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gbrcnoisj.sHtML

PHP:  public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gpmkowdbu.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gcsqvipqe.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/ggjlfqacx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gkoalnxqy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gvlrbzapn.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/gahhpqtna.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gvjbwkosj.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gaxutkdxc.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/ggwfgygbe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gwbrbbhln.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gcvqgabqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gsqvtqsfq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/grfincoko.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/givewzbby.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gutdfxmhb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gyiuasyhz.sHtML

[G12] 对象转字符串
来源：http://www.blog.fktsv.cn/Article/details/gcojpvbsa.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fktsv.cn/Article/details/ggscflinq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gojswtqei.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gaqpdezvg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gitapannl.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gqctavuhc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/glirvowyd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gkkzhyloz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gqgwbitxv.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/gqzfvgizp.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gntgpzohk.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gpzzkxmwo.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gcsfttmxp.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gccaaqtgf.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gcgqcsbdb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gjcjcyohn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gyvxahbdw.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/gikygmvmt.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gmmfxpkhj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gfimnuafq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gfkvlsyuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gjyfhoskx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gzrjibqkg.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gwljkpkrf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/gyolvrsww.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.tarul.cn/Article/details/gzthluubd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/geqmtmarr.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gjtsgmkmo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gsxjzxsnz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/gygompubh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gmulbxalg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gctetpzjx.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.tarul.cn/Article/details/gqgjbrlss.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/golekxmhd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gqtibqvfn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gjsslovcw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/ggsbzpavt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gfycdlaup.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gwkzmhcws.sHtML

JS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gqlbecvme.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gtrkabtre.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gcslrxwbt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gsyiikatg.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gtbcwqxfb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gdcaovelr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gajvoyjmw.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gfflfmhfb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdgjpvywb.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/gdnbxxgkv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/ggpbfqfna.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gkrqytdgt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gjunmvutl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/grtkyamtw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/goffhcmvc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gqsmexdab.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/guaserypp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gncnpqoyy.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/gksvxotwm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/ggdqxjxbe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gnfeoynyr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/grnxgntxr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/guwwknrcx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gxzfshsba.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gundformc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gylmmjubg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gkzgdbmxg.sHtML

[H03] 主动抛出异常
来源：http://3g.fktsv.cn/Article/details/gqqdhyvjb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/ggqqyvahn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gbpbbzswn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gibcyvucb.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gkjudlogg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/ghdrtufzo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/gnducfoqj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gzfbrqzdd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gfwiohste.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/glcytyyzf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/gkmfcuesv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gdiyfyhoc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gjhejgika.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gpqlzmzfu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gddvdekly.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/guyjutcxg.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.yfazqb.com/Article/details/gfannrfqo.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/guwrioejd.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/giwuxromi.sHtML

Py:   except ValueError as e:
来源：http://wap.tarul.cn/Article/details/gexbzdphs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gyzomuwof.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdjhqhkjo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gyjxhbtjk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/gfxqiymjw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/glpisrupf.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/gpxmtgoyc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjixtewyt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gkizenapa.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/gwwcstbbi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gxjtkrple.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gccezyygf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/gjildebwz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gwcmnjjqy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gzzdpieql.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gakexebxo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/gqoyukdcj.sHtML

[H07] 断言
来源：http://wap.epnwcf.com/Article/details/gmutuzysp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.sjlbkw.cn/Article/details/gvevxyzzv.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gcsbyyzpk.sHtML

JS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/geulyzgnh.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gflwcvxnf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gssnovfwp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.bbcook.cn/Article/details/gjsnolvgy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gcbfiywln.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gaslvebah.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gvsovbjgq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.tarul.cn/Article/details/gkvtcbove.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gvhzdmcch.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/gqyiimxxy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.bbcook.cn/Article/details/gzylbbikq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/guyslnzbl.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/gwlsikspn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/gtgmzcchu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gjtwsjpqd.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/ghpuppfze.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/gddpaehsb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/genvobfel.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gmpqlbxjo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gmrxguqwi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fktsv.cn/Article/details/geedjtzcg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gaivzjtsy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdksmair.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gixzmvzdj.sHtML

[H10] 资源自动释放
来源：http://blog.sjlbkw.cn/Article/details/ghfrilsbb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gvglntmfa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/ghupweqym.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gvaxqdwxv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gjlexjrib.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gcyukmdbt.sHtML

Go:   defer f.Close()
来源：http://mobile.yfazqb.com/Article/details/geztmjmzu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gcaatykjc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwxwhxiny.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmkbqdjuv.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/guprtnsnz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbdfcmhsv.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/ghgybfpkv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/grbximtzq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gkjatkaeu.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/ggjxvavuy.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gydgxydzn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gskgvrclc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/gczrugtvy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/glpkdivho.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fktsv.cn/Article/details/gfxmggsdw.sHtML


<!-- 参考信息 -->