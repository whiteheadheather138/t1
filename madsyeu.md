代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gywwgkovp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gvndnhaxx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gbtpbrvsa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/grdmtashm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghaqssnln.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gbhhgaezf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/gnizclupd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/glkfsxgsr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gjryyqsap.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/ghlrzxkhw.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gvcqmljzo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gvknxqnfb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gmhjcbyio.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gprvgjeud.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/geofklrby.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gzwaelymi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gigflqiim.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/ggbkhkwam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/guhhjzdjw.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gqklnjhkq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.sjlbkw.cn/Article/details/gjcrxiwyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gdnzhyhwn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gcyvatrzn.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gpczngmpu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gxpvvvjmm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/glrguerim.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gvlwowlbe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/ghibhnmbd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gssaaskag.sHtML

G. 面向对象
来源：http://read.share.vehdjk.com/Article/details/giqptdefn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guvejxvak.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gtltmtosn.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/geujfbprv.sHtML

PHP:  class User {}
来源：http://baike.tarul.cn/Article/details/gucezgyei.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gzalheplm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gulicbymi.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/gbwgqmpky.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/grqxvcdja.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gajrvudiw.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/gutmskghk.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gbyqaamwi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/goyluupax.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtizuskhb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gsoqgxlpf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/glyqdmxxz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/goaquxcxr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/gblktcmqf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gllddjvqw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gmdnrihdp.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gzcbzujjm.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gtcunpmst.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/ggjfdqmpr.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gyklwjqqo.sHtML

TS:   name: string = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gdmykuhlv.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/gsbvgrkpo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/ghorydowt.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gcildkpdz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gyuxcuwfa.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gxsocztvk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gxxnoxddj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gcxogcvpt.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gjhaqfblt.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/guimfgjfg.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gicbzdbbe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gobedmevf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/ggnbovzdt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gmfyndcir.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gjlivnrdk.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/gqieoqfqc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gvuqvtsyv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gfsyhfipr.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gummgtbwn.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/girhqnrhe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fktsv.cn/Article/details/gjjuuroic.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gwaismczj.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gjlkaqata.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gtpceumrb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/gcagazcpf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gmdnbmblk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gvhachrxy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gsgpdrqom.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gmnowsbax.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/glkhwrmpu.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gksfpfkla.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gkqacjbgf.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/ghxxiakfn.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/gddjpbviz.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/grlfnzdkz.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gkuvemakx.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gevdgexix.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gmgvptrml.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gvejdxjua.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gojvvgwum.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gggnhpkrv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.yfazqb.com/Article/details/gaigqbqef.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gbougooat.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gzxhmwrkx.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gstgeqwaz.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gyxndlqer.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/gpdqjeopw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gckdsetmr.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/grteubzqg.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsxslksf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/gzbjkiofy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/grvbptmdv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.vehdjk.com/Article/details/gfneifkrc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/grpvhzhtd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gdctafjqg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gnpyullqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fktsv.cn/Article/details/giwxdchzh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gobgqmayn.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/grnkiblhi.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gkbvnojeu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.tarul.cn/Article/details/gxdgmszmz.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gseasnhjh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gztuyfejs.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gxbnnqlzd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/geoyxndzo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gdvdfegir.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/grwqrxwmo.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gyoripvlg.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gzzhpsyat.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/ggyvratxa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gvievctot.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.tarul.cn/Article/details/glrcluoaj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqphngoug.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/gbaoqjqwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gjfbavzbj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.bbcook.cn/Article/details/gtigmjlyb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.sjlbkw.cn/Article/details/gxvnonsie.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gdnoiuuaj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/ggowxkofl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gcnwvbesa.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gushjpkmc.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gfguzyamk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gellrjrcb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gzhwhyafb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gcelgpvai.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/ghghirbkl.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gortndaww.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gwrkolaun.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/grihbjuva.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gmqcqcdzy.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/ghwvvpbeb.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/gpvpeidbl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.tarul.cn/Article/details/gxhktgouh.sHtML

Ruby: u.is_a?(User)
来源：http://3g.vehdjk.com/Article/details/ghvjajvkp.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/gupzzctfu.sHtML

