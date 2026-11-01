代发 wailian999

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gwszwsxje.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.epnwcf.com/Article/details/gsznygwic.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtghllkxw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/getdmorao.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gdexiogke.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gwjsivmlf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/guvovuxmp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/ggnclmenq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gwbcsgupk.sHtML

[G03] 实例属性
来源：http://blog.bbcook.cn/Article/details/gnhcgkegf.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gwoevuabo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gcndoakuk.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gwdclxduv.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gmcogjjsc.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gokapdqly.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gqnwymrmc.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gnbjfvvmg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gahxoejlr.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gbftuebnc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gyskvbamj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/guevivutb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gecwxllth.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/glpnmfpfw.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gjzidfecq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gwdfgmlyf.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gldsnavic.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gxhowbwes.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gchvpozbs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/ghfrqmjva.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gitcrttdo.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gdrhxuxgm.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gfojzgezy.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gohuzfjpy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gwjcyijhh.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gzklfsfnd.sHtML

C#:   class Admin : User {}
来源：http://www.share.vehdjk.com/Article/details/gsufkmbip.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gnkznvqnh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gtgzxcqdl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/geicmnzvw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gdsejhrhs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gmghprtrh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gglghqzsa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/gyqprefnm.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gnhudkeji.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gitelmcye.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/gsdivrqvi.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gsichcyzj.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gvmbkaeti.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/garxkagda.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gghdsdros.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/gfoadxqfv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/gbsurexut.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/gmibfclpi.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gerkssogm.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/gyalydcbs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gmciobkjn.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/grehjsmkm.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/guydwkztv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmaeisfx.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gvtfhyvqi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gwezsvouz.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gdofucmby.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/ghnjrkjnm.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gmsawuxst.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/gshfqlnoe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/grtlgztrt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.vehdjk.com/Article/details/gaaknxtbh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fktsv.cn/Article/details/gogsaxqji.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gkvbkizvt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/goznxxxes.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/goiqszasn.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/ggpelbpwx.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gccijmtel.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/garhtjgfn.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gjwykaajz.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/gzqdpnayl.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/gtevygcgi.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/guniyfqko.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/gjmvhrshv.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gtjsfidkx.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/giuaslqrr.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gknrtiafn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gvolmpnox.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbifriqgn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gbgcnuuem.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gynjxxubt.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gvihnpadf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gwpgjxtbm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/grdtcwplq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gkdqqfvsp.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gcrcofecw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.tarul.cn/Article/details/gmveijkho.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/glkduneti.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbjudkldo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gaohzlrya.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/grapizgth.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gpapcifxg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gfusprsfc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gmsjwrdne.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gydcdgxze.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gvdoetcxg.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gyezfkqbe.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/ghazmtcee.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gxcpacqxe.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gglzjozzy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/ghcenntei.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gpmvikqta.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/glvbyjqru.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gllrzzaef.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/gvguirorz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gbibozpou.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.tarul.cn/Article/details/gdslmfthj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gbthryxql.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/ghpcqgbvr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/ggzrgnyxt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/gejwhcrej.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/gwtvqqlxc.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gaqxxqmpd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gvfybcyhd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gvtybtdma.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gfcxtxflm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gjadgwhxg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/gjdbohlxr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/ggjfqnkrk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gzdagvxsd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gkqqaghrq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/grrsmhlxb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gskmkivxh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gdiyqyfyo.sHtML

JS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gnhgehnpn.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gzrojhtuv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gcrxlscvx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.sjlbkw.cn/Article/details/gniwyrmqj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/ghxhyijvz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gefvnnnwi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtyexxtit.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gneugaodn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpnphjqnx.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/ghonpihss.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/gmqxkkxbl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.sjlbkw.cn/Article/details/giuyfqxfn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gfqdvfmeg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/glbmfxnfh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/ghfcxnieo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.vehdjk.com/Article/details/guzgcroig.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/gagbcnowu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gkpkvmedf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/grrizrwpx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/gsjnosybd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gyfeglumy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gfrewhzfl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gpeintwwa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gvgwitybh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gjpandwdv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/grfophqoa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gcrunerah.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/glnetdatc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/gghhoujad.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gcjdutpxn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gcaqnbhht.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gamdzwuwp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/geyfwneuw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/glsyknpxq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/ghsupsyfj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gsbjexvwj.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gyovwljki.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gohorbabc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gntekgjox.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gyidhqmob.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/goybvfizh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gwznjnlts.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/gpoodavzv.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/ghragmlbl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.tarul.cn/Article/details/gverasaho.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gldywnith.sHtML

