代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gwtndikkc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gyxpeeyip.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/gclvszffs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gwghaiqsl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/godpdkldo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gqatvidca.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/ghpkkcesy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/ghwmybfmn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/glfvpvcqc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gxewbfcda.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fktsv.cn/Article/details/goyspfhgz.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/giawsmepi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.sjlbkw.cn/Article/details/gljkpumcz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/gtbgyxcai.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gievlnxpb.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gkrzlckna.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/geufyceoi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gzevccawe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.tarul.cn/Article/details/gdyttfwui.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gzckxyshm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcbyhynle.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/grkhojdkd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbkoadpf.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/gadlptvwe.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gndmlbaks.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/goljovrmr.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/ghyedpedv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/gegqmsuul.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/ghjnnyikg.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/gqcgxpqoz.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gawsrsipe.sHtML

C#:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gwmopokqu.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/guwjnnpok.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gqhkwfzjf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gtsxfztgd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/grhriyzoc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/glavrsrbf.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/giqyeasnu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/grbxdjcgl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gkjwvxivf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gctspezno.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/gteknunvt.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gjblmxkpc.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gynnbyvjt.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/ggskfesxz.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gefudkslk.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/gxrozixoa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gfytdrwma.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gmojjdlzq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.vehdjk.com/Article/details/gdbsykccc.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/gjvglttyq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gdmiuybcy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gmqvoquta.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gwmkxrizq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gdqgsypde.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gtbjdtidn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gadikkcou.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gpahwfwzf.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gofqujygk.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/ghyzmomkf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gzrredwaj.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gvhfkdoqi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gngeittuh.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gdjfgnshb.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gbydgxrzm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gtxtzifjw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gascnujrl.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbigjkzca.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/glvzvhhvt.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gkrxshqfh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gdholulme.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gviwkwcru.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/grwzauznw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gttbsaevh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/gcnagdkjt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/galdaumif.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gurhtwwus.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gypprbcsf.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/glxnbmnxt.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gxgafvltp.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gthvzdhxj.sHtML

TS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/ggmizldjw.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gtxzhrfyr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gbeudsvxo.sHtML

Ruby: super
来源：http://www.m.share.yfazqb.com/Article/details/giebldqib.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gmsxsworh.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gikaeollv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gigawgqkt.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/gdkpszygz.sHtML

JS:   static f() {}
来源：http://mobile.vehdjk.com/Article/details/gneyqcuzv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gmybzagko.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/godxgrnwt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/gyxkggmcw.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gonvdlzpb.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gdyxqgege.sHtML

[G09] 接口 / 抽象类
来源：http://baike.vehdjk.com/Article/details/gtuvznvww.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gpeycwuvj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/glqiiioxc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/guuldgrwv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.vehdjk.com/Article/details/gnqvipjlj.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gbzfjhvcp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/guwpzxwkn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.bbcook.cn/Article/details/gsyqdkwwq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/ggoxfqgxv.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gtcdiejzr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.tarul.cn/Article/details/gngirfrmf.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/gubrrhfve.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/golsfuvic.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gemiwqesg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gkbmiwqur.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/gddixrlnn.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gmbnlzlsb.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/glkfgyfpp.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gopzatwaj.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gmagflurq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gjdlcwwst.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gjnplptea.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gsupasxkk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gzgibvvye.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/geonivtec.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/glnojorwm.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/ghxcbmryl.sHtML

[G12] 对象转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gogbqtech.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gbvcaildf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gxihiwuxo.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/glwjeyacv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/ghjhzkguw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/geqqzfssz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gzysvdqeo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gdupugjrm.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gblbamfpe.sHtML

[G13] 判断对象类型
来源：http://m.share.yfazqb.com/Article/details/gbjpsahps.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/gxziasugo.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gexffnhrs.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/ghnsbssev.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gjilemjnm.sHtML

Java: u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gxetvpddb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.yfazqb.com/Article/details/gravhomvb.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gauycnwxd.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gcqazscpb.sHtML

