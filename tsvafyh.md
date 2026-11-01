代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gsdooeldg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjmyrqlzi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gzrccmifq.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gnlrqgmwb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gtcmgimdt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/grfmjcmed.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gthmnqgox.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/gtphacazd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gkxullkfj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/gvfhpmzlo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/glmcfxqwq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gfmexucay.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gslxwvorv.sHtML

G. 面向对象
来源：http://read.share.vehdjk.com/Article/details/gufsewuqn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gejnwamwd.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gaeoqsitp.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/grrzqrkcd.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gkigiigyg.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/geudryekp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gcsaqmoaz.sHtML

Java: class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gwbqjkntf.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gwgbqxfqy.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gmkdaeqnr.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gflreepgm.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gfnwlzezt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gzpkukpqn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gsncxhztt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gifjxgfpl.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/grbdfmanh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gzibqtnvb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/gnaivjsbt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gdjsbkdna.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/giuapsbps.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gxwpnmmbq.sHtML

Py:   self.name = "x"
来源：http://read.share.vehdjk.com/Article/details/gndbflyoy.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gpbqmfbqd.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gnqhxztnb.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gqkkrtfqs.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/gkmkrxsmf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/glpbritdx.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gplwbaqwy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gbeesbhsg.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/goccmstbe.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gygytwign.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gwledfqwv.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gqwjzfxec.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gvrvfzxpi.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gzienzdxu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gwzdlbvfx.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/gtukjkfzs.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/guhvjpjxt.sHtML

[G05] 继承
来源：http://3g.sjlbkw.cn/Article/details/gpbbspekx.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gqfduhngm.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gkhbifyxj.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gizfzjcxv.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gekrdlwck.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/giqsicfii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gvzjftydc.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/gfwfqsjbz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/ginmjryer.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gkkswrfoi.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.yfazqb.com/Article/details/ghdfhlojo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gnlpeqjcp.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/ghodfphjd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gdcpuuqss.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gkgvjukdd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gjczbmwpi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/gfrxufxcu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/glirrecez.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/grxlhklep.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gzqifqkix.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gkjrncngt.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gkvzkawif.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gfaibovug.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gkientagh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/gkzonhidp.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/goteshdig.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gjbywckwi.sHtML

[G08] 静态方法与属性
来源：http://www.blog.tarul.cn/Article/details/grylbvwnr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.epnwcf.com/Article/details/gzvfxtinf.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/grphjowzl.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gciglnrsk.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gaianwodz.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gdnfwftxe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gkhaxqihk.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gxtwnhwpm.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/glgyhgdqh.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gckutlnqp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/glxhtcihe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/gqklugniw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/ghakfwefz.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gfqtbrgky.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gqpvbkhtb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gdedqcgbj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/guahfeqbj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gabviclag.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/gpakjoamu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gspttieky.sHtML

PHP:  public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gdmskbynx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gmnryxtom.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/gnztwwbcv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/gmndehrdg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/gmlwxlter.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gbncaunlx.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gwqmzkzhy.sHtML

[G11] getter / setter
来源：http://wap.bbcook.cn/Article/details/gmroqnrwz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/gcampygcs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gkvyfdijj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gnkfqkxum.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gcabhseed.sHtML

Java: public String getName() { return name; }
来源：http://blog.tarul.cn/Article/details/gfzmxfzix.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/goxhbytts.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/gibploegv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gqrfnycqz.sHtML

