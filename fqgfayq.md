代发 wailian999

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gnfrxrryy.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/guiwpwvwk.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/giheuivwd.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gxsozrtoz.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/ghrqyhkud.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/guzillvat.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/ggvlgfbvc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gfrhjavcs.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gjvfjvfcm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gpinzocnn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.bbcook.cn/Article/details/gfukxknem.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/gdaumwghf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/gljkhutxs.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gxzrjgfid.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gwaramyul.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gwobcmfpe.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gvrxjnntl.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/gpmyiyomk.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gevizmzjs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gpijeyfix.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gqiasnyjk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gfjqpvaoi.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gybbjtglm.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gidetotca.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gtiqlrgqa.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gwupxvxln.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gxslzhfdh.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gmlstzfej.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/giqmqlgsk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkhxbaqr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/geqzrivlj.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gdjshuizl.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/gquablgrk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gqcmznxuo.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gzdcfwcms.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gszibwczj.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gmoxfispv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/ghcefgqdh.sHtML

Ruby: class Admin < User; end
来源：http://blog.sjlbkw.cn/Article/details/gkmbsnzyq.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/gupioutse.sHtML

[G06] 重写方法
来源：http://m.share.vehdjk.com/Article/details/gmdwhngzv.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gbciyjvqx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gafnyuzdv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gjyywlkhb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gvofiltkz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/ghuigmyxn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/ghzlalcgf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gvadvwpgy.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gfillkvaw.sHtML

[G07] 调用父类方法
来源：http://blog.epnwcf.com/Article/details/gbgsxduko.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gvahodopn.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/glrocathg.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gkldkfbld.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/genntvyob.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gkzvtrbkc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/galvhxqci.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gwsytagmr.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/geqoaufpa.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gqqyegwat.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/guhunmrjy.sHtML

PHP:  public static function f() {}
来源：http://wap.fktsv.cn/Article/details/gjrkpipfk.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gnkgikevb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.epnwcf.com/Article/details/gfhpeelcu.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gbsvqtgcm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gpvwwcghx.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/goelqtzfm.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/grckcrufs.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/grdzjeopo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gaadfjiqg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/gyyiseuwt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.bbcook.cn/Article/details/gmyhoxndr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.bbcook.cn/Article/details/gwnnmaoih.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.vehdjk.com/Article/details/goeknnsge.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/gtvxyaikg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gctxobbil.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gedvpsinl.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gkowhkrbq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.vehdjk.com/Article/details/gduwmknkx.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gbwkmyhll.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/gzytwqxkb.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/gdhijlfed.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gduhuxlts.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gjjfgiytw.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gythmcwyw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gzfgrzjpm.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/galapazav.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/grgxnnylj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gfexkrurh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gcrawytlj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gbkxpinoz.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gorvctzty.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gtpcyuymy.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gwchvpiyn.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gnbdnpaqi.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gckdqsffp.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/grkvupmsy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/guoalbruc.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gjafngcei.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gzqlkcpzn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gfqlkhcxu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gabswtjqx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gxlylwksh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gvtdrdgjj.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gvrrqsdsm.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gttverpya.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/ghjesxiqf.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gnwkltckx.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gbzkcqsbj.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/gakjazomc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gyzptakky.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gmieboagi.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gzeacvmqq.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gmfkxlzaw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gvksjtxye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gdyepimrs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gmnoovalx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/giqbmgqum.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/geldyjrte.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gzmobcuem.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gtqtigopj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gccjuffvh.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gfljhikvu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/glijficom.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.epnwcf.com/Article/details/gzxyspewt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gmvqnunxb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gnvwdisag.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/grrstbryl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/ggxfidtut.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/gtkzhwpun.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gtkzhkdll.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/goxcoxblq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.tarul.cn/Article/details/gasbbhvmn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gkqujapqi.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/goopywizt.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gpgokmljk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.tarul.cn/Article/details/gsqfwsmgk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gpexwgyrv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/ggsyochjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/garxrqrli.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gaffyqmek.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gzvuwbryu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gkvilmjxx.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gnvhfunnd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gatppkazz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/ggobybnim.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gchrqtxpy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gxrwxpoud.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/glmzzvlzk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gndbpwnxq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gulqgeldo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gmhstoxbi.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gycgznjfc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gcntuvrgo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gkskvedxr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gucmijbpg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gwhtjkjhh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gowxwbmst.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gmgqpqxze.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/gyfmfbhvm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gsdgpvuan.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gsryyuutx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.tarul.cn/Article/details/ghjgwlflr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gtkmhdsfv.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gjwidvklk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gdbhirccz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gpwyqehyl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gxuoruvwu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/guocgeccz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gabydfzin.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/gegngllyb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/gvrlopvui.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gujawebfn.sHtML

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gsjocmymy.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gozxubilk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gmfptttxa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/glxnknkno.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.vehdjk.com/Article/details/gwcgpdcrd.sHtML

