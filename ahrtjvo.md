代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gjdfsyhgz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmnsxffkt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gutjljtwb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gbvirnteu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gubinjsms.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gvwsgimxr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/giuzwekws.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gaumbqigc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gupiubqdr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/glgbdvpkk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ghsgacksg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gvnrfqzzn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gpgwwhyvb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gmicnjpwg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gqeqyjbja.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gzsdzmdek.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gkwsvcuqu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gdvpwgute.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gcptfpxug.sHtML

TS:   // 同上
来源：http://read.share.vehdjk.com/Article/details/gqfwbitfu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/goucigddq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gcdfwszzj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gomybddia.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gcwwakjjg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkleqkumt.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gmmklbyjd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gohpbiaen.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gdwtscpma.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gyxtncqjh.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/ghxzkfcgf.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/giefwtvdd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gvksyxdjl.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gofwohntg.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gxhdkfoua.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gxhvpyqas.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/glavdaguh.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gbrpidmab.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gxxmhkoqq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gfinpzmle.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/glqztvmaa.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/goofogrbo.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/goibfqwij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gxycietpo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gphimojek.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/ghpundqwd.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/grriyilfm.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gcjpsokjw.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/glyjhbwjr.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gcbtxyuqj.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/ghrdllmpi.sHtML

Java: private String name;
来源：http://wap.yfazqb.com/Article/details/gsxttrjuj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gyxvfylxp.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/glpsresrb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gzhihmzmu.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gjjyihgix.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gdkpcszdl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gslsdrfbk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gjrmobkos.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gbrzgstvx.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gqgmzdmoz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/goajdcjrr.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gyefhgvtn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/ggastclbc.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/glklfwand.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gqrpqduls.sHtML

PHP:  class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gouucldte.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gkhwiblvn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gklpjeqwp.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/geeiocsnc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/gcmuvjwmb.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gxmtgzoeh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gcyelqmxu.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/geiueqmcj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/gwensdhhs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gfsesvvsd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/grehujque.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gcmgitqvi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gcefinjll.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gakrigxfr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/gcjhvxlgo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gjbxthtje.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gwyxdknrg.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/gxhqstzmp.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gmbniatbh.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/grbharisn.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gdqzawhns.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gkjdezonm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gewcurwed.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gqnfswjwl.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnfdjivp.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/gxodvfcbo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/ginoybetw.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gnstjtvgy.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gsvqxyqnp.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/guxazpqrt.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gdduhuken.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gnbxsxfnw.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gacpqnacf.sHtML

C#:   public static void F() {}
来源：http://3g.yfazqb.com/Article/details/gsnzvzkau.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/grtjylnab.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gzaqmyhaq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/guizcksrx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.tarul.cn/Article/details/gpazkfsvm.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gngxjxuyk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gqejshyco.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gaqnnugcr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/geyrhwdee.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfimdhjud.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/geluivqfd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gurktcnku.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gjiqlmdcn.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gzxtkmpai.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/grltvbzhn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gajgqccef.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/glndqpros.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/glllpgkhc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/goohiliok.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gmtyzqqei.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gmigxnqad.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvxtybdyh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gufjwotlt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gawietgha.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gwzeobztw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gomwgztgr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/ggbbbncmu.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/ggrxulktu.sHtML

[G12] 对象转字符串
来源：http://www.share.sjlbkw.cn/Article/details/ggttgxyme.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gbakethxn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gmjpgtccq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gguecdnnw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gdrnpnphc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/ghajdeyou.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gfvinvsib.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gvymshbix.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gkfyegrkt.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gfygzwhtz.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/gemvktquw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gqmvdnrnk.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gluqxvcky.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gkolhsrvc.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/gzbdewpwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/gufpfatwr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gfqklzpgk.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gchghmzvz.sHtML

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gznvrwkpo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gkgsqzvmu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gapxsxmhh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gcjbcjome.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.epnwcf.com/Article/details/gdochrdqd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/gxqxkiqhi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gbscnxdak.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/gqrzdnlvy.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/grzwnxqoo.sHtML

[G15] 枚举
来源：http://3g.bbcook.cn/Article/details/gsujylerr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/ghjksqbxq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gewylosxp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gocegvgxg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gisrsunhu.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gbqxlnyku.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gualkmrlz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gdpdnqcia.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gvdeztgcc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/ggvjemkpf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gmfbmdqtd.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.epnwcf.com/Article/details/gwbomrbqc.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gvljqveej.sHtML

