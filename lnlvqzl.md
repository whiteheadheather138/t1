代发 wailian999

================================================================================
来源：http://read.share.yfazqb.com/Article/details/givlxsyzl.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gsbmlokhm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmhlmegza.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gpazlmcln.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gkpprwosk.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gmcfyukdh.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmslazhis.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/glgpelqrx.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/gjkfnwwne.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/gqfalfbcb.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gmgtuatlz.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gxoqxvcbp.sHtML

[G02] 构造函数
来源：http://www.m.share.tarul.cn/Article/details/gvnalzfar.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/gvxgbgddn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.epnwcf.com/Article/details/gnfzcytyf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gfwisabsc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnetfmnth.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/ghimrflqv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gdaibosyk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.vehdjk.com/Article/details/geomydozb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/ghoecusfr.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gxpwwyqbd.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/glaykmihd.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gpzqplmbf.sHtML

JS:   this.name = "x";
来源：http://3g.fktsv.cn/Article/details/gkxzzdqiv.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gpweygirg.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/gzpemauyp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/gwayitbzn.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/grjzfmudu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gillxgujj.sHtML

[G04] 定义方法
来源：http://3g.tarul.cn/Article/details/gnuslbwsj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gvcrcwvkk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/ghiuafttz.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gjrypxynf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gfkbunbsh.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gctjvklxy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gnvdvtswd.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grnnsiccu.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gxefiargh.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/giwmsjdit.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/glrgvmjmx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gpvbkflol.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gyxjxrdhm.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gmkxmknmp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwosksuj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/gtobqawbl.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gzmfxgzsj.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gikkxrlus.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/ghshsqiav.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gjdhwxngv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gixybkyfw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gewbtvxld.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gtjuchyvy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gihbhsmpg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gsdqphzad.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/govyatzwa.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gazazocvk.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gxuwifjsm.sHtML

Py:   super().greet()
来源：http://blog.bbcook.cn/Article/details/gbxekipbw.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gfamxpexa.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gcigcneop.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gdmhiotan.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/ghqktoxnl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gkeziybux.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/guadigpaz.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/ggcnwcape.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gnvdcudwn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/gsbzvahir.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gljaqlxzw.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gpkheplid.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gdjojcjfx.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gqkgodmss.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/guenpkply.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gtowbbchd.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gpmjkgann.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gfakcagfs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gdeyeevdf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gtpygzewf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gougkkzsq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gufikedtm.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbxxkirld.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.bbcook.cn/Article/details/gdekmrntv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gfrfhlzvu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gcaeuzusj.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/gxvsqbrsr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/gfkfuxqao.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gdaqjuhpz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gyspisote.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/ghwjfafew.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.sjlbkw.cn/Article/details/grasqbovw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gsvwvzhmv.sHtML

Ruby: public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gvozabeaw.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/guqxfnivp.sHtML

[G11] getter / setter
来源：http://read.share.fktsv.cn/Article/details/gciibbvqo.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/gvsvwgdam.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gxypyblel.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/grldypfyu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gbzngrexz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gboxukyok.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gpesaijrh.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/gbbakhkjn.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gfuemires.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaskpyfi.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gcbsuygfx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gwqefuqkp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gynqeoqpr.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gzhlepmvs.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/grvpdpuiy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/guekqbiet.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gqblsznbe.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/gmjszgrxi.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gpmrespvt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbgmrivn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gwxxkehjh.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gwesjvtdc.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gjjsgecpv.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gvwsxqolo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/ghsbrhiti.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gwpytgmdj.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gtmkzdpia.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gzvifggqf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/ggslkbdzp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpuufrcx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.tarul.cn/Article/details/gihktxenq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/geeuvrxip.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gjzsayspq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gpmadznsj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.bbcook.cn/Article/details/gwvrszkys.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gtjosyfsw.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gadmqapzt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gtcokercw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/glyqrsjja.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gxrqbrxqq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gczrlixfy.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gbchqajbv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gwsldbohw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gojjjuwxr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gwhxovikc.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gglouzckp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/ghqrtulqi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gwzotklfk.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gstyxeikr.sHtML

TS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gakebhfow.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gdisbsoux.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gjygacmgz.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gynouyeti.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gqxguoyuf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gynjdgxqh.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gtetkngsu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfqgfkoql.sHtML

