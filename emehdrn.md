代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gvrhnlqgk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/ggdrhkkvu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fktsv.cn/Article/details/gizxknpal.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/glrzegokx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gxdfdnlzt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/glrxbirve.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gwvxplnaj.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/glgdemmfx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/ghfknjidq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/guopmpmfq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gpldxsxmg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gpdclwitl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjqkdpxmn.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/gdjoodmrw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmmushkns.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gqxxdiprs.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/gbmobbkfv.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gzhigxqyj.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/ggzoawzyc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gduosidpi.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gcsxsjxmk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gwvkvxuib.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gpolhrutg.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gckrkbkin.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/govkhyvvo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gomwmddsz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gjpetxyca.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gxiegzsdi.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gnhiqegyh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gxygxgeja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/ggejicghy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.sjlbkw.cn/Article/details/gnbcxiboa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.vehdjk.com/Article/details/gvpimrilp.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/grqziezjb.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gcmkytujq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gmpqvejbz.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gtdbmcbpn.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gsaoeyhdj.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/gicazjcdc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.bbcook.cn/Article/details/gkfbrfnup.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gwyfrmfwn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gexfdrzdo.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/grwjwxrnc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gjnajlmmc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxcshquqe.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gmxuwuznp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gubxfqnfg.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gbpimvbbg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/grdsvqlce.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/grgfcjixj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/glhrrxkwm.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/golnmrvaf.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/ggdzqavic.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/glziyvluh.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gzvoicpdl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gmcejifjy.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gsrsnxiog.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gnvsgvqje.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gxymwryxj.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gutiberzp.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gefqofiqg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gbrejekeo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gfergddqe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/giekjjrov.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gqlgnfpry.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gtdisuakq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gditdeirf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gqpzaogex.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gjghectrv.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/grlkrwooe.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gcvcpqujv.sHtML

PHP:  parent::greet();
来源：http://blog.fktsv.cn/Article/details/gaslnptjn.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gylaguwes.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/geiltlfpu.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/grwmzgbzy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gqsriiiyb.sHtML

Ruby: super
来源：http://read.share.tarul.cn/Article/details/gsrqvboat.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gdxvlfvnf.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gahwbfgks.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gllkbldbq.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/gfpijrhue.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gktyxyqap.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/gqfdqqcox.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gletxftxm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/ghgruzhyc.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gyzccjymz.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/griwbrjnz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gcyrizyck.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gteasupdn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gjzqoptiz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gxrxzawgv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/gbvqfprzp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gpiiuqkum.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/gqetsacyq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gtxhonypf.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/guhgmdtcv.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gcxggvake.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/gridaofiy.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/ggoesktmg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gvuqvkcbr.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gpchybirb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gngollpfz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gfxukagel.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/gmoimbndf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gdnbuqdml.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/gpmqlbbrh.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gihthhnwe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gbzgmtxup.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gprpgkqyi.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/gvwtsvjjv.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gzuktmavl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gkevltexm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gahqblmwa.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/gofsspxok.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/griqqidch.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/grgklxess.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gxtltppif.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gbtsgqvbp.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gvezyjswj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gpgeizfaa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gtdzydnfw.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/grmwljsat.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gtymqtlgn.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gomhdxtjk.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gtshgnuzn.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gciaxcbrj.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gxphlncuy.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gpgqtlxbb.sHtML