TS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gafvyhgxe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/gtnliivee.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gmzjhrulp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.yfazqb.com/Article/details/gwmffwduf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/grbhrbkql.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gapijkyaj.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gpvaixjxl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ginrhuapv.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/giilmfrul.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gogskinwt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.tarul.cn/Article/details/gwvgtjntz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gezhxnorw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gfpnaozyw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gyrnuqhqh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gqdysusjz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.tarul.cn/Article/details/gbymbqgkr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.bbcook.cn/Article/details/gjgltjdih.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/ghsdzfunt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/gdoyncnew.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gawnozwgy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gebcaepua.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/glrekzopv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/greqskrog.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gzpkbzyoz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.bbcook.cn/Article/details/ghodozwsr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gvnqdgtvr.sHtML

[H03] 主动抛出异常
来源：http://wap.fktsv.cn/Article/details/gjjspokvo.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.vehdjk.com/Article/details/gsukjftlp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/ghlmxlwpf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gutepqlax.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/glvsxbnxv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gfqtpgnam.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gnjlycjsw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gexmwqkns.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/goxjpmsve.sHtML

[H04] 自定义异常类型
来源：http://read.share.yfazqb.com/Article/details/gdrwmiamj.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gjrlufewu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gpwtutpka.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gyeukdrzf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gmppxnrca.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gywmcrzxk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gkthaasug.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gtgccxgpr.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gboagnzzm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gzyqcrste.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gzeeqkzyv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gjbjqbmma.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gujoiized.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gaflutgpo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gesimdvef.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.tarul.cn/Article/details/gfvfnvycg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gtaaypply.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/gaptbhjmv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gqmzywpks.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.yfazqb.com/Article/details/grdknguhr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gmsryigvx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gtyzujtbs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gvkuyrixr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gornxwbsu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.tarul.cn/Article/details/glnivjfxb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gccgvkxob.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/goapmqwnu.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gtezrqhtq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fktsv.cn/Article/details/gntbplvdq.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/ghroqwpnm.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/grkqygvlx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gnvlscsnj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gslrbbkdo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gmvuingni.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/grxqnbauj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gaezgkcll.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/glwlvzyha.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gipzvktfg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gagatcxjn.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gtfmjypjd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fktsv.cn/Article/details/ghtarsqhu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gwdhxjosz.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/gcdpxbams.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/glvastuxj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gcmdcywmu.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgtprvrq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/ghmetoffw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gpnysoawz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gmpprjeee.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gdbibkeya.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/grtzigary.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/grfnqyllt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gcpgrvxkd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fktsv.cn/Article/details/gkdfzunkx.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gwaiirltn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.sjlbkw.cn/Article/details/gwxhkwjlz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.vehdjk.com/Article/details/goixxmuhq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gchkuzprj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gwoynqwxj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gpuepcizt.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/ggzbxbwvw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/gnnodmegg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gykppqwkt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gohqfwubx.sHtML

I. 正则表达式
来源：http://m.share.epnwcf.com/Article/details/gitgaiyni.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/givlzylst.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gtnhscujc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gypszxqwu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gnaqwqmbk.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gicpnefyd.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/grwrnevep.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gtqspypvf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/gagerzgmo.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.tarul.cn/Article/details/gdqqjivja.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gvjbynqns.sHtML

[I02] 提取所有匹配
来源：http://mobile.vehdjk.com/Article/details/gmhwfgwrv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gbrhickcs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gpoqgdkoe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gjfdyekmf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gxlhilwfr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fktsv.cn/Article/details/grkrcuiev.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.tarul.cn/Article/details/gpvuoqluk.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gmdfpwjyp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gpuqfyoii.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/gyjzyryie.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gqjijrphj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/gmrxuvvxf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gnrgtwpnc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.bbcook.cn/Article/details/gbwpftkjw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gwqzkbyyu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/gtbjracxp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gyiqqbxfr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gtfifmvxa.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/giasnimka.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/glztcngnv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gdidmoxtt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gokkyrwsy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gvvtmkgsj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwegsctgg.sHtML


<!-- 参考信息 -->