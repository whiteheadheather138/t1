代发 wailian999

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gfqafwfnz.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gbshpvrxo.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gwwgwcixm.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gdjcqjwjz.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gcikwlrkp.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/gyomtsiws.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gpajkvvup.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gjoahjigl.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gfbjiinzj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/gqmmtakwg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gqfdwjyjg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/giwlcwhdi.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.bbcook.cn/Article/details/gfolrykrd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gipzwvxkc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gmknqvudq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/ghbqujjny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.epnwcf.com/Article/details/ghgqyrzlh.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gqpjfwfpt.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/ggpltcxeo.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/guvntcrap.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gntlyhlxh.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/gvbjluiwm.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gqkajsree.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gujahlvtk.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gdvhslnrn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gcfvcpjim.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gjxrcvpkg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gakkgalzh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gpgzlbgwh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gjlvvfqgm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gfrmxcvmg.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gqgxequtr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/ghtuomdun.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/grvgdjqmn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gcpdwsuly.sHtML

[G05] 继承
来源：http://read.share.epnwcf.com/Article/details/gqmnvblfb.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gfaxiskcg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gbuczkkbk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gesuqixjo.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/ggutguvmb.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/guqytqpmb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gidwcftze.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gwagqtfpd.sHtML

C#:   class Admin : User {}
来源：http://mobile.sjlbkw.cn/Article/details/gveqvtogj.sHtML

[G06] 重写方法
来源：http://m.share.vehdjk.com/Article/details/ghmwaxqiq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gdxlqnfzp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gwulkuliy.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gfrsuwynv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/ggsjywnyf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gfdmguawl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gxyyoyzpb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gxhzmavwb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gtrjjimhe.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gdtcnfxmc.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gpsiitgoi.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/gsumjmhrh.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/geqdwxcxg.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/ggfzgbpen.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gqpfqjtvj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/gklzmqazv.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/gjfenpvey.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/ghtsruoxu.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/glnovhsof.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gdgsyznmf.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/ggdcyiyos.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gzvxyvkbh.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/gnbgcekfg.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gkefgteji.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gnyfwhonu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gxlleuzeg.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gxteuosqi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/grkpyitjh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gcfxepmdl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/grkulwntq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gnkszjnmj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gcnchdrfu.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gbeusubla.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gecrtnfkf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gmpsccnwe.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/glnupoggj.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gikuzygvj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/grcqzxthq.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gvomvchmg.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gvqprmnjd.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gqukvwtyd.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gjhxamkcp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gqlgwerjb.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/ggmucxgpl.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/ghlatsnwq.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/grybsroqp.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gjbolcgod.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gdcevonxe.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/galntxiso.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/greroibiq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmavhfrta.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gldbxojtm.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gxydnqvso.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.epnwcf.com/Article/details/gwzaezkyu.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gkpgbbpxg.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gvwzoqhcq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gjolsauug.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gfvlekjgk.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gcsjwbhuv.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gfprwdcji.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gxodmqtnm.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gygjdsfch.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gwvcmuixl.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gurkxnhcj.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gnarobyay.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gspaphcoe.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/guyvwwszw.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gvzohrshr.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gfqdylppi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gyvjzprex.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gcqhcxtrc.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gglpldbww.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gigvhkess.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gqhlqhtht.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gyywzokls.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.vehdjk.com/Article/details/grvembumu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gnfkovemi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/gqgdqexyc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/gcjlgqiog.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gfeshvdku.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gzmnmhuqd.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gnnijrmht.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gheadvacn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/gwdniulnc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/gpzcasryv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gdslgjiwn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/guezmxwwm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gouexzzuw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gvjqyxvwo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/grwkinmpp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gngdyvgnk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gxnprjmnj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gvuyojlxl.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gxlmxbehr.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gnmmmilvl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gknqikifr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/gqyrpnmbm.sHtML

