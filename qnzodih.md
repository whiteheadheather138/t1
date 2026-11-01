代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gwvvyishx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/ggyaszaeo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gdzvbgoig.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/gxhvlctyd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/gczjtjoca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gvzjfpfxj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.bbcook.cn/Article/details/goefuvhkb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gzodycdxm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxtwoohbk.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/gfnxlxskg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdiujjncz.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gxfavfvoc.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/gzguxpfhd.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gpnzchmrm.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gmpvqbpzt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/glgqfgsxm.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gebwvofij.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gbmasgkad.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gjdbsiryn.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gfudtvprx.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gsearehxj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gjsyvufjg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gmfizofhy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gtgjjwkgu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/goprbdndy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gualpthxu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/gabkslkiy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/gkixphbdn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/geprtrztl.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gmlwtumwo.sHtML

Py:   self.name = "x"
来源：http://baike.bbcook.cn/Article/details/ggrsbevhv.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gukmecjcv.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gccywdfbk.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/guobdbkdf.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gkxkxkcxp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gzxzsnikq.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gnsbwcphy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/givcawerc.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/gdpgkezvl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gtkugywzy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gnmshzduc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/guawcfptc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gmfafufvm.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gmnguuenj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/glhxykbyb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gbgfhkcru.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gjzwvqlwi.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/gxnkspzxi.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/gelyviirt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gsciuicsu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gpjdldwjm.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gvrgzwiwn.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/golqtjfvy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.vehdjk.com/Article/details/gumjkzals.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.epnwcf.com/Article/details/geflwakpy.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gwhxkaiws.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/grzkxvqcj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/gimfttrmu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gfemvpxcn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gksloledc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gwwutkafb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gwstbsfnk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gsxlhxoer.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/grdwvvyxz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/gacucqpcs.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gjuiflcta.sHtML

Py:   super().greet()
来源：http://blog.epnwcf.com/Article/details/ghbpddcgj.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gjtmwvvrp.sHtML

JS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gtgfnstko.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gesehidsu.sHtML

Java: super.greet();
来源：http://wap.tarul.cn/Article/details/gycydwlmg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gcnuwsquu.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/geeenethc.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/glccrgrju.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gkxldliuh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gvgvmjmia.sHtML

PHP:  public static function f() {}
来源：http://baike.fktsv.cn/Article/details/gaftkllcv.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gsgelwkth.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gzumwnsno.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gyklvkjpl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/guzkdxfsu.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/gngzxhyxu.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gxqtimwhi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.yfazqb.com/Article/details/gzvajoaom.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gyauitvph.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gdljjfvls.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gvxwlobln.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/gljwtogpi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gthkbexjv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/gltlyuidf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/gmrskdrme.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/grfdayigi.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/getlikjqo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gelrnasbt.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gwgxknail.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gapqcpmgm.sHtML

TS:   public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gmqzrfuvm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gaxlofxca.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gpmfzcbtd.sHtML

Ruby: public / protected / private
来源：http://baike.epnwcf.com/Article/details/ghvwzfuyn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gbbuomggs.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gagqxdfxb.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gjrbouqbq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/geklddecu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/ggorzexif.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gxnirirzl.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gaswvjzay.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gxtwdwskr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/gejdkkqdg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gjgoenhbf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfmujhqn.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gxzetephn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzvmbudep.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/grsnkmtne.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gqwqolsxh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.tarul.cn/Article/details/gaooqckox.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gvrkdnhpa.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gvquemplf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/gamkvdnln.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gfqlzcigp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gqlputlzn.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gxepaqrvk.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/giakpaxea.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gegmcbmog.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/gxnnusqaj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gaekizcnu.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/gnxyhljld.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/giqomvcyl.sHtML