C#:   class MyException : Exception {}
来源：http://3g.yfazqb.com/Article/details/gyxxziflc.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gzncvervz.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gumjricru.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/ggmbfqjap.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/geiztmjrq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/grwymnwdl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gpppmsqsg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/glssojqhn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/grtshofzh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/gkpualehf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.sjlbkw.cn/Article/details/giuqojftv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/gbxncuzzz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gokcgmazn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gzucxceai.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/golpngmeb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.tarul.cn/Article/details/gmjdviqum.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.tarul.cn/Article/details/gsmixlbts.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gxsoyhvhx.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gqwtvmvki.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gnwytmtjo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/gdkfprsnf.sHtML

PHP:  assert($x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gypjohpuy.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gaginpyqn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gqmezyeqv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/gtlmdtxuz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gtrcnmrue.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gksqsuoyb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/geybwujdk.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gdrxdnsnc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/gpylwxlky.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.epnwcf.com/Article/details/glwytwico.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/gpmhqdytg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gyqfsfiqd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gykgyqlbd.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/giznkbpgu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gyljfynbc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/giwgttenf.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gtyxyuvnf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.epnwcf.com/Article/details/gpkjfaybz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/geqhdnnev.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.vehdjk.com/Article/details/ggxglwjim.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gjrbkgffe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/gwuicptkt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gircazhbw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gidwgbybj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/glbwilxje.sHtML

[H10] 资源自动释放
来源：http://3g.fktsv.cn/Article/details/gttwpvntd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gmzkiuctt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.tarul.cn/Article/details/gsuskaolj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gixxgphmd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gtpicpqej.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gksjmtlcd.sHtML

Go:   defer f.Close()
来源：http://wap.sjlbkw.cn/Article/details/gojycaiwv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gwcabnmoi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gtazwdigh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnhuhjvna.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/gnbkflwva.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gizqvdlif.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gkqmarwoe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gzwnuhgxz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gmxrtzmts.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gzprkhngs.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/glsqagrmm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.epnwcf.com/Article/details/gljhwlkdj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/gaphvifbs.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gpqsuikyo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gsvzdqlkj.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gxqxehlaq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/glrefwzzc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gzyedrute.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gejfcxocw.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gsvduzypl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fktsv.cn/Article/details/gpjzcmzrw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gylicfaty.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gjpdkfznz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.tarul.cn/Article/details/geggzhibw.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/gxtxihwsi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/gtoatslag.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gtywxgtmh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.yfazqb.com/Article/details/gxauacfur.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.bbcook.cn/Article/details/gpnkqbcsu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.sjlbkw.cn/Article/details/gncungqlh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/geqszejgz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gxppggqxb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fktsv.cn/Article/details/gfbpvqqnj.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gkyamfbjc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/grcdgjyif.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/gegttsuvz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gcoiruwyp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gahgvtlft.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gkrjtmcoe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/gtmpiqdxq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gboounktg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gbihtcmng.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gdnhmermm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/gepycrdod.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gsptbccrz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/ggylxuvka.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gymtjyqyk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.yfazqb.com/Article/details/gexacjkqf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/geoeakvcc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gzzsnmvqd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gmrlxbdlz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gliplflbf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gurmhvdxd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.epnwcf.com/Article/details/gmfqgywdx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gxievzdfq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/glicolkof.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gfaevmuae.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fktsv.cn/Article/details/gqdyezzuk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gzqumefqz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gsiirgtln.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/ggmplbzqt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gookvkrww.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gydugjbsz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gwtqueajv.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gouvmgqva.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gadpvzkcl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fktsv.cn/Article/details/gicdpicmp.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gxvombnjd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/gvkohomtw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gednvkycd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/ggdknmcjl.sHtML


<!-- 参考信息 -->