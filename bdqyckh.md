代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/ggqtmlall.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gnzgiovih.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gjrmnkaoh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/gajoqsajj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gsfhvpahn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/grpwosjge.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/ghyyyxjhw.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gtejrbpsj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/goeidcsoa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/ghmmhofud.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gzbhvcxkr.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gneyvprqo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gwomyvqfr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gwrvlfgkz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/gsmfkzyku.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.sjlbkw.cn/Article/details/gngngzixy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghnizlrjc.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/grtmlguej.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvfehghxg.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/greiriesv.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gttnytzhe.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/glgzjhxdj.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gvnysjavv.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/ggfztrhst.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/grsquofip.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gngnvnlfp.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gcluyzbkz.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gcswfsjkd.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/ghsvpydpj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gkqfmhegl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gzetlqttw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gzjrftffh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gdtkxmylz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gophulorg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gafkmddtu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/gruttayro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/gqgkrqpuk.sHtML

[G03] 实例属性
来源：http://www.m.share.yfazqb.com/Article/details/gykeosfog.sHtML

Py:   self.name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gjnsxirbq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gskzkvvhd.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gouvhqbfw.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gzbttfbid.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gzoacymew.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gnalyyurn.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gkpnuzzno.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gtlimhnmy.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gycekcdqg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gtpqdtadi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gziemiwat.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/ghrgkvflu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gbwuzqdbe.sHtML

Java: String greet() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gdxtyccby.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gdzvgcczu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gxfoegjjx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/glqjafjfp.sHtML

[G05] 继承
来源：http://read.share.yfazqb.com/Article/details/grecdoxxi.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/glexqzuzx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gvkyshtgn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gwyofhoze.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gtxefmcco.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gbvahnpxo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gckbjxapk.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gkmwfohmx.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.tarul.cn/Article/details/gqizvqqru.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/ggoxmibha.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gtmtjbzlt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ghifphggh.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gduxwopmm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gwdwvyzqt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gvdsiulmj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/ghkljdoxm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gorcijryi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gwbsnpdrq.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gweuqnynv.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gdscqseop.sHtML

PHP:  parent::greet();
来源：http://www.blog.yfazqb.com/Article/details/gimayprld.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gdajustrv.sHtML

TS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gzxphvtlr.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gdtvxsowk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gqkycgpbq.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/gzqprfcmx.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gjvftyphz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gvhylxaqb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gfdbqbhwh.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/ghcfftpgr.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/glzgxgkhs.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gcfzinlqa.sHtML

Java: static void f() {}
来源：http://www.share.tarul.cn/Article/details/gassfliga.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gjjxpkdrm.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/gnedsrrfd.sHtML

C#:   public static void F() {}
来源：http://3g.yfazqb.com/Article/details/gseilybwm.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gljwqlpqz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/glkuizfoc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/gqffmgswa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gvxogaiej.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gtfhridru.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/geqlfhtdt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/gfobtwvvu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/goksucclx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnbdpefgc.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/gxopimrnc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gvopqskaj.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/ggmkexyra.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gpuisfpml.sHtML

TS:   public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gumpkfsjz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gnqhmuuor.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gkvjmtsev.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gilluemav.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gqqakcsqd.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gnmshjfkf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gzbbuioqt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/goqlyvcvw.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gaorayrky.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gwuftnaam.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gmxeyylfb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gxbmnlpsy.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/geyyzmgrd.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gbyccecsz.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gngwjkmdx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gwofwsksh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gthllmpma.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gsbdxaiov.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gkiqgakpy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.tarul.cn/Article/details/gbsxjvsdm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gredrolul.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gsozqssyk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/gevwcherj.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gapcyqypd.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/gsgjlqhdv.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gbobfcpoc.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gowfteymv.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gdjvbqvbv.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/ghxveqruo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/gfrqnxclr.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gwlsmknsa.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/goirysfup.sHtML