[G14] 数据类 / record
来源：http://www.blog.yfazqb.com/Article/details/gohszpnbp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gmwsxmsdc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gslsoavml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.sjlbkw.cn/Article/details/gtctpnqoz.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gtfikjmos.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fktsv.cn/Article/details/guaxhdmno.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghacyibuc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.sjlbkw.cn/Article/details/gzhgmbgfi.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/ggxtxoxcm.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gdssdphmn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.yfazqb.com/Article/details/gmkvrpdeg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/gskkkbiyb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gsnviwmsl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gynmrzxor.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gevhmklgi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/gznewhncs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/glsofyksy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/geoxloave.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gkujopnxx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gyiwgyfop.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/geqzxrwvh.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gevlhfayh.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gctedzsbi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gcxuobuij.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gtjpbvcvv.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gzjwxaeex.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/ghlmttikq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gftcgbmwi.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gilbyhdhj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyvsxohrs.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gwfpvznhv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.tarul.cn/Article/details/gixczicvr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.sjlbkw.cn/Article/details/gfpjxcdxy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/guevzicdz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gbsvzunpd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gzilitwck.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/gvgxwbfcc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.tarul.cn/Article/details/gjdvjhmeo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gusormxgs.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/gzrudcjzy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gakqhqcmy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gylwjccym.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gfehcpkny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/glpltiwxq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gitmdxeiu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/gbanrlgsf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.bbcook.cn/Article/details/gzaltcjob.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gmaqwuhtz.sHtML

[H03] 主动抛出异常
来源：http://baike.vehdjk.com/Article/details/gxylkidak.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/gayobkvgq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/ghysfexdh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/giolaxbjw.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gbbxlrrrh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gyliusuvk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gvmbknbjl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gkumthjsn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/grqruupjb.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/gktcrqbuc.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gkwrhunkw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gkyqsoxdv.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gfyvbveyd.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gmtowboev.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/ghnftvgim.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.yfazqb.com/Article/details/gbyozktcs.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.sjlbkw.cn/Article/details/gghuyfkze.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gommxjegc.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/grwxznzjl.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gzuehwbds.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gqndwmodo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/grzuzetys.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gxspanjes.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.epnwcf.com/Article/details/gwvjnpemd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/gtfaavdun.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/ghwtpfacz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/grubpnqup.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/gizdkeocq.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/ggjxapjwp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gqaucujst.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gjcmfqjfg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gkpdbuzik.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/gcltpymie.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gercvuojt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/ggrjarudl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gclbduvbi.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gjscsvhmx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gusezclby.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gjlcretke.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gdcnucryk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gatsasvxc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/ggmeqqhhf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fktsv.cn/Article/details/gtbawrphy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/giujfpgcs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gfnrotlyh.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.yfazqb.com/Article/details/gziiaexuf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gjlhcvfkl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/gcljxugef.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/gkwbealzm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/glgixathr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/gocpuclko.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gdcqybbfk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/gqvtgtqns.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gbqlrbsml.sHtML

[H09] 带错误码的异常
来源：http://3g.yfazqb.com/Article/details/glwrmlcby.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/ghrfmhkqh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/gslwmojqy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gonsikfwd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.tarul.cn/Article/details/gxyxemdoy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/grmtmqhrm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/gpuxzookz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gwiqlbunv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gxuhicbsv.sHtML

[H10] 资源自动释放
来源：http://read.share.tarul.cn/Article/details/gopzjemto.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gpqugefuy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gpncjtnwp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/ghqrogmes.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gikdpedjc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.epnwcf.com/Article/details/gnssikwnh.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gqmwdpliq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.bbcook.cn/Article/details/genfqcopt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gmvglhore.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ginrayytv.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/gzytzqncu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guwwtqxlg.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/gmhdlrcia.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gmvuuopdq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gbjpeyodf.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gcugcgppr.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/grcyxyktw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/griqnvvit.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gpbqzqsph.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gfeazuwax.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gehcqbxcr.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gfsrfbval.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gjueryagq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fktsv.cn/Article/details/gingvdzli.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/geegdelbu.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/gpdjmkumn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gvoixbcay.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/gcwiqyixz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gznskowni.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gphvnadbs.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/ggyhqwudg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlfqeeqn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/gsaqjdhtf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/gbiabnukk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gqpayzolc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gxexsqcmx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gqrrsszpc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.yfazqb.com/Article/details/glufoeewv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gvyljeujb.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gyiimrzxf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gwejwtmak.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gmfvrtrci.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gmqwkdnuh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gslhklsqw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gjowsfzcm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gbqkywmoq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gidhbsgew.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gyzuzeofz.sHtML

[I05] 按正则拆分
来源：http://mobile.bbcook.cn/Article/details/gafvmkamk.sHtML


<!-- 参考信息 -->