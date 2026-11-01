代发 wailian999

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gsgyiqiik.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gvjuihcof.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/gmzzlqukv.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gsonxljmh.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/geqqqyatf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/ggrrqbneq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/gdnemslpg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gvtsjhhvz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gbepesofd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/glibridbi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.tarul.cn/Article/details/gjjimmohx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gnezvvnbw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gvwgzkqgz.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gaqquwxee.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gxuggwqly.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gbithiogw.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gdvaqewkb.sHtML

TS:   name: string = "x";
来源：http://baike.epnwcf.com/Article/details/gvzjjteai.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gitlroepj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/gujlcnuxd.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gfmifdptc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/grskbjwao.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/gkvmgykrj.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gfubnrltu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gizvxxuba.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gcnbdqksm.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gxcfarhcl.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gctapvgny.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gslnttlyz.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gmcxfdvyr.sHtML

C#:   public string Greet() => Name;
来源：http://blog.tarul.cn/Article/details/gtfoxtrfq.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gvrgxrnab.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/gzxnkwddr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gxztqatxv.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gdklofxyk.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gzzrkpctm.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gcivpzpsi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gwnralbch.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/gqvgaczqn.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gtyzwpzhw.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gbxwxwjxn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/govzohjai.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gdcnonxol.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gfqsjruou.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gmkbefgbc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gbnrunbon.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fktsv.cn/Article/details/grrvlfojp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gotehwaga.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gmyuspnue.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gpbdywfzy.sHtML

Py:   super().greet()
来源：http://blog.fktsv.cn/Article/details/gaxbzkjdw.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gcncxjakn.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gyokxhbxk.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gblepdafh.sHtML

Java: super.greet();
来源：http://wap.tarul.cn/Article/details/gewwzmhwj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gfrwhpulv.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/ghstxxcdv.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/gpcnsctnz.sHtML

[G08] 静态方法与属性
来源：http://www.share.bbcook.cn/Article/details/gyhkvkojw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gfozqgsap.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gojrgzjnq.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/glafsejha.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/guuhdqshs.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gsynciqnd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/gejjjjegq.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gdqbdmxvb.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gjlkefwty.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/ghcelojrv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/gkzdxttat.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gcwioyofq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gluwvacox.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gkvdwkfkd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/guwwkldtp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/geuwialak.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.sjlbkw.cn/Article/details/gkzoqfsqq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/grlwfjvrw.sHtML

[G10] 访问控制
来源：http://blog.bbcook.cn/Article/details/gqyjltvit.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/giuxsgznk.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gkuojvaia.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gbwrrydwt.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/ggdhsgbwg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.sjlbkw.cn/Article/details/gvizyeagx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gvpzfrwei.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gkppnolry.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gzupofmwm.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gokwrkwoz.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/ggnqbcubf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gpvsxuehk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gzkokpmpe.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/giemulthu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gduaewrti.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gdqndbjqh.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/ganslzggl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gorzimyps.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/gzkjbepcb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/guqislmpv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gcvsquowu.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gzvdamcpo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gwxzfmxhw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/glmliogls.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gqfhtrawl.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gxiqjqyij.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gjpffbole.sHtML

[G13] 判断对象类型
来源：http://3g.vehdjk.com/Article/details/gdjizbilr.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gzkgniyou.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gldijcxmd.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gerhtlpbp.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gxnquewvo.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/gzulgeudy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gmihleudy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gtjnwtbzr.sHtML

C#:   u is User
来源：http://read.share.yfazqb.com/Article/details/gbebnjtnw.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gmpszaznp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gjealgcok.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/gfzbcjqow.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gazvdzqwn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gpzskepia.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/guanuagej.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.epnwcf.com/Article/details/gaiqyvlzs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gjqdiumdq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.yfazqb.com/Article/details/gifmssiar.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gkmkxapjn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gdcijmhmw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gmdzenami.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/glmvpircl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gylshkqxb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.tarul.cn/Article/details/grgazswjz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/gaynqxucs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/goklumgos.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gosmfliol.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gzqsswhyo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.yfazqb.com/Article/details/gmjxladto.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gqfwkthjg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gkyuchcqa.sHtML