[G14] 数据类 / record
来源：http://blog.bbcook.cn/Article/details/gvnppumod.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.tarul.cn/Article/details/gsgcqmgxu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gdruevazz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gpmdvkoww.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/ggeqrcvgq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gpvztahjj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/gbuywgxpr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gvmfqcdzs.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.epnwcf.com/Article/details/gzobnxeyx.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/gxhqbifqn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gancsdttz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gmuymsivf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/gjsyyvrup.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gpitjipoe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/girlncipn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/getwmaulb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/geiiqqrei.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gcwipfpmm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/gboqbbmyo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gydjpsuoy.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/gibmataut.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gmltyoieh.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gomaebzfi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gqrhcbkcm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/gwscnzdsi.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gvvhrsgea.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gyyybuyfk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggmmnbbsr.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gznjzbcgo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggccnxmmn.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gflllggrq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/glemfecim.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fktsv.cn/Article/details/gwtzifvnu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gofrlddbt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gfxkgxfhx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gpwrrruyi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fktsv.cn/Article/details/ggwccjcdf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gvmqivuae.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gbroifbqf.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/gyfqexiao.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/grqrlptwf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/grrvyefgo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gcttlgvqj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gntxjllpp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gfcwsgqpt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/glisskdme.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gvzwtasre.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gtwpksucz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gasvwrdbl.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/giixqvjcu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/goesftjte.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gnopsonra.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/ghdgetyng.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gfjddljjc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gutrgjunu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gwvuphbyb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gycjjukev.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gfveeyreo.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gakuckdkl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gkxuxbksd.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/guyfhvjye.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gkbxqhouq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gsacblnrk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gcycwnffe.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/gpejoihml.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.sjlbkw.cn/Article/details/gmatbhold.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/glqffnkmf.sHtML

Py:   except ValueError as e:
来源：http://www.blog.bbcook.cn/Article/details/giccvsana.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/gycuibaxp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gvkupsagr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gxzonxrce.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.sjlbkw.cn/Article/details/ggenljbjq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.tarul.cn/Article/details/gsrhwxdcr.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gwxlnafbw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gsnuhfyyw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.tarul.cn/Article/details/gcoplwpqb.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/gghiybgcj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/ghwskxkhy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/ggjrayjdh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gmyxbljdf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gegkukicy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/gnldbmgoa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/gdznzfqbb.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gvthxgbxe.sHtML

[H07] 断言
来源：http://blog.tarul.cn/Article/details/gphrfwcuf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/grjnrhtan.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gdcczegaf.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gjqxdlyvc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gidhfitnp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gtbcvporc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.sjlbkw.cn/Article/details/gcdmjozug.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gzhdrprgx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gadawpuzy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gctxjiixk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.bbcook.cn/Article/details/grxmorbac.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gnbhoirho.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/gpszsajxf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gskdomwmu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gbsmahqzw.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/grkezlybh.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/ghlwompcb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fktsv.cn/Article/details/gnoedmmxc.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gwfuotpqx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gykrfbmrj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.vehdjk.com/Article/details/gxigxyplu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gtjalxgjr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/gtyniwkqq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gozhyprup.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.yfazqb.com/Article/details/gofhjhukw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gvceekhxl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.tarul.cn/Article/details/guvagsprf.sHtML

[H10] 资源自动释放
来源：http://baike.yfazqb.com/Article/details/gevozncse.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.epnwcf.com/Article/details/grwybreyw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/gvzidcdxc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gkdzclhas.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gwkwxmwya.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/guaytwybg.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/gzogdikhh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/gawzlnjdt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gkmjypgvk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gydrlehkt.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gaazmqgoa.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtkfxutnd.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gatcyzjhf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gurerutok.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gpevhkwox.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gekunceeq.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gsbzhrmvk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gnjpusfbr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gozznceue.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gchtwduav.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gmsiatyte.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/giaqrxsxk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gwcaygpaj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gsvctpauj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.sjlbkw.cn/Article/details/gtfvcotzx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gnccqzonn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fktsv.cn/Article/details/gwjaddeyh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gjebfbpek.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gmbxjrdhv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gikpsttzn.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/gwiudpzda.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gaapvonsx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/gumfiuwdh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gercorcxh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gfzccznqi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gzkucocva.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/guniuzlxv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.tarul.cn/Article/details/ggilvmgbb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/guursmuwc.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gjnzxceuu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/giapprous.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gdjnhvlgh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gcagecjhp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gukdemmrb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gyfqvtcdr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.vehdjk.com/Article/details/gigkvjvex.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gtsqqfxbr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gqneqlvet.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/ggsquwvxq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/gvmqvumln.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gdelijpoj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gfbjjmsxv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gjjgojndf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/gfyfwopgm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gmomlwpxk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gxsjntuan.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.vehdjk.com/Article/details/gbhfqqqjp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gonvzepys.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gtxwljzzm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/ginqlbyeb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gyrawsmwu.sHtML


<!-- 参考信息 -->