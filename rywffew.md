代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/gclvvzaxb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gbkofumiy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gyudfhskj.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gcbrdvsfy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gkdbtphab.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/guhjuvacc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/goqybjnea.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gzxtfbhma.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqqjjaujd.sHtML

G. 面向对象
来源：http://blog.tarul.cn/Article/details/gwmthczui.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grunreqyc.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/gwhxnjmul.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gpbmblcwc.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gfokuxpzl.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gblpvpgjq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/ghqpebagw.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gflnqdppq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/glgkgbqjq.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gzdveakdu.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gtegcpfmk.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gjxwlrvcz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gvsfxpjdj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/glpaxysdy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gltwysvxl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/gusoeerdg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/glbxelrsc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.epnwcf.com/Article/details/gdgtrwtpr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gasyjmjjs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/gqdfsbljl.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gjoxsgxwn.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/guwcuauiz.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/gntpdyuqa.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/godijvxjh.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gmdxklymt.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/gnkrvespw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gmkfoyoix.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gqhtepxfw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.yfazqb.com/Article/details/gyakywvff.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gopuldsmw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gpltufrwd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gpmcvaboj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gmlflvihs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gbsgkwtrx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/giglreovi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gewfoduxc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gznwcrwtg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/glyjanbyy.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/gialwndmf.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/gngstsono.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gljreqhla.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gifaqjuiu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gkhhehnpv.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gpkqwuzkd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gknkyrjev.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/gyufhvlkw.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gmscdwaev.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gmjrjcuzj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gaukddymz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gykwksioo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gfvvtvlfe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/ggunzxkxi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gtdpydtnb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gtbavuqtb.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/givyqkynl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gyqzqrqzx.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gehdwnuom.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/giokzodje.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gncyubwbq.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gwmnilysp.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gjgzzdpwt.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gbyhmeghm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gtpbfwngf.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gfziywqjv.sHtML

C#:   base.Greet();
来源：http://mobile.fktsv.cn/Article/details/gwyznkohm.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gplihmwji.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gymedxuzb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grcbtqolg.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/goiwgcpbg.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/gtcibtwrk.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gfztcuwpq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gokqjguoc.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/gcnxuunbq.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gtaqdczim.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.sjlbkw.cn/Article/details/grltfpeat.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gzingyqez.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gawwxkcmo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gyafcnflj.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/gbdkemfxt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gnxxtmdeu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/glzeoerkj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/guzunnujs.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gfzvcvvmm.sHtML

[G10] 访问控制
来源：http://baike.epnwcf.com/Article/details/gjqwmprsq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gqxsjtxll.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gpxfprnse.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/geiauiejy.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gdozerlud.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gpekqsqxx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/gmxtenwyi.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gvjocpoer.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/ggfxkjsoe.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcxzhnvl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/guddeipvm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/ghuyrmtor.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gwvtncuow.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gjmnbcowo.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gqnmsypwj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gnlzhrekh.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gavhmiagv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gldgmbaia.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gqrvgtijn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gjusnevqe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gcklcsdyc.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwtwbuotc.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gajsygcbt.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.bbcook.cn/Article/details/gqqesdvtn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gtisglpls.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gjropqqgf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gnbedsagy.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/giowhnxki.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gakvbrheb.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gkxpkpeap.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gtwhzfwdb.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gvbxswoto.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/ghcmbyvat.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/gpweouegm.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gpglylbhw.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/ghzuxdusn.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gplpsulvq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gaoqtmzdw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/ggfyntejy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gimxmpnmo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/gqonarxws.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gwryxtxua.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/gcbbmbswz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.epnwcf.com/Article/details/gryanzfpx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/giqoizuaz.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/gcwdcglws.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gnjoiakoj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.epnwcf.com/Article/details/guvmgifja.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.vehdjk.com/Article/details/gbntagtps.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gkvgkmlrj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gadbxjabj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gccmcdboc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/glcczdekj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gdykxbqgj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/giufdtqwm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.bbcook.cn/Article/details/gtvityuax.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.tarul.cn/Article/details/gimknaxqk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/goihkevzt.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmlsaxknz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/gextyxrob.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gykdxfdls.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gtorucqjj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gkykdmdcv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gahafdeil.sHtML