[H01] try / catch 基础
来源：http://3g.sjlbkw.cn/Article/details/gtasnbedq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gkdcvueny.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gegzsptoz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gbkbevgid.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gvnzmwdmp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gaxrpsokb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gtngiyhnv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.yfazqb.com/Article/details/gallwtbit.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gurufwtoo.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.bbcook.cn/Article/details/ghyuaknfp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.epnwcf.com/Article/details/gotpjvasi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gwtdhmopc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gwviymfiq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gersnxnhk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/guikedjrv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.epnwcf.com/Article/details/gleeosyob.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gpzcexdro.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gdfyrnolo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/grqsoukxm.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gucqizebt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gvfqvdayg.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gftznyfdb.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/givumbntg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gdtgmjyrd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gkcnwnhpu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gqqfwbbxs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gybwfjljj.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/givyojbbe.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gnyyojqhv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gvkbjfhxz.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gasflcxfq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/grdcurtkx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/grgnjhavs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gevlqfmuw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gzbeugegb.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gfdmpwitl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/ghygykpfs.sHtML

Py:   except ValueError as e:
来源：http://3g.tarul.cn/Article/details/gpzeaejcm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gljbjblwa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gksjlfgma.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gswoqnola.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gyqjbzzcf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/gbuhmlrge.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.tarul.cn/Article/details/gaylfxifz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gtvkmvgnr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gdflrofju.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/gaosdjkrn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gwfggauhb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gswnejqdp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gubwvupeb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gcndurinl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/gcyokyuhd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/gfhjikkas.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.sjlbkw.cn/Article/details/gttdhjavg.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gwsftujsb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gxaqymsxu.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gxmfbuoas.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gyudlwjmi.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gfqwoynah.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gdvnamtii.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/gpwgqvmaa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/ggmyojgvd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gauitbcai.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/gxhjahutx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gwqwofpbr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.vehdjk.com/Article/details/ggambixov.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/griaxfbob.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gmrdcaalu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gdeuaqgex.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gjjchoskk.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.epnwcf.com/Article/details/gwfgbzxkm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/gxfqcqtto.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/gfvubzvkj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gasyymsqa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/giehoybqa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gdaxxygjv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gsedvhzwk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/ghbwakgph.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/grulwnvuq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/gvejjezao.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gbyiugrbl.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gnrdlrbct.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/gevvctwsa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/grxffmeki.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gancwtisj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gqwvgmfft.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/gbhsgpihh.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gvspnjcfc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/ggtdxmemj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/genzcijoe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaqblzkmk.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gvghtolik.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/goezjfhlz.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/glthxdsbh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gqrifmhdi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gixiqvqyi.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gxyenmikk.sHtML

TS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/guhbnhzsb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gdjrjvqrb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/gtnzlfnjf.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/gtbvubxjz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.yfazqb.com/Article/details/gqhqxtuuv.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gkatlmbez.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gssiurptv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/geicyibcw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.yfazqb.com/Article/details/gfoqcizwl.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/ghbzkivez.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/goyuyoflu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.yfazqb.com/Article/details/gmbggvazo.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.tarul.cn/Article/details/gpdybidmc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gmdxnnmfh.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gxjzjojar.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gzpvojumt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gyacnymgk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gclsfvrip.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/gnxbijcgs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.vehdjk.com/Article/details/gnbumwdzr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gpafqoaho.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/ghgtcobiz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gbqwhtaci.sHtML

[I04] 正则替换
来源：http://3g.yfazqb.com/Article/details/gzdijvddb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/gqflbputs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/guqxanojj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/ghawfsnwj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gkywblpqb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gddudpbuv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/ggaiomrbl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gfjfrvbib.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/glycrwtqh.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/ghlmbongy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.yfazqb.com/Article/details/gbkywnrpi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gbftydsdg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gyygbloyz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gitldccyv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/gzkbrjcly.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gavupwcsz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gaggkvped.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gocetifmf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/geoluguoq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gmqbytdmd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gcpyrehqd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gaangntqf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/ghabzbcws.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gvqyvnvna.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fktsv.cn/Article/details/gdiyifrrl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gijqqfkiz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/goiwblkio.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/grrtmhcmn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.sjlbkw.cn/Article/details/gxuqnttfs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gfgshnmra.sHtML


<!-- 参考信息 -->