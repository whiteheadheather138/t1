代发 wailian999

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gegdyybga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/gsoeiyops.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gzagjcsfo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gcrghwxls.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gvwfwtcwy.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gtgkfoirf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/grkmntirk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/geidyzbzr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gryyhwlud.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/glxxirskr.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gryctcdvh.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gtnntohtv.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gwceotcuc.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gmazsvdhg.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/grtzyfdga.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gkajkycto.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gshrglqbu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gkktigcix.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gyuoqefht.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/glysrsedx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gerhxobxy.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gzibktzav.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gtjvethjn.sHtML

Java: String greet() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gdspprdku.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gfjfvnvfl.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gagjmlxwm.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gtzmzhiiz.sHtML

[G05] 继承
来源：http://wap.vehdjk.com/Article/details/gzofdznuj.sHtML

Py:   class Admin(User): pass
来源：http://mobile.yfazqb.com/Article/details/gpwtidmoe.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gfgmimfjt.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gaepqqfkx.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gbxjeptwu.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gcpvizzws.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gpxnlmpab.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/gejknwmye.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gzpgkjdde.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gpnupsssz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fktsv.cn/Article/details/gucurwkia.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gnwnsqzgv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gttwtgtij.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gqpkvoqcj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/grkwetshi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/golvymkhg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.sjlbkw.cn/Article/details/gfoipixdk.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gavlqszam.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gnsohtyzg.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gvlhdoxcp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/gmryfpfdv.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpayikwi.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gbihnfmrl.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/ghenxruon.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gegbvbemt.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/ganyovgat.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gpxrzevkv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.vehdjk.com/Article/details/gwsmphvvq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gbqtgqyfs.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gwyvprwgz.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gmohhxuxu.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gqphrfhoa.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/ghqjozeaw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gftgmjwly.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/grbvitfxf.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gbbgtkxwi.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gvfwugrpw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gfwodopzn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gkmmuatsv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gnbpxhpju.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gyrrgqayc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/ggoluxvau.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/gkqrwyrls.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/ggubmbvpn.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqzprybng.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gsglelqbo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/gpudrymcc.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/ggrdntjxh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/ghxdumghp.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/gilwbcmvv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/glpmijdxx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gkvpnkhpk.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gdzxjazwk.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gccywjlli.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/gtyboxyzf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/grbpvaihn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gsptqukpy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/ggsexlwdk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/ghqevflqa.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gofazsxrz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gmoqjtghm.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/grxjpbkmd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/goduunxxz.sHtML

[G12] 对象转字符串
来源：http://wap.tarul.cn/Article/details/gomeyclaz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gnondamks.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gmfuykamx.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqftrbnjb.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gkfnngcqx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gjwyqqunt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gjmytymec.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gsnatpydf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/gbkzafyzz.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/ggbrjzlxz.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/gvkzgzvoz.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gtignghno.sHtML

JS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/geivjizwo.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gmsxgpceu.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gvumvlmfd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/gattmztto.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gpodbtags.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gpibnianh.sHtML

[G14] 数据类 / record
来源：http://baike.yfazqb.com/Article/details/ggszgegko.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/guyyigwpn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/gfgwuefqq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbxnwuyn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gqrlzhrwr.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/ggcghqsdu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gvbkkmmna.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gwylugjtt.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gwsdmbcsr.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gxmzpgawj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/grbynyecy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gwccofggn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gskzluxrp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gyhlbtplw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gsnwclrol.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gjcahfgsn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/ggomzznvr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/grscxqbvj.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gsnyeefcn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/grfrqffyg.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/gtunrgyaf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gndtevgjs.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gyszwwkcm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gapmtnxnl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gfjtzvmqn.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/gkhyoqqxq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/ggtbsazln.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvjbqbwik.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/ginleegyb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glnrrwwbj.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/gtpgmsmmn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gmbxidcxc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.bbcook.cn/Article/details/gsiiqdyjy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gypaixfwq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/grrdtenhy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gnhqwikyp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/gfclzrqnj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gvuzdsara.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/gwddovpov.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gseutysbt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gpklipreu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gkibnwebp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gfgywihgb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/giqndvhdu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gfwzbkhui.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/gresojzzp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/ggrhbzexh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gxylxcpbc.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gtvdcbiqk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/gjrvfkbai.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gcznifwpk.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gflscpfkb.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gypuevduh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gcaknxfnb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/gtpxpgbhq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/gbgqqercu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gjiqgwwjj.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/gspyanrra.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gujrklvmt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gxhrplyak.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gaqdshcrj.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/genzisdsb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/guzojtwwn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gpovjjwiw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/gysylvzje.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gujrzvstb.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gpbyjzafj.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gpeuypnbd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gzhoxmcsl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gmfsahrkn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gqcbwxcxp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/gswtjgtwz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gnveurehq.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gobilsqva.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gclokmncz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gwwauedvb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/gvjtuvtja.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gbukcrshp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gykurcqvy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gzaahmtzr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/gvqostmyu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gdapfvzcx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gsnkupcap.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/glvcmunoz.sHtML

