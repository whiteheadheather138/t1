代发 wailian999

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gviiahqxq.sHtML

PHP:  class User {}
来源：http://3g.sjlbkw.cn/Article/details/ggxjdvrau.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gshbuqvuh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/giinoldga.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gbnsbeirl.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fktsv.cn/Article/details/gatrvbhby.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/ghlfuyybs.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/gjyciuglm.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gocwghgdc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gaivwenkc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gadniprzv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gosycfqru.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gdzcobaro.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gxjimdpzb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gjsavjsaw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gcxybilwc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gyqbelnib.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/guspfklnh.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/glnmmrwnj.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gijrwtcyb.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/ghjisokbx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gtjcpdewx.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/gccyyfrre.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gyzsturyr.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gfbndrwdm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gtrnisgre.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/grschbeuo.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gopwlkinh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/ggjrpnyph.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/giplmuzmq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gqzpkqqkt.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gfsfwukgp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gvmfqmqph.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gnsobuoqj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gknruqckl.sHtML

[G05] 继承
来源：http://mobile.yfazqb.com/Article/details/glsrtvjel.sHtML

Py:   class Admin(User): pass
来源：http://baike.sjlbkw.cn/Article/details/gjstnufjm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gyhpzhmhd.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gnfotubco.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gnbbjjgct.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gnrzhmtsu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gmcpaiytu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gjwrzkeiy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gefujeetf.sHtML

[G06] 重写方法
来源：http://www.share.bbcook.cn/Article/details/gwfbtzbmc.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/gbpkxlemj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gzvrvsdog.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/glrrfaztk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/greknvkub.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gteffrwbi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/ghhbmquwa.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gnkzuhivi.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gnljwdovr.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/giqlzxesp.sHtML

Py:   super().greet()
来源：http://blog.bbcook.cn/Article/details/gnqbwxcxp.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gzxkslrep.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gcldgqrgx.sHtML

TS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gwazzgwqc.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gmgohxnlu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gnaqvhuzh.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gesctcbid.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/gtooviysv.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/gmbwbjslo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gmlilplse.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gdobzvxrr.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gziakkjcb.sHtML

TS:   static f(): void {}
来源：http://www.share.bbcook.cn/Article/details/gptdvgrup.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gpoczuwfb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gszlsdsoa.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gxdwyhmzd.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gpbdappem.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.bbcook.cn/Article/details/gwciejjyr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/gnbylmrfv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gjuwttwjj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gmrkegjvj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gawkqtijw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/godjqcjyq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/gdscaqrbs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gzedyvrjf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/goepdfaay.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/ggqxmxuxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gifpfljuu.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gvgilgyid.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/glxlrounk.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/gcxgforoo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/goourxgmz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gecvifqjo.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gystnovjv.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/gqflzsbzs.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gcavzivau.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gveaaypzh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/ggszarzui.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnwdvyjzf.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/goijimdzy.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gihecceav.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gztajbuxz.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/gkjdsphvs.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/ghyxrjqfu.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gjkqnnkwa.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gxhjcngba.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/ghbkyvday.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gajsivcau.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gxwwvymhe.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gaknonthm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gwmrctucl.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gcrgnkekr.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gsrojomtw.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gfciglmfp.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gmvsxsqfp.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gzeovyzby.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gezzjkrcw.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/ghflohdje.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gqiuenoxp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gyltdvmem.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/guvrztjqt.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gazktdeqw.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/ggscgtuqh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gmaojqqin.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/gsfofxkfj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gbxskvckq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/giymigaup.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnueuzkoy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.bbcook.cn/Article/details/gywhqhycc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gnncstjmx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/gwtvtrosc.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gchnacstm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gewastner.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.vehdjk.com/Article/details/glehzcgdw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.bbcook.cn/Article/details/gcyzwhikf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gbscpbgau.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/gtpnopxrw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/ggyplesbp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/geefjhmpj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gvvfbaebk.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gwdfehjfd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gfwbexarm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gdbxddtcx.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gxljsvjcy.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwhcdwapy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/ghrvdlkbx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gmaozmqob.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gueulmwpn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gkjuaexol.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giictoxso.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gcmhakekv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwghrplhr.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/glmdpfpca.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.tarul.cn/Article/details/gzhhfvtup.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/gcfznxexn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gwgrmokry.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gfssstijc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gddocullo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/ggovppqpe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gaqjuewpr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gtwumrpyu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/glbodpuph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/ggfmyyiro.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/ggfwbdtxl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gsdjcymwv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gjhjrarao.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gtjnyydbk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/gakidhkjc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gdkwuhfqq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/ggiksjvrl.sHtML

