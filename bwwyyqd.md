代发 wailian999

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/ghcvdvquv.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gowbgkdik.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gmtpzsybl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gfiryfcvc.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gfmflqcxx.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/gpvnhskbj.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gnixpdpcr.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gbogerirm.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gtldirvxz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gwkqhmdys.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/gnarlaywl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/grlaaoteg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gfmmjfyyx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gltoamzda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gezmevdom.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/ghgpqiwau.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/garyrhcsh.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gzubrabkh.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/guflpxqoy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gsvxwjdmp.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gzwgiqsfl.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gcfwwvjov.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gqqeucmhq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/ggvgtroci.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gjuyjqfha.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.bbcook.cn/Article/details/gqsmqxdiu.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/ghdxeixjj.sHtML

Py:   def greet(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gxkjkcula.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gvrzpjelp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gyscfziec.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gjllkrbez.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gapkgehic.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gvulqugsr.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gbdgigzya.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gyhzuhjzz.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gjgaiguvt.sHtML

Py:   class Admin(User): pass
来源：http://blog.sjlbkw.cn/Article/details/gpsgkyvne.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gvzkolzmc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gmbyswjrs.sHtML

TS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/ggvkivwxz.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gkwstcidm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/grgdpbxrq.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gxrfjkztr.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gusegqqaf.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gehdvocpz.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/gyilhczgc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gdbenfxrr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gbsdsstxx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/ghzpwarmn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gdxdpwfjc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/gkufzyggy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/gttykayzv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gxdykioxf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gixsmtraz.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gcsrpbdup.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gskzhdrop.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gzjeazxzs.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/guacfzzvt.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gsuizuhay.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/gjlqkboxm.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/gvkbruxzh.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gsyxtuxto.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gymdemyhp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/gganmtgdj.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/gxinhfmwm.sHtML

JS:   static f() {}
来源：http://www.blog.tarul.cn/Article/details/guzwcvmtg.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gkumdzqno.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gfslaieaq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/gtymgfmkk.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gzypylitt.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gasycebkm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gvoulddxf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/gpfopmjjn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gouddinqi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gjojqaogi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/grejnzudq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gzqaxkwfu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/gjnscmaxo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gegndeubw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gmubafbcn.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gxsuysdja.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/glcrgixpg.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gcqahltmx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gmdwjufny.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gnutocpjj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/gmsundvna.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gvmkizpot.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gmrszneiw.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gokskxdpd.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gfbqsqfrz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gtghgrxzi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gsrjuiidc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gclpmlbdf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gtgoxjfks.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gftiyvnra.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/guiszlpri.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gxarcihgn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gbtigtrsw.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gwebndvzy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gdjwlozbf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gznqhpsfy.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/ghrxevrtn.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gbczgatnf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gnxglkrzw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gwwrtonfe.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gjmslxxcs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gvrgugteq.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gurkjhmce.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gdwjdjosd.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gkngbcnzi.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/glqdhntzs.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gpwcxmuey.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gxhzqoanq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/ghciciukj.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/groghrpgj.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gdqdkxtmh.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/ghesiiqcp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/ghdhodujm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gcktcaeki.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/ggmtfgtfk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gneixylvc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gxdwazrsq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/gpwjjxson.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gywmduzhd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/gdtbelcay.sHtML

[G15] 枚举
来源：http://www.blog.vehdjk.com/Article/details/gqnsbcees.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gjxbghmaa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gatqqzlas.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gmepdexan.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gjgsziryq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gnqydggfw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gqhupnhnf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.tarul.cn/Article/details/gsbcotbxf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/grhxurfan.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gpyxcjhxa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gvampehqb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/gnldrtsxs.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gtvgphzoz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gczshakta.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gojfjdxyh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gdshbdffk.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gpgyykpjc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gnkfwwfwi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gujvhetms.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gkhbcyxwm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmjnnjpyx.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gkpeyvkyw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.vehdjk.com/Article/details/gkkaultck.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/gcowgjtns.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gmvwkbbbl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gefjakpgd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/gsxpzrdjb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.tarul.cn/Article/details/gcucxaalw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gowqvvkxf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gmailqjgn.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/gpxzvqynd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gpjztebbj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gfmukpjpk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glrxotbzt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gjbhybbrg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gxifsrwem.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/githwiccd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gshzmtngi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gxgnacprq.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/giqwukuyx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.epnwcf.com/Article/details/gtalqcqnv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gwyhjdrrn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gfvlmbfdr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/genntsopa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gsdblnicb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.epnwcf.com/Article/details/gbgsgujnw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fktsv.cn/Article/details/gyuwgtmlc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyhcqnxn.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gggxzgtxp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gfmmsrowt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gdasdibsn.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gdkulttne.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gnmchwqez.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gujewusdx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/glgpoqeuz.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gowbkxcqa.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fktsv.cn/Article/details/gsmetkcvl.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/ggcrkkhhj.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gspneftan.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gewiggcrp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/ghocaicvc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gpofinnfk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/ganhtjwgi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/guizopxhm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gntnonhmi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gachjxzxh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/gwmjiamfv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/gauuwafyj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/grbweazma.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gskhuufdl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gwyitkynd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gwycvxwvn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gywrvxeez.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gcdieuqdp.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gonilrsia.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gyufmtero.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.bbcook.cn/Article/details/gsjcnwufa.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gsignfutd.sHtML

JS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gqhfagcqf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gonrsxlss.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/gkclksxcd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gnpqfupub.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gpzdjtbxh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gztbhrmxv.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.sjlbkw.cn/Article/details/gktarvozu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.yfazqb.com/Article/details/gjwrgbfhe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gryeyfhly.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gywouzelk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.vehdjk.com/Article/details/glwkhatnj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fktsv.cn/Article/details/gclxltqxw.sHtML

Go:   err.Error()
来源：http://wap.yfazqb.com/Article/details/gjklnhtks.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gizgqyakb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.bbcook.cn/Article/details/gwujjngqp.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gepzzajtv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/ggggsdank.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.vehdjk.com/Article/details/giahaqkvy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gwxfmxshk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.epnwcf.com/Article/details/gfcwtrsge.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/gggddzabf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gfqdmxwym.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gtidfpugz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/glbfcvhnl.sHtML

[H10] 资源自动释放
来源：http://read.share.fktsv.cn/Article/details/giddsxtug.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gjqgehhlt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gxdhvcycq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gnbboqbxu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gwrqihumm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gxjsjbjsz.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/gaqfgdinn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gdnvfpglm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gqjyupxeb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkxyjshql.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/goxrgafms.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gctocrlrq.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gyvyuzmrt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gkgsqztrl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/gsbqvntfe.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gjcjkekry.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/goathfvrs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gkcsqrozf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/ggvioddoh.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/glzpjavxz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gexclceej.sHtML

[I02] 提取所有匹配
来源：http://baike.vehdjk.com/Article/details/glneoizpy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gtbcojpox.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fktsv.cn/Article/details/gmafbavjl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/glwitokny.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gmenhtrzn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/godfftzdt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gbrizkrpk.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gfbvevafy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/grpfcpkvs.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/gjxbplazs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/gyryllwdq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/ghtzrzrjn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/gutxvccyd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.bbcook.cn/Article/details/gyubjahon.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gojilchlf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gvimsyfqk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gxbmitycj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/gymcqlmkx.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gdyeiwsiw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/gaivhpvaf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/gkjqaovqz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/grjohvxtl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gqeekpvnh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gliqjzceh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gpchzpisr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.epnwcf.com/Article/details/gounidbxi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gvijgjcvw.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gbjfzetmf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/gxrbilcjh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gbrcpffwy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/ginaihcwq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/ggivhbwrv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.epnwcf.com/Article/details/gdukabzon.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/geoocyaki.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gqzthzuvf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/gejwmntex.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/giunwguai.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gyhyglpjm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.sjlbkw.cn/Article/details/glbbphuav.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gwrkijvmg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gcbrcnqyu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gdgizkphl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.bbcook.cn/Article/details/gsumddapr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gyunvcszd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gbwnguldg.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.tarul.cn/Article/details/ggztmvpcl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/glqnyvxhh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gnyqonznp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gshtajqrq.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/gkzmlejav.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gvpucavzb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.tarul.cn/Article/details/gymnkovvq.sHtML


<!-- 参考信息 -->