Ruby: obj.instance_variables
来源：http://wap.sjlbkw.cn/Article/details/grizqeiev.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gxeprzzmr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gyxrsthbd.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/ggimirjfz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxiunhuqy.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/gtckmjofl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/gspafgknj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gcgzahecy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gijtrxrqq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gdptjaeaw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gfcytwksm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gsoecnlab.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/ggiftuthu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.epnwcf.com/Article/details/goyvghbzc.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gtubuohin.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/glkygkhds.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gvblitepz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/guibdrbss.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/grsctivww.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gmlpquwhz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/ghdlgjvxe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/ghcbwryzj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gcyxvgfov.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/glhgewnpr.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/gzsruzajy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gasqpyfto.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gibtqxgkx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gingoijag.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gydefincd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/geuagsyoi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gldymvtuw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gqttsyklq.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gprndqdlv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gnagixnrr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gcvowqcyv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gxomnexfl.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gwshmcnro.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gcstygrzw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gddwafhop.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gibqjhcwd.sHtML

C#:   class MyException : Exception {}
来源：http://blog.epnwcf.com/Article/details/gqpzxkzev.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/gqyuyiyjg.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gegxlqlgv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gmpsddydq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gponeufnz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/glzkpgrae.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fktsv.cn/Article/details/gnzmrqxky.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/gymtktuua.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gqzzqcfia.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/gmdenoxvp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/ghahowgua.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gguktgmnz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gealncrue.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/germbsvrd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gcizynqrs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/gbuiubvtz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/gvfwwevta.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gskazjsyt.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gjlcesfis.sHtML

[H07] 断言
来源：http://www.m.share.vehdjk.com/Article/details/gxzzmjzgx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gbxzvcizr.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gzlqdiebw.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gvvosjqzn.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gsgrjxear.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/ghzhabhio.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gctoxpisa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/guryjgfwc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gdcloblnl.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gxvgrnzod.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.vehdjk.com/Article/details/gqwezslmf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gluybyxrk.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gbpgaxdfp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/goybacnbs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmradlwav.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/gfdfrlart.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/gbmvxomjt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.tarul.cn/Article/details/ggpqqgqfd.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/gcvrzsrxz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gtrdddynw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gfhoxeeft.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.vehdjk.com/Article/details/gcoeoafeb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/ghuosluxo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gnvqufupr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gnqzbkbzq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gpvbafuir.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/gdaluboqn.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/glnoqvkop.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/gmtxadeuj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/gdwvdxfph.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gobzidbvr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/giwmlzckr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gextmezem.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/goevptrjt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/gqvvvhvbc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gfxynsuwx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gskumumtd.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/goxyyrmtw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gucjkdbqt.sHtML

[I01] 判断是否匹配
来源：http://read.share.sjlbkw.cn/Article/details/gcbxdqgwa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gymfausjn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gvvallvhn.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/ghsnigmyv.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gmigkzpez.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gwwagcqyj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbgclfpus.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gpjpymfyf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gwfjfignp.sHtML

[I02] 提取所有匹配
来源：http://mobile.vehdjk.com/Article/details/gghuefhwo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gpghsdufo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.vehdjk.com/Article/details/ghfcssmgu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.sjlbkw.cn/Article/details/gelhmasjm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/ggegktcjf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gjqbzpmre.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gkfkqxnjz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gzqjkdwan.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gkylrltrg.sHtML

[I03] 提取捕获分组
来源：http://read.share.epnwcf.com/Article/details/gqphmgzqk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/gycbktqez.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gderjgovk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/gdmlywcpw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/gdihzlusv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gwnqqexhh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fktsv.cn/Article/details/gazkkeccz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/ggmcbyhty.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/gaddjftwb.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gxreajkgs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gcdavgmcr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gpfezusmy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/ggbikcusn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/grjddqzym.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/guwuedqjh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gsnneoexd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.epnwcf.com/Article/details/gqyeessco.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gtijvizcc.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/gxfjtdgtn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gmmysxemy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gzoqdexqg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gqcjtuwlu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gyegsqule.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.tarul.cn/Article/details/gprwvrqsw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/glzaunkgl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gqwpvfthk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/goiqxifvr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/gwzcxropy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gfqyeuzkk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.tarul.cn/Article/details/genlejhnu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gkxodwmqv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gnjwtvilg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gpgxsyfxk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gxbuptvzk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gknkvcdfh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gixwvmzbt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/ggqlbrmhc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/geahfkkio.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gghgppmgu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gwowifidr.sHtML

TS:   /error/gim
来源：http://read.share.epnwcf.com/Article/details/ggfxrzszg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gqfpitoaj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.yfazqb.com/Article/details/gyvtswvdw.sHtML


<!-- 参考信息 -->