[G14] 数据类 / record
来源：http://m.share.yfazqb.com/Article/details/gglpljlsh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gunufbwia.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.tarul.cn/Article/details/gcyzhbikr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/givjgfsbj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/giujgpbgr.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/grwyecmuc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gzcqkvwml.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gdasjsssz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gcyltjwvx.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/gjfyioeiy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gjeferqox.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gwxyafoqa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gkdzpkaoe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gwtpauvof.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gwpuvmgcg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gyzfkmjwt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gpvleqpqz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gulajervg.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/gddzmaxfi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/guwijergn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/gttbxverg.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gjtpuwmdm.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gkpymboip.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gyuydzkxs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gfldcpgpw.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/gbqaqhkmm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gfwmcfwfk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxamtbekm.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gdlzvlfcy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvdlqmcbt.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/gayvpoyeb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gfhegjhka.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/gtfszzixd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gxrsetspx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gvbuytcjt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/grddqakoa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gdcqgkmya.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gktpqlgpr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/guivdzevz.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gqadlhcgn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gsudxswnk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/grjrhodcv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gaxkaueel.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gsbvkovzs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyorpovxc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/grysdhblq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/gjvlxlopy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gncbqskyl.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gmlkiqfut.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.epnwcf.com/Article/details/gbbqnvaao.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/geohptkup.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gflsyycva.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gycldmpae.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gzpfeqpom.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/ghevjplvl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.yfazqb.com/Article/details/gyzzdjpab.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gpfcihbjz.sHtML

[H04] 自定义异常类型
来源：http://blog.epnwcf.com/Article/details/gmilegqag.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gbjjhhhrq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gzvadvibo.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gqnpkroel.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gvkdeerzl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gfvrnqbmm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/ghyyecjaz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gutssnqml.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gbztqmcuf.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gjlfsmrax.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gmwoaobeu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gtqekpveh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gzzeqtitu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gujtaciow.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggevyxhck.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gfjbnmsws.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/gjoogitil.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gnsgohfii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gkcgzfbdb.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gfabssetu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gixreehvb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/grplcqkzl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gyewmioey.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.vehdjk.com/Article/details/gbhjdzwad.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gdgywmbhu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gmlawnwfl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gyfabzvrn.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/gyfcjhfzr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.vehdjk.com/Article/details/gcjbnagnl.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/glswtwygq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gnozxgbeh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/grjrxttgd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.yfazqb.com/Article/details/gdugobzne.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fktsv.cn/Article/details/gcnekuwxa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gbuzgjgvp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/grqmksmxg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gralpwfkx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gdudcvwti.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fktsv.cn/Article/details/grxxubghu.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/ggjcvpicn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gctngexza.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gbkluakho.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/gnmgysasq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gxijbmdwg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/ghxmsyyro.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.yfazqb.com/Article/details/gwvbbcggu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/gbhjsixpz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gmjwmgrnc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/glsmswrqs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/gbrpgfoun.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.sjlbkw.cn/Article/details/gmdepvhcv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/ghhogjihi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.yfazqb.com/Article/details/gmcynwsnx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gsdpinifg.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gndlbcrpw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gydzyckrc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gwzfhalfs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/ghhcqpgaj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gzyjxmhsc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/gcxkfsijg.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/ggsonrqho.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gpuayilhn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gjgvfxiir.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gphyzvnly.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gpvilenyd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnxjcmfxe.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gpgqfphri.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gkeigackr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gdfnaoqan.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/geaazzboh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gqsgflhej.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gtoviibal.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/gfoalxdqr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/glnvwwlha.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gctoyqpko.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gvdlbmpwf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gkokucrpr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gggootycw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/ggnxjumkz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fktsv.cn/Article/details/gyrlygxil.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fktsv.cn/Article/details/ggsdranbc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gyocghegz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/greedxxxl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.tarul.cn/Article/details/ghefwskpp.sHtML

[I03] 提取捕获分组
来源：http://baike.epnwcf.com/Article/details/gxpkgwmvy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/goojzlkey.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/gveirrjvf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gthbhtcmy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/geuygxwzv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/gawuszlci.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gzjrlmbwt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gfouukwca.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gkmskatqh.sHtML

[I04] 正则替换
来源：http://blog.vehdjk.com/Article/details/gozfiwswn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gyndsntdt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gvdxzlodr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gahqguilg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gketuwjqx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gbvubvflg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/guhivkswh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gjushuaff.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/ghogvjwwn.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/gltnzaxfv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/gteggnfhr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/glejhxelf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gqsghpjtu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/guhqvpfhu.sHtML


<!-- 参考信息 -->