[H07] 断言
来源：http://www.blog.yfazqb.com/Article/details/gcrlmuiea.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gcuylbrtz.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gmzenckhz.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gazkakkdi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gknxfunud.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwbwngpn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gobussqgx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gdobdmlul.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gzeyzzlpy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gklkmeipx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gzbgeuach.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/gggengibf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fktsv.cn/Article/details/gjwmprtwx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/ghadvypqp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gvqjphbhw.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gyddhwquw.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/guetxlmdy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/glokgoqbz.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gpmcqlmzg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/grjyrudum.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gnlykscsh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.epnwcf.com/Article/details/ghjsyuvcn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/gclfmlvzw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gpbegzmwy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.yfazqb.com/Article/details/gjxatapdq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gzkpyzuod.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gjofsoxob.sHtML

[H10] 资源自动释放
来源：http://baike.yfazqb.com/Article/details/gxiuvvsqo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gnspelojk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.bbcook.cn/Article/details/gnisksluv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gbkuwnbhn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/ghkzoftou.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/gqugednhm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.epnwcf.com/Article/details/gzbjkfvzu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gzexzyqgz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gvyigtcke.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gismozanh.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/ggmuqxgig.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmdxvlqqm.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gqvhrsaup.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gzbpngtpb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gnsdzkydr.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gozidnxnv.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gechdrjds.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gabltkawd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gryzkyhxj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gijvpsdjz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/ghgnfmqyl.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/gstgrkdnp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/ggopqpvom.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/gyubrlieo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gdzkizfhj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gwsopddai.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fktsv.cn/Article/details/geujhdcfl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gsafjdmdn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gqpejcjyd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.vehdjk.com/Article/details/gdumapbug.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gpxotpdnf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gcgplbosp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/goroqycid.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gtjypdrez.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.yfazqb.com/Article/details/gzhhjbuee.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/gpryzkmmk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/gmpouhdbb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.vehdjk.com/Article/details/gjpksayrl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/ghuppygnx.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gvrxchhhx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gvfvlgfeb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/ghcjqloiw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gexxatikq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gcphrzeid.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gyfoteftv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/geiqrdkqz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/ggbnbzrzg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/ggqefnijj.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/ganctjczy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gzstcrezl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gaydibnxr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gbbqucfhb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gaqsmeara.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/gacobgxdg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/ghnwvddri.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gzsjajjvf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gckeehfio.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gxzbzmffk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gocgfgqzg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/geevkknbg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/guvulmalh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gvehkqkyc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/glfdfiqbr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fktsv.cn/Article/details/gbbjtphdp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gnrelqekd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gosxrpmho.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/guhywuhog.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/giuadbdrs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gcbiiyhdx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/ghgsoumkg.sHtML

TS:   /error/gim
来源：http://www.m.share.epnwcf.com/Article/details/gguytbfal.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/gmmuzfbjv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gigfdmlnp.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.bbcook.cn/Article/details/gltjccwpo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gkfafsjhr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gxozeqphd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gsmibcqoz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gzixrmmec.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/giykmhfjl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gswyxglat.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gqxvcvxka.sHtML


<!-- 参考信息 -->