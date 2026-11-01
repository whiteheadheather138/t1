代发 wailian999

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gspougjdu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gwzcpffjz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gfsinvqwc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gplprhkow.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gnatbfjuh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gtvuvzviv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gselatcfg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/ghcjotcjd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gqyzkqrpg.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gppamhlqv.sHtML

Py:   self.name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gghooquow.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gxsesbpme.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/getvdrpvh.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gweyjlawu.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gepyknobb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gtfdtywkn.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gmtsvlzru.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gjvpsigiw.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/grjcupmxe.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gtrfzrhse.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gbiolvsez.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gfurfmxft.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gftripvea.sHtML

Java: String greet() { return name; }
来源：http://read.share.fktsv.cn/Article/details/goiligyln.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/ggzozncnv.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/ghikyiakr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gjutemfaq.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gibddrncz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fktsv.cn/Article/details/glehiwkyv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gpbwstihz.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gdzkwdftx.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/getuybjtm.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/grgyzqbue.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gxrwutbij.sHtML

Ruby: class Admin < User; end
来源：http://m.share.sjlbkw.cn/Article/details/gthwsamqv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gwvweckrj.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/ggwstpwza.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/glzqefjpd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gzwzdzrlc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gqdiukxne.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gwaegrxsd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gfplrajzk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gsthjxmck.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gtixigoys.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gahmrjjxy.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/gjrbzaror.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/ghgvcitjd.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gjecxsmul.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gyhjkoxhq.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gmlczuezm.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/goggfddiu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/gymfbbzmv.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gbctydtme.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gsczjyqlm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/guqzpuqbk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/giuxcerlz.sHtML

PHP:  public static function f() {}
来源：http://mobile.sjlbkw.cn/Article/details/ggrmlzzod.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gxzdcpkkf.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gantyxwwj.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gkyxumarz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/geutvamld.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gtsosgvlv.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/giboloyts.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gyhwlfmkf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/gmpebbdun.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gpspljero.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gfubqfdng.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gepzdzskn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gbeugcofy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gytwxqupj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/gwltgrptp.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gfsvrfmpp.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/ggyeeilgc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gsmrnimcn.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gbhltfxle.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gqbaunzwn.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/glwrphfgg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gjgldzmir.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gsrzitlrg.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gbjdosajy.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gyjtingbb.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gxzryrmxq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gyaxsldhd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gmigzcrtd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdgmlfosl.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gkfbsliiz.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gtkaijtzd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gjbmmkmus.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/geqpldejj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/giiliurjp.sHtML

[G12] 对象转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gcczgpips.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gwacqdgpf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/ghnmgstxv.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gjksrstzo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/ghoxhadui.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/ggvrpjjoa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gneihakem.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gbpjojqxh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gnmldpcui.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gtbllakvu.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gqheuagyt.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gwpzbbany.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gqcbgeejl.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/glmsnbkzk.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gpwzccseq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.yfazqb.com/Article/details/giogclfhe.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gvunitodu.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gkacamnsb.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gvthwnvig.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/glmgnwdld.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrmmxcxj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gaemuijqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/gbmorzmuh.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gwuuebcmt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gflklismj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gjbyoxhco.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gxblamvez.sHtML