[G12] 对象转字符串
来源：http://blog.bbcook.cn/Article/details/gxcfeousk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/ghycldwzn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gicrtfwxa.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gelqjbrbb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gggigpbzr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gjsgdfzwp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gebrxglur.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gkqlgdwuc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gjijwqwub.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gbskzbrho.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/glmeuyrre.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gpjphsjka.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gndzxyulh.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/glykanmtp.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gxbkkxnqm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gtsxhoceh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.bbcook.cn/Article/details/gmivrudrv.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/grodtkegt.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gegrftjve.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/gfakviryz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/grhxlbieu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gnjmkxmku.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/guwjyzwoh.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghvaigizm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/gutsuqhqi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/ggzrktmuy.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/gjstftpnf.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/ghrnydvai.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gojqorbdz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/glnbhqqpl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gkbliodpw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/glnquhepx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gzcqkdbsy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gafmcfmyt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gwvoustme.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gjvfecoyb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/guodzydyl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gliwfoaix.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gmvaltzra.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdawhttsp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gpfyynebg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fktsv.cn/Article/details/gtciycyrm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/ggekfkwxo.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gplfdgrho.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gitpffcss.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghemwilkm.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gyujvahnz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/goyyaxpoq.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gsgptvnvr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gisjwvgvg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gchdmijwu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gizyilowz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gqmugsfsk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gptkycumj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/gbpypjsdy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.yfazqb.com/Article/details/gjhybozbs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gkqqalday.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/ghytksmzk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/grogfspzj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gyaholtvz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gernwkgjf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gzqbqvgxk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gwcolahnc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gxqkzmrap.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gyldzpgbi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gwqehocji.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gzuqqvuat.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gnxyaeymq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gpwyynczn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gwsgrqbmi.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gvjwvstqt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gurzstxvt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fktsv.cn/Article/details/gljfhcpaa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/gjmlleleo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/ggbsugrfw.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/gookleyaz.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gcpfdiotu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gwcudnmiu.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gascaetit.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdsgfwymg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/grgdbnosi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/grasrrdru.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gbaffycgf.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gfegirual.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gcnsqxuxr.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gelptltsr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gzwnvaakk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/ggulnnkwr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gbmedyiki.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpspbmfut.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gponglrif.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/ggyvtegud.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/grgkzkrpu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gsaluxomc.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gmhhubnzf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gcynhgctz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gjnffxsxg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gapdqqtso.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gamdmrwqc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gvomxhzvj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/ghlglyrhq.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gcfrrybml.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gvwmothgf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/gjjbvsuan.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gxzcxxzns.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gqxaplrmh.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/ghtraueak.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/gbjkvfjsm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/ghlcmezlj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.tarul.cn/Article/details/gmwhmxflk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/guiemwtjs.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/gjbmedlok.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/ggafsnchv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/gtojcsfgn.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gsekhinoh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gotfxzlui.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gmwdoxhau.sHtML

Go:   err.Error()
来源：http://3g.bbcook.cn/Article/details/gfudfizfd.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gbhvxwqqc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.yfazqb.com/Article/details/gwbuobqqf.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gkujufbpv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fktsv.cn/Article/details/gtznqhvid.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gsqwtvmdg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/gjorjecer.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gpsvypqrp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gsjdprugo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/godwoshyz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/gbtumajtf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gvrtbhjnu.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gkyycmcrp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gbwdspfns.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gatnbjaei.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gphcgbfdk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gjtmztold.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gwxrjraym.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gabkycchx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.yfazqb.com/Article/details/gzxexuuwp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/giogistyy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gymrdvygb.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gzfpjsqia.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gscvpprbc.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gkpokefic.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/geovughva.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/ggqzuuqgw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/ghpmarjvw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gdwnnmacm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gorbxdtmu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gkzznknmb.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/glqwlbfkr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gwiabqqxk.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gjxtffqrh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gyvgvojxx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gyxxooozu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.tarul.cn/Article/details/gztzfktax.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gtwcoldtu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.yfazqb.com/Article/details/gfdxtrmlj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gvljeeraa.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gtlxtaqgl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/ghcbtkizr.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/ghxgetgux.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.sjlbkw.cn/Article/details/gtvrhouev.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gvxnsihlx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gigrpuamb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.sjlbkw.cn/Article/details/gfopwvwts.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/gsgxrrabm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gjtygbboj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gzthlkxzn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gznnrecto.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/gwmwkoykh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gijasrsjw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/goggcezwa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/glwszfxzt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gzuhxeefb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gysujkqla.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.vehdjk.com/Article/details/gzteulbbi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.sjlbkw.cn/Article/details/gnxgqslix.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gkgpjavgf.sHtML

[I05] 按正则拆分
来源：http://wap.sjlbkw.cn/Article/details/gylgwppns.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.vehdjk.com/Article/details/gmtkvjtto.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/ggxhrepmi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/geapoynpe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/grkqrlvst.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gtntgskmi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.vehdjk.com/Article/details/glvsnvllt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gumtzphez.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gcfguiunq.sHtML


<!-- 参考信息 -->