H. 异常与错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gfuhqjlte.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdzaupehf.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gcwoeyxik.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gkucheybw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/gaqxioydp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gccufjmic.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gzlcycmuw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/guampdlri.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/gwixfmhud.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.tarul.cn/Article/details/gbqtgshdn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gtegppnxh.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/gtchvxjiu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gwwwgfeiq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gnqenzqlf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gsikjccmn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gnkqwoqrn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gdxitfapz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gvqotawwr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gmtvyuqhp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/guzsdmppz.sHtML

[H03] 主动抛出异常
来源：http://wap.tarul.cn/Article/details/gznlzaxui.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gxfhdgawt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gxnykljhs.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gqgemopry.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/ghlbeurxz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gnvwdjxvb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.epnwcf.com/Article/details/gobmrlqon.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.epnwcf.com/Article/details/gifeqhvpx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gvnhayvzn.sHtML

[H04] 自定义异常类型
来源：http://wap.sjlbkw.cn/Article/details/ggqtadaig.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/gfkhowomd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gvibapsdp.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gbwfenopk.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gpeuximbb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gjdwlvcpt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/goxowdzcl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/glfhdrery.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/gumpiwnnr.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/gqyvdqrfv.sHtML

Py:   except ValueError as e:
来源：http://3g.sjlbkw.cn/Article/details/grxetmymw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gwdemalxn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gumqahjze.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gneiokbnt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.epnwcf.com/Article/details/ghmqhpdyu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/gsmtynqwa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/gissfrpyg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/gcjtjdofg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gsdlwydhn.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gwlvfmtjw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gvudevmxk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gpxzmstsa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gmpkojteq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/glsbsikez.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.epnwcf.com/Article/details/gwjavpeqo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gywwtguwj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.vehdjk.com/Article/details/gcchjuhgv.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/gkkeejbsk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.vehdjk.com/Article/details/gpkyfudfq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gbzohsnpf.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gzsogzzsc.sHtML

TS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/grmbrtyso.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/gmhkzxmcr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/gdgeqcddb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/geefpjwiu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gsyhdfvxb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/gblcqehso.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/ghvhbtaqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/glgutbtov.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gjszvplgd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/gpcymkgex.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/gmakdztvj.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/gmwqymlxg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.sjlbkw.cn/Article/details/gznbzewej.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.vehdjk.com/Article/details/guymtzxdg.sHtML

[H09] 带错误码的异常
来源：http://mobile.vehdjk.com/Article/details/gnwravqip.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/gqthernhh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/ghtwzrknl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gmcdjoeyy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.vehdjk.com/Article/details/glvohdpkj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/gfyyvdech.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/guxinhbcy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/gmwsttema.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/gmldenxas.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gjzhbjzgj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gmatrknnl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/glswoqjdh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gbrzfzyvc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gfejfjjsx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/ggmxjoogc.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gwyvutbin.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/gxnsufmji.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gndnkxwdw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmmewputf.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gtwgxoniv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gcsledexu.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/gpyipcgxe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/glmsodynp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gquggvrnc.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gkwslayfk.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gtwusfqhd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.vehdjk.com/Article/details/ghkptiide.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.vehdjk.com/Article/details/gfydvwjgi.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gyfdmcydy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gkijhzjrs.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.tarul.cn/Article/details/gvfkzslbg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gjkemoqqn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/gdbuffyzz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gewbyfzpv.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gypgambqf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwhkwnuw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/gczzucyez.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/grhhmzawi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.yfazqb.com/Article/details/gqmmhjpmj.sHtML

[I03] 提取捕获分组
来源：http://read.share.vehdjk.com/Article/details/ghfbqucqa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/grswnsrli.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.bbcook.cn/Article/details/gtzyhsrjb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gifmkkybz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gcohkgtmf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/ggduytkfv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/gsvjrqvur.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.bbcook.cn/Article/details/gwfvwpfkd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.epnwcf.com/Article/details/gftmiaafg.sHtML

[I04] 正则替换
来源：http://baike.epnwcf.com/Article/details/ggzjrpcrw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gttbuxgnm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gomztxqlm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gbcwnysyb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gerjtxirk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gxwtblhvg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gcuulbiza.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gzvkhggfy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gpgfysfna.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gnezzpuuj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.vehdjk.com/Article/details/gsvukajyr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/gilakkipw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/ginthdrbi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gaiycwfrf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fktsv.cn/Article/details/gwbargdkl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gndtjefrb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gjajbeisv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/gbbpfgcns.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/grssurwye.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gaydjtblt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gmzeoopvu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gfbgrblyg.sHtML


<!-- 参考信息 -->