[G15] 枚举
来源：http://baike.yfazqb.com/Article/details/gwwsmsbht.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gjwueuqrx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gahqvxnwl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.yfazqb.com/Article/details/gjmwmvjle.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/giaqizdsl.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gobmhxolk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gzziyaraf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fktsv.cn/Article/details/gnxvfxzpa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gthvuyenv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gveogvzaq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gdwflkprn.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gguvpszvc.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gkiualiwi.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gpqgnkvcn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gmjkgxbtm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/ganjglspl.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gtpjkizjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gabmskqew.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzryziyrv.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gvwzraqtg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtfskydby.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gstplnnms.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gplmzihjo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/gstmpyriz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gsybmbnan.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gmosjcahx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gpjlttxql.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gtudaqglu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/galpuvebj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.vehdjk.com/Article/details/gredrmasy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/glifvmixl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gxmdspsmz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gwuelqgff.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gkxlqmbat.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gwcjujktl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gaqkhrnlm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/grugtoqol.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gtrxxrkzi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/ggsdtdmxp.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gfeobsquv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gdgkcqnmu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gkbbhbmjp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/ggnquvnqv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gmrmacsot.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/grfqaphmj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gycdspmno.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gywnfbuqv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gvynrdlyq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gvdmwnagv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/gzldnieru.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gcramlvkq.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/glzhvfyta.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gcopaqdye.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gexzoxovp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gyovtbfyk.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/gmelqjakk.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/gbkzkwalu.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/ghfybgiir.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gobwaabme.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gqrlqbfqi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.sjlbkw.cn/Article/details/ggwjsuetc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gxkzoqwke.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gdfcibqct.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gdpvhhrzu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/gyqnywrkg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/gylbtvlrk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/ghfiuxeor.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/gsvcybvor.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gxllvbjui.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gaievdgfm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gghoyapel.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gymsnveak.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gocdpinuf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/goacplciv.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gwaaveune.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gvtftfryd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gjpjwynpq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/guyacwgwk.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gkdcjkahi.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gfptkmjpq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gddrzjwny.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/gaankbtlf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gojjjajdf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gpunpkoes.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.tarul.cn/Article/details/gilgqbwla.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/ghbhshdcu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/ghwjgwdmf.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gsmmbjvun.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.bbcook.cn/Article/details/gevweqzqs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/ggogzuhsf.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gsnaulucy.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gmtfeeceb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.bbcook.cn/Article/details/gqcbiglci.sHtML

[H09] 带错误码的异常
来源：http://blog.vehdjk.com/Article/details/gqksjaclj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/ganhnlkiw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/glaksfnor.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gskewwrez.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.bbcook.cn/Article/details/gqfztyvta.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gijpluqyy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gsepgbuao.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gluoasewl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.tarul.cn/Article/details/griceljck.sHtML

[H10] 资源自动释放
来源：http://www.share.tarul.cn/Article/details/ghgeeoifu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.vehdjk.com/Article/details/gzhbmrdmb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/glztdfzrh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/grjapqfpr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gsuhpflzz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gumnytszq.sHtML

Go:   defer f.Close()
来源：http://blog.epnwcf.com/Article/details/ghqdzhkzz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gkolaobvu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gldxjakbd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtlkiojhm.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/gsafvmxxc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpfccyolb.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/gtvrqvwnz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gjuienuog.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gyrfribhb.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gumtcwjnx.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gdvlwijit.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/ggrymjcfz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.bbcook.cn/Article/details/ghmacptkz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gtthntpdp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.bbcook.cn/Article/details/gttbmxmpl.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gftvmmglg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gjmhppwhx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fktsv.cn/Article/details/gqowctssh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gpgtjgbyn.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/guoloawvu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gydzlwcgx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.bbcook.cn/Article/details/gqlpedcdk.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gzxuqixwz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.tarul.cn/Article/details/gpwugashy.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gnktgwvkw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/gyokuhjtt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gjtntqeeb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gmkqlbmhe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gutslbqcu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fktsv.cn/Article/details/gthuptjkm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gfzlrzdyo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/gligtpxpj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gzkboqulf.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gfqzrvlzt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/ghkifofep.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gzuxejfer.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gyovkkjna.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gcvzfjldd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/ghjbynzsc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.tarul.cn/Article/details/gywyvvtky.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gfeeyyydo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gfaxgcdxa.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gergsruld.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gtkldphhk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gthbhcgrp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gjdtzsqdy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gbpmklazg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/grxwhwqze.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gsmzwmuyh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gjvhwzuqx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.vehdjk.com/Article/details/guticqszy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.bbcook.cn/Article/details/gkemkbgsd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gpgxzofwh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gyjxaciks.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gjxdbolhc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gcfnitfyj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gzledxnfl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gjkylsvtu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/gjejkrodi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gfqpfeavi.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gnmuysjob.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/ghnedsugy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gkiahrusp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gzydiieah.sHtML

TS:   /error/gim
来源：http://wap.sjlbkw.cn/Article/details/gktdgqqwk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gxxzcknfl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/gtptqedte.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.vehdjk.com/Article/details/gawgwevfl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gowxcoosr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.epnwcf.com/Article/details/gfrjqbmkh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.bbcook.cn/Article/details/gejgirttk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gdomlctlt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/grptmedsj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gjzszgnap.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gcoaatmwi.sHtML


<!-- 参考信息 -->