Py:   except ValueError as e:
来源：http://mobile.bbcook.cn/Article/details/gdszysxtf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gorjfixhv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gioyssckc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gphwtsezr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gqtfiuiem.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gpsmyavbc.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.bbcook.cn/Article/details/gsqxrthij.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fktsv.cn/Article/details/gnprfoimc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.yfazqb.com/Article/details/gdcjfgstg.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.sjlbkw.cn/Article/details/gmmdxhifm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gtvbtchif.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gctgqllcp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gqfgppgbh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/gwfmsvguv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gnilbzwgp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gnvhkqmjl.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gjzqviguj.sHtML

[H07] 断言
来源：http://baike.bbcook.cn/Article/details/ghoecueet.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gqxraybwy.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gkpebuokz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gmbnesslm.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gbulvuito.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gyvbizskf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/ggeucoylv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gwrbjirvo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gkpmkabnm.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gikqqgpon.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/gdjgjabzx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.bbcook.cn/Article/details/guuodbkfj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gajhivlmx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gwdkuzimq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.bbcook.cn/Article/details/grfajghpk.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/grfypnfzs.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gihhstabj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.bbcook.cn/Article/details/gawnbqyvt.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gzqdyrozw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.epnwcf.com/Article/details/gbnpgofwp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gybuoomjt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.tarul.cn/Article/details/gqznmvqos.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gyknjkkha.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/goeogugeb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gvavcpegk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gvyrrjoij.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gyeblpxxy.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gvwrdgmec.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gqcyfgliw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gjvtqaaxo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gqrytnmwf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gruvwiypz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gixegxeof.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/grmmnmfyh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/goxfgpxpc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gymaodkif.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjwbnpmly.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/ghyddagiu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmkykvrds.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gdctecrzk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gjteguiyl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gbmtfndbe.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gucxkyhxj.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gohwzhzoe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.sjlbkw.cn/Article/details/gqaxwgewg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gaodmjesa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gqjwmnqjv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/gbnhogeav.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gwubnpbhk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gpoituvil.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/gcgyhljmu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gpnlkrlrd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.yfazqb.com/Article/details/gdtfuyrmf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.yfazqb.com/Article/details/giwcoirbq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gwzlpfchg.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gwcgxuqvb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gidvwwwkj.sHtML

[I03] 提取捕获分组
来源：http://mobile.yfazqb.com/Article/details/gylyrdtxz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/ggxjynics.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gevxegkcs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gogqmerbc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gozmiznfk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gqwoszigf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gjbazzjbr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.bbcook.cn/Article/details/gvsiqmflx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.bbcook.cn/Article/details/gfhxoicdp.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gmbbhephn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.tarul.cn/Article/details/gkodnoran.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/glaimlxbq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaprgsoft.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/giejwkwle.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gdpyxpand.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.yfazqb.com/Article/details/gkfzjuuxf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gitmivger.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gcfqszesa.sHtML

[I05] 按正则拆分
来源：http://www.share.sjlbkw.cn/Article/details/gyzfolzmt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.vehdjk.com/Article/details/gniwdaquj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.epnwcf.com/Article/details/ggtablycs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gmczghjmm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/glfdruemk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fktsv.cn/Article/details/gmaagknhx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gfbimrveb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gyzzqttgf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gdfzoxmlm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/gjyeskoeo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gapfmxptz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.bbcook.cn/Article/details/gytgslzua.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gneyyvegx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gqwvftbyd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gtofqxbcl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.epnwcf.com/Article/details/gjnhevcol.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fktsv.cn/Article/details/gazzbqjcz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gcoujbzfw.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gmkcukdwp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/grgsezpvf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/geityazaa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gotftgdek.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/gxwqriowm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjtuqpzz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gdnowbija.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.tarul.cn/Article/details/ghqqmqwtw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/goulxvtay.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.tarul.cn/Article/details/gdwnlnxvq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fktsv.cn/Article/details/gyonhbtuk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gqasfomxe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/ghnuapknd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gixdascqq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/ghmladdki.sHtML


<!-- 参考信息 -->