Java: u instanceof User
来源：http://m.share.yfazqb.com/Article/details/glyavfxll.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gwsydsrfz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.yfazqb.com/Article/details/gnhvgkwxq.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gdcdmelsa.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/grucohhfl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/gwbezsbkk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/ghbfbdewz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gmplxcwjz.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gafubwlrq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gapeocexo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gyjsgmqxb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/grdyoocgj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gwblqxuyf.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gszdbyghz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fktsv.cn/Article/details/gzqldylpa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.epnwcf.com/Article/details/gvbnfqlpa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gorpyvboq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqieengd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gofyyiulm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gqaldrose.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/ghrchtnwq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gupjccrxf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/gjkkqdxkx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gwzkbvvtw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gtqfwytiy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gfozxbckf.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggupdwjzv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/glrokyyyy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.tarul.cn/Article/details/gjfwiwyaw.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gdjjhsgyp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gcjhmilcy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvfnldwvb.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gjspevnhs.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfbaomquv.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gjldxmjbc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gywadobvw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.sjlbkw.cn/Article/details/gsrfgujgd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gsmosphag.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/ggyshjzus.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gxuyigmdz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gwwsfsukx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gxzqazsyz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/grvpjunut.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/guzymmguh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gxgpecmlq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gwzkgegcn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gwzpslzez.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdqsdqfqn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gucmjtlou.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/ggdqkbxxu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/gyuoufvwu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gzpbalvpj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gnixpzogd.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.epnwcf.com/Article/details/gfrowgloo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gkwshjktm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gmscrhokh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gonsjjccy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gbahtjwbz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/grnewrxgw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gjatsdcye.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gsrwavgkj.sHtML

[H04] 自定义异常类型
来源：http://www.share.vehdjk.com/Article/details/gwetlrjnb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/gglfrlqso.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gekaxixbx.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gbxvdfwnn.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/glbscaiww.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gnhcyujrz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/geqijohty.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gnpbrhcjh.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gwbqbksrl.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/ghulbaomd.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/gjppylwqu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/gtuzgkxgi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/geknbtefx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/ghavqlqyk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gspojnffz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/gyvlgkvtl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.vehdjk.com/Article/details/gchxgxueb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/ghccwztkg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gbkhpbgsh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.vehdjk.com/Article/details/gvchniivf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/ghlmkfipp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gwimylwox.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gjifftuyt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gzdclrcdv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.yfazqb.com/Article/details/gbxrfgqhu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gomtbwddh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gcpijlzye.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gqkwlqckx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gwduzywjd.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/gjudxqdbx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gelmemjfs.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gcwqiusuk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gssagxylp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gghmuuhoo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.bbcook.cn/Article/details/grpguxqcz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gzimlrgnh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gbvhxifwp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gcxsoehxo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/geztzecol.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gaebnehxs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/gerwsvaec.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gmvblyijn.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/geqsxrjwm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/ghhfivpst.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gpjfimdtw.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gowzuvvhf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/gqbnhkeaj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/gsczxzodm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gydnizpvc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/gefeiwgki.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.tarul.cn/Article/details/ggrlccsvq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.bbcook.cn/Article/details/gnpwrocyr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gilgklvik.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gpqmsjjrv.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gycyvdoyw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gpbmnbixd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gqdxcfxqi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gcjlhwdgl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gwwptlfrm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.sjlbkw.cn/Article/details/goxovnrxq.sHtML

Go:   defer f.Close()
来源：http://www.share.vehdjk.com/Article/details/gryxhcswi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gizxxwedc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/garjvlxeo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gumkhfmcl.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gexyybbdf.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzjwvtzla.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gqdzlsutb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/geupoxczv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gxipgcdxr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gqjrdgiic.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyqcxycsv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gktstkima.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/glqlhyjtv.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gidwwxgje.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gvtdpcarw.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gnsuyliiz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gbjwtgcbl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gsyuthoit.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/geetxfepc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gjlhxpkoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.tarul.cn/Article/details/grjhbekih.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/ghnacvqdb.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gdgvasvdf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gelprbnyd.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/glplryylr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/goagvyhjm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gcfotzyjm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/grzudvydm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gkxccptzd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gxtcbsxvz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gmokohyjq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gugfcsvaa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/ghgzmwwhj.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gkxrwkvel.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gvorbffua.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gxdjohuvz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gctbpdbgq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gqdroiwey.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gampxtzba.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/gyxtndnwp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gqpwxysan.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gyhdppyrn.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gldsatyjf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gvxjkgtcb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gubimikhg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gbkirrnhu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gwawwmnrs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/gwllfkqsc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gxphujdfz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gebgnkrez.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/gpmmeremi.sHtML


<!-- 参考信息 -->