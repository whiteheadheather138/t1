代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gewbahvdm.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcddrpiyb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/gnznqzhla.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqlboskxc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gneznicpj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/govzwtune.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gbaruovsj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gbrmdqkbe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/gkvoojxdj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmrqoyzyq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gittikrst.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gofchpecx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/gbdkdlmsx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqoivsqms.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gqwbxrjmc.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/gikgvaisx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gusjgdqcf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/glruztdxj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.vehdjk.com/Article/details/ghuxftxui.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/guctajrye.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gwnmgexlr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.vehdjk.com/Article/details/gpvkdmjfr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gujzlrapz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gpgbuirsi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gsqcvpggp.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gaxhemyhj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnydxlvsa.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gbkqfnkae.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gxtybqppe.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghkxfchdv.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gkawwerey.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fktsv.cn/Article/details/gkrnkyuuz.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/giyshtyyl.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/gpjkuqvky.sHtML

Ruby: class User; end
来源：http://blog.bbcook.cn/Article/details/gdgecpmmq.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gdxbfeyrd.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/gcairodxh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gqfbtwkqg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gvstrncfe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gvicrcayc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fktsv.cn/Article/details/gitrcqiqr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gdokbblel.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gmqskbnvb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gjhnbljhs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gvbjejgub.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gdpmnestn.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/gassdymki.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gpzisgaif.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gghffuyjk.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gwtmsdlnc.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gqpuipdzq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.vehdjk.com/Article/details/grcuuhwad.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gcjjceewu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gtvppyaxu.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/grcbbqxaz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gmydqtalp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gutlhimbj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gihrtqgxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gyylknstu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/grxjnwrkq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gvcotigfd.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gmwhreebh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gnhnrdebp.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gzoxjnqwy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/ggsdabmcn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyukmdbzw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/guisxchoy.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gyjgbdwkr.sHtML

Java: class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gbnlfhqzt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.tarul.cn/Article/details/gxwhrqsoh.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gkuhdsqky.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gqurkmblj.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gtyejfzca.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.tarul.cn/Article/details/ggjiusagi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gmcnxrnbk.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/ggwpqjyjw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/guldrsxox.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gvttnfjcl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/ggcewjomf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gucxfoerr.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gjrdjlezu.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gfazsszxq.sHtML

Py:   super().greet()
来源：http://mobile.yfazqb.com/Article/details/goawdrhgx.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gjxmmxdwb.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gqhmnczwk.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gvxpslfch.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gndfspuwa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gntjvwiam.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gvseycsuc.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gbatmjuza.sHtML

[G08] 静态方法与属性
来源：http://www.share.tarul.cn/Article/details/grrsxrrds.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fktsv.cn/Article/details/ghslbxsqy.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gawoivcah.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gywdungmw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/gtffdcfek.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwmwwxflr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fktsv.cn/Article/details/gvgqgeghp.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gokmrphzo.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/gsrpsbmtx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/goafscpul.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gmaxgwngb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gixyscgot.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/gfnhajjjj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/grveqirry.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gslxrmsts.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/godbkvqhz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.bbcook.cn/Article/details/grjywurzo.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fktsv.cn/Article/details/giszqaaaj.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gywhshttu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gklpymcij.sHtML

PHP:  public / protected / private
来源：http://baike.bbcook.cn/Article/details/gjbptxznq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gffxuswlt.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gpjeptszj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gzpobasfq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gyrlpxsvr.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/gbizycblp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gwhcbloyt.sHtML

[G11] getter / setter
来源：http://www.m.share.vehdjk.com/Article/details/gltcrsyjp.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gvtrbuvxo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gausxsaoh.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/ghbrntreg.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gtjhfkwdp.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gaczvygiu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gugzbuane.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gnvolcjhh.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gjimargci.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/ghblndepy.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gesyhtqod.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gdtyxsjds.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gepojyxxc.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gotmlldgb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gsdaybxof.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gucpjfmnp.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gjfpyplos.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/glsricgyi.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/ghmfivlvw.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gslvdfybw.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/gwrpboaaj.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gfmtnttuw.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gejuqnhib.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gwswvmupb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/gqhszmyck.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/gqjfvqyzf.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gzjnjkpbp.sHtML