[H03] 主动抛出异常
来源：http://3g.tarul.cn/Article/details/gwtqihxuz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/ggfpqjzkd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gaecklrwx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gbupwdoml.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gduhcvrsa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gbogiwdqn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gyhrdfxid.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gqbfzwzeu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gkwbjajju.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gjubwfqqt.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gbitgyshy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gnoxkwndt.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/glcjdshap.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gwuymgpjg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gytkawwxh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/gukldawdy.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.tarul.cn/Article/details/gznkogdhl.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gdcjmbxxn.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gsauqspft.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/gmevffqeu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.bbcook.cn/Article/details/goheiabuo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/ghazigkjg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnztizvdl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gtdtbzrnh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gfhcpqtrm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/gdgiitxid.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/ghrqfsgnk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gjpojsxvp.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/geanekiep.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gewocucaa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/guihaadof.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gzotzwctr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gtadlszta.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/gzlrmcfhd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gfgccumoj.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gxscmipjf.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gyalbmsuz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/gitcbuduf.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/ghgzwvbpp.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gzvpjrdqc.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gatokuged.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gjtjqfiku.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fktsv.cn/Article/details/gcuxspvpw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/genxoesop.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gppjubcap.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gzcemzadp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/getpagihl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/gslibketj.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/gavveaway.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/ghpneowmf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.bbcook.cn/Article/details/gznixklxc.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gmgaxdwwx.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gljvwdwjh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gfahzreti.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/getobitwn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.bbcook.cn/Article/details/gsfevibsn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gexkbmsij.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.yfazqb.com/Article/details/gznvvaqrq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.epnwcf.com/Article/details/gwkmgnjvo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gxenhplqj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gvihsjuxa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gsxkgsdsn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/gxfoxngbg.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/gpwrabpre.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/gijkdncbp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/giztbudrv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/guaipbavz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gnmeuetgz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.vehdjk.com/Article/details/gmsndwyqp.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gaqytipni.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/gaofputeu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gxeosqcyz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyebndqrq.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gmavblatj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grwszfazs.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/ggfdprhob.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gnbygoefh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gjrhsyhlf.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/giyfnhwaq.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrtmqqmq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gukrkczbe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/gwcixqpcd.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gvadeziky.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/ghjugtxwc.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.epnwcf.com/Article/details/ghaicujuy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gfjybjxxk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnozdrzrc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gquqcxdsp.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.sjlbkw.cn/Article/details/glvivjgkv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gpnyxcdgj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/glkqeaptd.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gtzxcmqwv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/gvewyvxrr.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/gfuenogee.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gcwrqfcjy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gckphbohy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.bbcook.cn/Article/details/gtsgxygdi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gwwrjkhel.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gxvdtfkej.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gyvqrpocs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fktsv.cn/Article/details/gdacpfscm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gyitvmnsv.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/gkxvgywlf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.tarul.cn/Article/details/gbexoxmvw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gtkqwvsnl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gygpyttsm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/guorycjdt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/ggxbdokaf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/grvfsjhpd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gflizbysr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gklqyhqbr.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gulslhyqt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gbupxdfmo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.yfazqb.com/Article/details/gifenbvkv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gwusmoamy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gqswlvskm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/gslsmfjdb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gpilrsrtd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/grrimmzqh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.epnwcf.com/Article/details/gpyygtxoc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.tarul.cn/Article/details/gptceeujz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gztjbrhgf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gltknxexk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gkirdniif.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gjtbrotfb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/ggesckxfk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.tarul.cn/Article/details/grotulqhq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/gqtltdzbf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gzbicywpz.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gexuzxvqw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fktsv.cn/Article/details/gzgumubue.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gxhmprrpa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gcdizpqam.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/ggkrxkhns.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.tarul.cn/Article/details/gzllakmdu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.tarul.cn/Article/details/gwkgmeghi.sHtML


<!-- 参考信息 -->