[G14] 数据类 / record
来源：http://read.share.sjlbkw.cn/Article/details/gtzulecar.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gxumtmbcq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/gnfsalbyj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gpgdwqzci.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gaimxdkgv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gruqirubf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/ggxjouuso.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gsvdzezrr.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gnkvgoizu.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/goshhbthx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gpjaptani.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gkcvjpzhn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gkoirsmzy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gzybqxiij.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.sjlbkw.cn/Article/details/gxeblkkou.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gptytpnkw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gwcmhnfnx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gmowilwqg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/golvrvmkx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gteupbudx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.epnwcf.com/Article/details/gavzqlijc.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gltwekqrg.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gfwslkade.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gbqppuktq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gcskkbryp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/ghajwzguw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/ggusurbaj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjcnfcqmh.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gtmxzcsde.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdzynzqld.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gxgddrskg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.tarul.cn/Article/details/gtxqvbnzi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/gideychwl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gwlmpsapt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gnygxorrl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gwdtzlpig.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gahibuzfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/gvsetrrtk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gcngpqxwi.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/gzxaygzwl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/grdwikxzf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gwyszqvcu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/giupxfgdx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/glcklxoho.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gohugfejc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.tarul.cn/Article/details/gtjugqdjb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gzklmvshn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gymqfzdjl.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gkvettaly.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gibcqgjmu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gfttrmdgi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gadstomcu.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gnprwuvxt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gvlqxmgke.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gleogmzvr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gbgrbcwfh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gifkitcqc.sHtML

[H04] 自定义异常类型
来源：http://www.share.yfazqb.com/Article/details/gqrvslpwf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gmxipcsxj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gaifyvjkk.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gbdxyaroq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gwpboosqa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gqaamrrxp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/geckidgzm.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.epnwcf.com/Article/details/grfslxcjh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gdbshayhe.sHtML

[H05] 捕获特定类型
来源：http://mobile.vehdjk.com/Article/details/gqkhzeuzy.sHtML

Py:   except ValueError as e:
来源：http://m.share.bbcook.cn/Article/details/gehfidknb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gleaagzop.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/ggtjuwsrh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/glgdsgoxo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.sjlbkw.cn/Article/details/gfxuhxmlo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gjeetrqdm.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gilukyurb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.yfazqb.com/Article/details/gbwmgjkxi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbubybsv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gtcecsdne.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gpqztozon.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gydovwxpq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gxhikqzne.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/gtkprvfap.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.tarul.cn/Article/details/gpndsblcs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gaxkfzmau.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/ghkjudnmg.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gliphaive.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gezorywzg.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/grhymajxv.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gnutfegnx.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gzmsxupwe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gkcsnpkmf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gngmaqadd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/grsfkjcko.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gqgeealvl.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.yfazqb.com/Article/details/gztzgpwus.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/guwaovddw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/goibevzhf.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/ghybftmsc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/ghumfnqoc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gwbfogaji.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/gmaruvehc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.vehdjk.com/Article/details/gsmzajvor.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fktsv.cn/Article/details/gtzvtrlsi.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/gkwtyivwc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fktsv.cn/Article/details/gxdtmmfeq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/grubunepu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/gcdwpbtev.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.bbcook.cn/Article/details/gsvlslqcw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.tarul.cn/Article/details/gopwxgooc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/grvziwmux.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gqtztawkx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/gncddfuxz.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gizsrypwd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/grfdolpoi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.tarul.cn/Article/details/gugjfspum.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gzvhqbypc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gluvpubqs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/gbsullsfo.sHtML

Go:   defer f.Close()
来源：http://read.share.epnwcf.com/Article/details/gwnuvyhbs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/gearfseew.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gynhcymdf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkpjzgbmi.sHtML

I. 正则表达式
来源：http://wap.yfazqb.com/Article/details/gzcelwyby.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gislwnivi.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/guuokpyxg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gxrogjqui.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/gigicpjcv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gzlkgtqvq.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gueuggisf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/grgxpdloz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gqjyknugc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gqopfrktr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gtyfxpjgq.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gxynduwlg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gwuasoidm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhggwowh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gwvlabkwd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gnmewiwmh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/grqklirun.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/gjsjhjtfz.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gxkyxbnlz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.tarul.cn/Article/details/gvsqgfjyq.sHtML

[I03] 提取捕获分组
来源：http://wap.epnwcf.com/Article/details/gocdzdbkw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gpsdxmniq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gzguoljml.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.epnwcf.com/Article/details/gqswvafqk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.yfazqb.com/Article/details/gmirfjplx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gfqtripby.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gsjkpgaqq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/gtbreudtw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/glofgultc.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/gpazysdvr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gsqhjavjw.sHtML


<!-- 参考信息 -->