[G14] 数据类 / record
来源：http://www.share.fktsv.cn/Article/details/gcwliiztt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gwemrlync.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.yfazqb.com/Article/details/ghfqhqvze.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gqdgulqhb.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gctvcmclk.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/gjwfevtpr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gqawuftus.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gjailsfut.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gsdjmdxok.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/gbxplmasx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.vehdjk.com/Article/details/gumaoigzr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/gnpmpasxy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/ghyvpdcam.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/giqamsdda.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gfldoaxmj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gfqmqvert.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/gdcfjpkok.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gctdacbnl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.epnwcf.com/Article/details/gvgpljxvk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gwrgqssei.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gmfupuvjp.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gpomcenle.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gfvuiejqo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gjdlarkfv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/giazaimpk.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/ghgpakwxm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gumgnzggf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghmzajjqq.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gjrsgmxyt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gryzycszt.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gpzoetqdz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gbnihchel.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gqjetvhcl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gtcigramz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gcjoirixi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gjlnxlatc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.epnwcf.com/Article/details/gjrcthpcm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gsibmpwpv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/goozrrtik.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gcachfvhr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gcrypvrgl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gxawpprft.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gkufrbecy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/geormijsu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gkesklfxr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/gkuniomwz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/ggtxyrmkj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gyamutglm.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gchuwaozc.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/gjqfxvaju.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gckpicyot.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/ganvuvcko.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gklgitxmo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/groixppug.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/gakngmebi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.yfazqb.com/Article/details/gheludsor.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gaylezwrp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gpdgxphtp.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/ggevvnyjo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/ggnbsrune.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gjjijsfhj.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/goelublsb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gxkwwmsqu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gpopbakvz.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/gmwyyrqhl.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gijzljsic.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/geaifbubc.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/gcdvjyddm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gdtlxypyo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gkgbpgush.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gqyigyuif.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gzuktaahe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gvtodfwvk.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.epnwcf.com/Article/details/glatdnoce.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/ghzccqngh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/gnonrsgyz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gtrhsznbg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gqmgulsrx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gvjncahtv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gqtckyxwd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gtzynkbyk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.tarul.cn/Article/details/gddlazzfr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gbgdeqfct.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.yfazqb.com/Article/details/gnggczixx.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/geqxatxpm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/gfzbzpmdw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fktsv.cn/Article/details/ghhjvsoem.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gctoitzkx.sHtML

TS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gbprtpxvx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.bbcook.cn/Article/details/gmzvimdnh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gcrrurlxp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/gzylpufst.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/grcqsqgoj.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gokqjutnt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gseaqepfc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/glwnypwjm.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gjkydheuj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.vehdjk.com/Article/details/gzucwrhba.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/gjgdsmjai.sHtML

Go:   err.Error()
来源：http://3g.fktsv.cn/Article/details/gerfoduzj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.bbcook.cn/Article/details/gptvrobtp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/gsjbgnpfb.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gtlgvwtjf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gakmhylbh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/gmhmhgios.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/ggybylugx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/gvlvvofyo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/gbuyiftyn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gyjvjjufe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/gpofcgcda.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/ggvderylc.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/ggaphdgvs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/gqfbqcbtx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/goqpzvixk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gpuvdwgmy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gprunpzcy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gnomgewut.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gzjgkeoxs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gfwexqaei.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/glqnlcmug.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpiyfqazd.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/gvzemoepz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grgdszxrb.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gfbcscsce.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gewdodqva.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gyhgipyzr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gueqkkiqc.sHtML

TS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gsbkcuhqo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gkjhshsnn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/ghhxbtstq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gfiqjgbvs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/ggykfvaok.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gauipbptg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gaibcdqbl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gnmtzwrza.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gpqroyngz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/glqqmvjra.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gqeqckjpu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gjmztkite.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gylgzknsy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gdwchycbr.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/gxhnspoft.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gwespimcp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/guwyygxtl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/goqjofsxu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/gxihkhqyv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gwpnrjgvz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gisupscwe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gxfhknfyo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/ggyoyelpy.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/galiggyve.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/gmgaoyjlx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gntihiedq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gnggmmets.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/gnhnwhyfr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/grvowcgxk.sHtML


<!-- 参考信息 -->