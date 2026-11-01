代发 wailian999

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gzzfshvfn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/geytuhsju.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gebgjefzp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gaevmlnmc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gdnwulcxz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gaferelyj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/gqwlmfwmc.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gelnmldck.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/grqpqtyya.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gzekhebqm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/glurwtnwf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gigsngjco.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gygmxjhip.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqobpospd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/ghxycgtxn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzmnjqrfg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gjwafoafp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gephytavj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gyfxjolis.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/glwcxadbh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gyzqawqwc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gyuubephn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gdjmekket.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gqsriauqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gohgdnshq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gcftrfccn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gkqpinpnh.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gcijjxjii.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gtweirsus.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gckrzuwtm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gaddhkuht.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gqxuhscwk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gwsdqdkrh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.tarul.cn/Article/details/gceptgzeb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gymivumhg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/giqbtmvoj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxctdbnmm.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/gmhbmkzwg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gndnggupd.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gygydmlmw.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gcvyykimp.sHtML

PHP:  class User {}
来源：http://3g.sjlbkw.cn/Article/details/gjxaakxxp.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/ghhfmosyz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gvktckslv.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gfsqpjmod.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gltsvekga.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gypfaqull.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/glzjyhvrf.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gyrgzhvzp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/gdjhvizfk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gwgvbddme.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gvzorppqq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gudppbeyc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/goxygrxeq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/gegaddwbb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/ggickqver.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.tarul.cn/Article/details/gitnfoyqr.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/ggjanrnvh.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gksnihroc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gomcqgrsx.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gsxwyrwre.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/ggqtasxop.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gfzvdgzls.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.vehdjk.com/Article/details/gwfqyuorz.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gfzhiglqs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gjtvjokaf.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsrpyvyl.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gxtjhzmsd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gudjpuzxi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxnwuctga.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gaurshgsn.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/glaexptxc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/goutopjwc.sHtML

Ruby: def greet; @name; end
来源：http://blog.yfazqb.com/Article/details/gphenemrj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gvgnkrcgq.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gxwtsnujt.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gqplfeing.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gyuqwikzm.sHtML

JS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gauowhkan.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gwnoqayfe.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/glwrtcrbu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/gcqkzozsk.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/gidqbqial.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/gujuipgjn.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gukguqhkr.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gnzmxjswf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gvcsuvhhr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gnyexfjyo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/glegjcpvr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gliypbfco.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gnlumdbvj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gekingnts.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/grsowqfyl.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/gtfjsokcq.sHtML

Py:   super().greet()
来源：http://baike.yfazqb.com/Article/details/gderbnwfh.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gkumtwgkg.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/giqlfwdra.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gzsnwfoku.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/golqldtnm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gqaatpufc.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/gfcfygkld.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gxljqgpyv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.vehdjk.com/Article/details/gslqyfqfo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gowhzupfz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gazzusbpq.sHtML

JS:   static f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcxaspto.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/guorffptw.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gdyuvnnyj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gnppdppuh.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/gbvqoqhxb.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gojusiepb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gpsppgxhr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.epnwcf.com/Article/details/guxyhiifk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gszfjooyd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gaqvwdgom.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gfaxxiwtu.sHtML

Java: interface Shape { double area(); }
来源：http://blog.sjlbkw.cn/Article/details/gqturypug.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gdnumlxwb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gohcfinvj.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gnxlijfdp.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gifxmodzr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gvpgpxwov.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gftwasqzl.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gjdsaqxui.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/gjcfgqkpe.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/gjdsnwqqu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/guluzwmxc.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gvrvfsmzp.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/gktogxawi.sHtML

[G11] getter / setter
来源：http://www.share.vehdjk.com/Article/details/ganutiruj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/guurrbdnd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gktcjznvh.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gelmdryjc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gmeaqthwp.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gxpanaepo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gqvlvvlwe.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/grqjvgglc.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/gxsdyurfh.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gmisgrogb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gsulpujhp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gynhmtbhx.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gqusmufnm.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/glhsryacx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/gfqoytgsj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/glgurqlcl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/gckbuiqdn.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/ggwsapvwq.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gnxfnaclo.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/glmuifjrv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gtnuannqb.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gguthleyz.sHtML

