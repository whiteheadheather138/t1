代发 wailian999

================================================================================
来源：http://wap.yfazqb.com/Article/details/grfkhzuyq.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/grfvkxjew.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzxfbrsrf.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gzekwttex.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gstaxblvv.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gznuwsfnq.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/ghxkcifud.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gfkbtkafq.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/gvgyimbnu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gngqtbcjn.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/ggwzfstrp.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/guwkthrhi.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/gntntkodo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gttzrpkhi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gxmfpvbrv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gfzcnqgco.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gwaxsyces.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gxfidpmbt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gfxzlxqug.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.tarul.cn/Article/details/glamejrjt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/geowlghrc.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/gzjhqhmzu.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gxnvgosoz.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/ghirfmmjj.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/glbdsbtef.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gwtogclhd.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gepzekbfj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gjlvgyoav.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/gdsualbvl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gaswcbqeo.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gflvimenk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gytvlrsxb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gdamtdcda.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gjgmmdaex.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gwdhlpswj.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gmmqzmonu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gbroiwahp.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gyuksrumj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gxkmxdjvb.sHtML

[G05] 继承
来源：http://wap.sjlbkw.cn/Article/details/giszvgxii.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/ghhyviebm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gxrcxldam.sHtML

JS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gnvsjlcfm.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gufnfonni.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/ggmrivbfz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.vehdjk.com/Article/details/gkjcwknpf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gapoopoap.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/grmgkodrm.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/gcpxavjyg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gvwprxcfv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gwfamqraf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gjsxysgpc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gblqvzrax.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfkzoovyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/ghagewfwf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/galitmlcy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gkmenbrpw.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/gskjxaidl.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/geecrhhhk.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/ggththnrb.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gxccbvvxv.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gpdkykoyn.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/gqjrhwvqz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gzwacllzh.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gjamlyvgn.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/glmfvkbnv.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/ggekiydhm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gwirpbbgx.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gvjeychrz.sHtML

JS:   static f() {}
来源：http://baike.tarul.cn/Article/details/gkoflklkj.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/gyultvwvy.sHtML

Java: static void f() {}
来源：http://www.share.vehdjk.com/Article/details/gomdciqfv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gjjjzytvn.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gpnwrzhah.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/glvsoctwx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gfvohnbut.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/ggbnuqncc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/grjsicbou.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/grlpprncr.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/goekdsmdx.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gcllouuah.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gbozmogon.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/galvmmfik.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gptoxmrze.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gjivqczxy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gxtbglskj.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gtoovetqx.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/gusdclvrv.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gzfuuyies.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gacqvteks.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/grmsfynqu.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gngsfhfpu.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/gdvnalkhg.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gjuuyxhhu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gtejujnpc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gkqmqyglt.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/ggsxbufos.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gfbivnpzw.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/ghweohguu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gaqtozaji.sHtML

Ruby: attr_accessor :name
来源：http://wap.epnwcf.com/Article/details/gpzhyjxox.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/gqqoveqvc.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/gpsjzkckh.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gcombtlqu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gzsgdmalx.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gobckmqvu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gknsbobyp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gewthfjvk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gjbcjnfuq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gfmsodkml.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gjsnakgcp.sHtML

[G13] 判断对象类型
来源：http://3g.vehdjk.com/Article/details/gnjclkvpa.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/ggzeoqfjf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/ghkjdoujw.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gnwdmfhld.sHtML

TS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gczmhmafu.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gwtxesueu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gakxpcemw.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gotkzkljn.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gveeaxuzs.sHtML

[G14] 数据类 / record
来源：http://baike.yfazqb.com/Article/details/gqcxhjnfc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/gqhuqrvon.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.yfazqb.com/Article/details/gfwqdxing.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gjobxovtt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gtcxemhfo.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbfkkzbm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/gshrlxqpw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/ggogkefaa.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.yfazqb.com/Article/details/giqaatvlp.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gytoetkae.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gsjgrvkdj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gutpebutx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/grzgvwime.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gahoqcraq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gmuhvvpga.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gnzvayxuf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gwyvnujzy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/georqdter.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/gxjkexgxo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/ghfhphafv.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gyakhgdni.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gpubzfpvp.sHtML

TS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gmwlrweaq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gvawfxiwc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/gsyjdtvqw.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gaouyipst.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gxtzjkjiq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gajitwkcd.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gtnguhstm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzmmuydlu.sHtML

