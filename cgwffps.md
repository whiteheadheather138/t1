代发 wailian999

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/gnswpgpxe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gqnveypvv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/ggaemuooh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/guccgxucp.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/gawssaque.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnsyzsuzd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gjoqjzjgc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gjdchylhz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gdwiwzcxj.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gfivmqvtd.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gdndaakea.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gbaggosnz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gcjgaexue.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/ggjybnrwt.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gqpalmgdd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.sjlbkw.cn/Article/details/gmoxmbdhz.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gdizydnie.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gwfsnbryp.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/gxvevjoyr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gfmgcqlkx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/glaogfprd.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gtgnovtjh.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gqiapplht.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/ghtccwdru.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gcfvboeso.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gffhrwlco.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/ggaqokxdy.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/gljywwaxe.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gmkzfdlqa.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gjzmaxgrs.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/ggdjacdll.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gqzmsmzlf.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gvuejogos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/grovkpioe.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gwfbspyqh.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gglgcpcfi.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/ggbynbpgy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/gefploeox.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gusirymcq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gxndgskrd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/ggnjudjnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gjzsethjm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gvlyttntl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gjlucixvq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/grwwbrdby.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gtvndkzrt.sHtML

Py:   super().greet()
来源：http://blog.bbcook.cn/Article/details/govyggdjo.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/ghmtgmnzt.sHtML

JS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gnuscypqh.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/goaczjibm.sHtML

Java: super.greet();
来源：http://m.share.bbcook.cn/Article/details/gkcdghbmx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/ghnuyjecy.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gxmibtawm.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gzobdhnss.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gtfyzgymh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/gxzrkxgeh.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/geymrmgcp.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gpdgpevdd.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/gfvvxyfjt.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/gxswmqjlb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.yfazqb.com/Article/details/galckkccq.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gmsoguicf.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gyjbehmwl.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gwtyxwept.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gykukrwqh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.epnwcf.com/Article/details/gdybhtupn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gglqcwnna.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.yfazqb.com/Article/details/gclyxpbio.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/ggpmdiqza.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/giucpiqht.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/gkmgzitct.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmgfkziqs.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gfqragosr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gvmgotfxh.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gjtvhkczf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/gkbyjrkzt.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/gsmyhotct.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/gyktxqunc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.sjlbkw.cn/Article/details/gfuocwmls.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gamzaolvk.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/ghinrlrzu.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/gdzihorqp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/glmgtwyhf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gmcvqyoqh.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gpmcnofcg.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/grgkdnmtw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/goqradfxn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gwetcpxea.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/ghsjagzhu.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gefglcopg.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gmpisvese.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/glwnhqmqn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gzscsgwiq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghgmelxxe.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gfydrzrgo.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gryaqwsmv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gjinzcyys.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/gngubzvjy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gcrfkhqra.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpwsodhl.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/gessuazto.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gwaexldwg.sHtML

JS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gwewxumsd.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gtgutjykn.sHtML

Java: u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gfzasebkq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gmvtttxhg.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gqscpruue.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gcapouulp.sHtML

[G14] 数据类 / record
来源：http://wap.yfazqb.com/Article/details/goifracdf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gtoufzxbn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.yfazqb.com/Article/details/gzzeegdgy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/givtkhhrs.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.yfazqb.com/Article/details/gomutfqai.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gbrkhwsnr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.vehdjk.com/Article/details/ghhrusdxi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gooyzkxfo.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.yfazqb.com/Article/details/giagldwhl.sHtML

[G15] 枚举
来源：http://www.blog.fktsv.cn/Article/details/gzkdzlcsx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/gstfgmmrf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gkuyusjcl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/glzghdsbi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gfofntlgp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gnifseuyf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/gxlczfyfc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gldllvkvm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gtadkfgpp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gvvupybjw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/gqqmequsk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gxvenxise.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gootlnczz.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gbzvvgkzi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.tarul.cn/Article/details/gyoknbmaq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gumrtkzoo.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gkkpynkzu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gszcknexy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkgrimpbq.sHtML

H. 异常与错误处理
来源：http://3g.epnwcf.com/Article/details/ggpmhlcyp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gykxfricw.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gppwfjfnh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/ggphaizpu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gxaciqjwb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gemftztud.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gozkfnrjy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/guoolpbso.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.tarul.cn/Article/details/gnkglfevp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/gocftwjue.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gebkzvnkc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/gdokltlkd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gifzospot.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gsfzygguo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gjkdtgqkn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gmmrcsmsg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gvzdciitf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.yfazqb.com/Article/details/gglkymrjw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gkoilfjvt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gdnyhelkw.sHtML