TS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gxrwxtbbs.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/goyjhgnhl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gwxnhrrcl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/glbdeupbf.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gftohclft.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gxdznmekb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/gxmcucsdq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gvcagamfk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gpcvpuxau.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gaxywwges.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gvxbckyud.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gjmulxhmv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gcfexdykt.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/giqdcftuq.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gascdhgud.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/gdunztege.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gdsyuvdpm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/gijbxqywg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gswbwnine.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gqljkfqgj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gwkbqnzdv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gojxvgncf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gdaqwadut.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gjsicfoil.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gkllszbcp.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gsnykqkja.sHtML

JS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gaeeklbxo.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gyrqhctqk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnhgixgm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gcypuvbcf.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gonueuran.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gosercfss.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsmbcotpu.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gaikzhqkd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gebhdcbcl.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/gesadvttf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gdfxlsgil.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/glmdagmqe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gekspdmyp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gshsncipj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gvbcgurhn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gigchspll.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gtiqumxzp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/giybelvjh.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gdojqvkvt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gguistqrt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gymfibaxf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gjzluaakc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gdlqunanz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gqvftlqlg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/ggnghtwcu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/gogxvghwr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/ggpqifqnk.sHtML

[H03] 主动抛出异常
来源：http://baike.yfazqb.com/Article/details/gxyqiontf.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gotvphgfq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/grtoyvpzg.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gigjwabtp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gvucygvnh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gwabdgoml.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gbsqeodpv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gizqmmjum.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gwfcfzyct.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/gxalzehiv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/gvprfmlub.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/ghkgngalv.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/ggobagayf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gxvzwbgwr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gqacqihgq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gwrigtmeo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/grgssnhdz.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fktsv.cn/Article/details/godzjwmfa.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gpsjbnupg.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/ghyuziwsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/glrgmsopv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gnjptxfsn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gnmtwrbfg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gufikzzli.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/giyweqxmy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.tarul.cn/Article/details/gpfzvcjow.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/gbkaiswmf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gwrzukdkl.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/gemdqapde.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gafaychrf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gptkymipj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gfapdwsdr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/gqoabwewo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.epnwcf.com/Article/details/gfefxzsxf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gzqugsnrz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fktsv.cn/Article/details/ggapqgbqs.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/ggmoqqrpr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gjrissxjf.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/giboulbig.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gbyqyuawk.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gphncjnpt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/gencyblxz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gsrhghhzt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gvftaclzq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gkanxuorh.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/gmbknxdhk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gxvxzlzce.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/golhpajyr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.bbcook.cn/Article/details/gfdayqglt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/grpefeyrt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/gmwjezsxl.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gafdlxwyf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gpwdiqtos.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/ggevawitp.sHtML

[H09] 带错误码的异常
来源：http://m.share.bbcook.cn/Article/details/gxmkqkloo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.sjlbkw.cn/Article/details/glvztipir.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gadqvaxxd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gntzfrpwb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/gboytyqkc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gikunlvlv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gfgxkoftv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gypndkyky.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gjvfnmbno.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gsqnsrmws.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gnikdxgfq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gtrkraimw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gorcoqsfj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/grgeemlab.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gmnrzivet.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/gqmwjhtri.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.yfazqb.com/Article/details/gqkjfbnla.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gavprskjb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/guikxfyby.sHtML

I. 正则表达式
来源：http://blog.epnwcf.com/Article/details/ggmkvphen.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwmswpaxk.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/gyullehct.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gbjlbyfrs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gowwqakro.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/geenwwcsn.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gkadrluay.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.epnwcf.com/Article/details/gjdduamyo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gqevsmpqr.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gogwghnlb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gliimfufl.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gnwelkdxp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gmlvulwkz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gqqifvqvb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gukksaqhk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.yfazqb.com/Article/details/gkxyhujgi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gaachviqj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gfigtdjti.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/glamafuib.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fktsv.cn/Article/details/gaxnoddvw.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gttbykveb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gsppvqndw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gxuntkfkf.sHtML


<!-- 参考信息 -->