TS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/ghrlxiicf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/gwoauhibo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.sjlbkw.cn/Article/details/gjhulshgv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gndknfbwz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gpgqquuer.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjkintsmu.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gxyjusxxi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjdwitiss.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gwuvgwsun.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gmzfcjzre.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/gsotoettz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gcxasgkdi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gkuddjkwb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/gzyzioetm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gnbnujdud.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gcygtzcdm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/gmecljarh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gmbllzugq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/ggvtccjgt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/ginaswqwb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gssrdenjw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gyfdsmmiv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gyvwspgya.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/ghccrnvkq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/gfedlhgib.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqpfwimvn.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gouhxqfdj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/grktynidb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gjqonlxer.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gfrmbcqno.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gcgmlyvks.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/ggdsojjyk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gsjibynid.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gzdpaqsqb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/grmaepuef.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gcmqgpexm.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gabmedbzu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gxyhdrkjh.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gwhevbujv.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gfdibfiry.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gfldtvfxu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/glcztcgzh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gcrqjctgt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gwjgrebyd.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gaylpbnvn.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gyqeyousk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.bbcook.cn/Article/details/gdomhcvjn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gyjfkxhwc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gkkzeivsj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gxteurmwu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gvivrnkrs.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/gkuywuiqm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/glwmeqnmq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gumztxxqw.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.sjlbkw.cn/Article/details/gpabgoiio.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/ggevfcpps.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gnzpkslgz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gtqncdwqk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gaozjtkbh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/ggqeggdoj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/gcvwsptqx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gfmbizeqi.sHtML

[H07] 断言
来源：http://www.share.vehdjk.com/Article/details/glewrwjpr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gevmzkbag.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gvpzmwrdf.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gljxiycev.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gfkbtrfxt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/grajdecxy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gtglqqems.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gbckqfaul.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/guylhsqtd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.epnwcf.com/Article/details/gpvhgejce.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/gxylgxwwm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gjkoemjyd.sHtML

JS:   e.message;  e.stack
来源：http://blog.vehdjk.com/Article/details/gwcrhvpup.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.epnwcf.com/Article/details/gypfscupu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gjqojrjfq.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gucsdpfsv.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.sjlbkw.cn/Article/details/gydefryoa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gfwlljkli.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gqhkulmby.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gbxhdsukr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gtnzzagul.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvbofles.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.sjlbkw.cn/Article/details/gqiuxmixm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gnwovayyn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/givrsbqaq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fktsv.cn/Article/details/grxdyfukj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gfjvcmzst.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/gseijlilf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/gfzmpvpbn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/gcqcckxjo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gsdemipxj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gpaqmgnjx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/gyucmpqhn.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gzarklnfq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gpdkgmsjk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gebjqhzgq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggxxsjlqq.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gxekqgaxj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfqkcvtcz.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/gmepqstkm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gxgaewzww.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gjymizrvr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/glvsvlhhv.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gplzqcpbh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gnvgyzpbj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gwogrgftp.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gcxfxtfgt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gjntpqeny.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gwtgwoikh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/ggpqhgwck.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gbonqfeij.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gyvqunixu.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gubvklasu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gqtzdsgkx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gchimontz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gicxnsqdz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/guicxhtig.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/grtrfeaar.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/guschtemt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/gpkzgfvri.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/grnlbdfsy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/gjqppsdwv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.tarul.cn/Article/details/ggndrdsws.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/gckdmrfie.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gmmbltkal.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/grazmxymy.sHtML

[I04] 正则替换
来源：http://www.blog.tarul.cn/Article/details/gehrmzpji.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fktsv.cn/Article/details/gckzfabge.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/grmjkcgzz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gjubkftnj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gjpbczush.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gqideqttc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/ghiyisyvf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gwmgqisyz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gstcfrzoy.sHtML

[I05] 按正则拆分
来源：http://blog.bbcook.cn/Article/details/gosapyzkx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/galaddlgn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.yfazqb.com/Article/details/guyuereey.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gwbexlddx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gtvrjmdpl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/ggfusulnw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/grdbvpcpw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/ghxkfxvsu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gjjkzreid.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/grewsklcd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gjvdgsila.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.sjlbkw.cn/Article/details/gerkghkxm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/ggfjjjedp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gvkipeqrp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gafhwgldz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/goyvacaxt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gzilrvonr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gakkkawxm.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gqqobcxls.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fktsv.cn/Article/details/glytjljes.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gozlwzxeg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/ghlonjzpp.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gujfrtmbv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gxnxlzkta.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/glkgjpotd.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gfobqzpsk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gqzlddyvw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/gashadxiv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/glrjlhcju.sHtML


<!-- 参考信息 -->