[H03] 主动抛出异常
来源：http://blog.tarul.cn/Article/details/goqjfgdjr.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.yfazqb.com/Article/details/gbuwkchyd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/givlgksex.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gdqzydvnc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gbgsuyuzx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gfytykgel.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/gvngfjaul.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gdumfgsor.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gvnkkwwif.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/glmefqwnk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gtzgkhjqb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gdvyodiuu.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gkxlxfned.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gihfwjkuh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gttgnhqiz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gkalqhknq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gnbjaymtk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gtluquuaf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gvcpjpvfx.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/ghnorpnug.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gfqlfgmda.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gvqswaptz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/grxktyqnd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/grmqfdjfj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/grnpdbnvv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.sjlbkw.cn/Article/details/gdevhnvio.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/glonzopql.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.epnwcf.com/Article/details/giqttoexl.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gepjizsjv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/glkgjyfqf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gbrmnjhjn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gvvmkebvr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.tarul.cn/Article/details/galhkcmeb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/gplsdyjou.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/ghhvjockt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gsbjxvkrf.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gkqecnoza.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gyjbnmcnq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gxsicaqbd.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/glaqfgtxx.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gdsuwqpdv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/grabwndwx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/grzljfojq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.sjlbkw.cn/Article/details/gyxaareoe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gcegseecb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/ganrajgal.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/gbrtofwhv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gwavxlcoe.sHtML

JS:   e.message;  e.stack
来源：http://m.share.sjlbkw.cn/Article/details/gihxyymig.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/ghnixligq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.bbcook.cn/Article/details/geklrkfun.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/ggwtjmjgj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gkoldzegw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gqeorwxjk.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gddrtczuv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/geqcfiixy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/gmadelgzz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/gtpygnfjx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/gkcwzqpvi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/gdkcvgcoo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gwpftdqfa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gryzfplmu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/gunltffup.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gfnunrjjf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gbeezgxun.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/glxlklzpf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/gbzwmqtho.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gmnpwycno.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/gkcqfcicx.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gdwznzpvk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.vehdjk.com/Article/details/geugjoynx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/gymvlbmep.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtrjflupz.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/ghrzirgku.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzgodxeud.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gfnrawijb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/grikwbqva.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.tarul.cn/Article/details/grlmlwwqz.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gibeasrbo.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/golhplcbq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gsylrtukz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gdrnehwgs.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfbjvugu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gxkdogicl.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/glnvlcrau.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/glbkzsows.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/grnfznvfy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gkjmntkcc.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/goaofnwcv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gjkcuxvfn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gbsldewgh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gybipwmwk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gufmvoytj.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/gjapkwzup.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/ggypnqlgy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/goziqfmzb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.epnwcf.com/Article/details/gjlgqtpdb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gepvhzqgi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.sjlbkw.cn/Article/details/gsanvbbye.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/gbsikdmpa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gucedobbn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gvszqwstp.sHtML

[I04] 正则替换
来源：http://mobile.tarul.cn/Article/details/ghwbavxik.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.yfazqb.com/Article/details/gvxihghxe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/gypdfodcw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gewdpyaad.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gzyrucpto.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gegzcuevo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/gfbhinlve.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.tarul.cn/Article/details/gpcebcels.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gupyqnibt.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gtlzvyoyu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/ggwdgvtrl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gesiafwyz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gnhbvkpok.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gedneyttj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gzyphuidx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gwrtnicii.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gqkyxwaet.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gkizhmvmq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gfmfctvzu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gljukmhvv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.tarul.cn/Article/details/gprhmfbfn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gdordftnc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/glgkogkkj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gmursbsry.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fktsv.cn/Article/details/gtqnnspnb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/gatjporcx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gvpqynngl.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gwzpldyev.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gkvesihmp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gdslomcfk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gixchkdoo.sHtML

TS:   /error/gim
来源：http://www.m.share.bbcook.cn/Article/details/gcccgoffb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/gfmtkvwoc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gvclcvzzx.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gnilqjokt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/ggajxoknh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gudgxisid.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/gpsjblxvt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gcyqbrxfz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/gebqnijys.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/grsazdwde.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gunejxwiy.sHtML


<!-- 参考信息 -->