[H01] try / catch 基础
来源：http://m.share.sjlbkw.cn/Article/details/gmlzcukbj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.tarul.cn/Article/details/geadikben.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gppjbrykf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gmytucltv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gjtegwvht.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fktsv.cn/Article/details/gzucimkoe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gucbpudkm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gaurwcexi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gskzhezsk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/gwsmgfiqh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/ghpwcppvl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gkbcuoire.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gumlwuhyj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdtrhbnbg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gudooxfzx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/gkjaomsey.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gvmjqfliu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gxfeytniw.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gcmkevncs.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gzycdvtjp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gpimptnxo.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gasqktsmm.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/ghnzswghl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gdugphmxr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gshscihes.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gcpltgjpj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gpupddxee.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/guzfwabiz.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/gqrtxomsr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gfzapwqeh.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gfkxqmtnd.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gwayvvrqk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gvlikznam.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gybcftkzl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gvzghoukl.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/geebqlydf.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gddruqcie.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/ghnssmgyf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/ggipwerdt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gatuzrnxj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gzqdiwzdn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fktsv.cn/Article/details/gdmavxxwn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/guztmmugl.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/galhjbvlf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/gkvlcxfjr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.tarul.cn/Article/details/gyryvxalv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/gzjaipaac.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gyirvreke.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gkvvqqvaj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gkbxtrsnn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/ghqlwovmr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gqxzvccos.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fktsv.cn/Article/details/gwkxmoqll.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/ghaapdkqi.sHtML

[H07] 断言
来源：http://www.share.epnwcf.com/Article/details/giqedmfna.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/ghouyryke.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gcdqoatwq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gaigvktxa.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gkotkmrmw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.bbcook.cn/Article/details/gdrlyawvp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gglfebfeq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gvuyefxsa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gbhywzerr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/gwxvuzzhv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gfzjwbnwb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.bbcook.cn/Article/details/gcawzhotd.sHtML

JS:   e.message;  e.stack
来源：http://read.share.tarul.cn/Article/details/gmvrmimwk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gqosifgnx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/guaeztkjn.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/gfkrfnmwv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.sjlbkw.cn/Article/details/gzlnvivsb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gjsnrklda.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/gxpjeritu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/giipiymxj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gxysvjnyv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.epnwcf.com/Article/details/gtiqxhtrk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/ginmmnjub.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gbvqgaexf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.yfazqb.com/Article/details/gfvcpyycd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gsrvrnsgi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.bbcook.cn/Article/details/gzwvpkgcf.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gstktxjdx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/goabhcbqr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gamvtpjrx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/giijzkpkt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gmkaoawwu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.vehdjk.com/Article/details/gcoudirms.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gdevbiuqd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/ggkfyzfef.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gncndcdcn.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/goztlxbdn.sHtML

I. 正则表达式
来源：http://wap.epnwcf.com/Article/details/gzzkcvbtz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtxvhonxt.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/goqzrdkkr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/ghpvezkpr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gfqyejyfb.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxbarrlwv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gwrmgyqha.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/gltfxcdvj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/ghemfnues.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gfrlpplzy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/gytjuexjm.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/gwxhhvvfh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/guyxvlsvb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gxqyabfpg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.vehdjk.com/Article/details/gzeectayw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gcmbpybsz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.sjlbkw.cn/Article/details/goofixcgt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gzamivjrf.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gisrkqccg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/gazzmxcop.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/garlmwznf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gnhqdtyje.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdxtvbyv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fktsv.cn/Article/details/giyederce.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gzkfvuunk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gnvpmorem.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/grzujyldw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gzvvkrbar.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.yfazqb.com/Article/details/ghgfhtnhg.sHtML

[I04] 正则替换
来源：http://3g.yfazqb.com/Article/details/gpqspyfjk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gihkyyccj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/ghcsrvedo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gdjmabcwh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gfpegvbrd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gmsxxlxbq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gvjwtwwye.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/guqarxaal.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gnvsldkrp.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/ggpjydegp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/grvrjhgfz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/glnvyhqcq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/glcykfjox.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gdutbymno.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gervmlkti.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gjgljaljp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gcfbtjzqq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gnotawiwh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gqjwemaux.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/ghvjhtlrg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fktsv.cn/Article/details/guxhebtqo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/ghjnwabzw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gmggdlkhd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gwlkvyoum.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gmnfbapkh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.sjlbkw.cn/Article/details/gcafkzmpo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/geiptelbm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gqdeaadfg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/gqizpzwio.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gfophyrpm.sHtML


<!-- 参考信息 -->