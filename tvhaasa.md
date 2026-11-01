代发 wailian999

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/gnyszmqsw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gtlqgityg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtfctzstj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gbhzmfoxk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gstzmeubf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gfvsynuzx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gzymhobaw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gyplfxjtk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtnmyqwgy.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gpkfjtlai.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gyungbzhl.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gwhgwifun.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gwozoqfvo.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gqlwxfxbo.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/ggaqwaots.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/gnevifxvl.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gavzrlhcd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gokwoyxfr.sHtML

[G04] 定义方法
来源：http://m.share.sjlbkw.cn/Article/details/gdogxysjp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gsdueajqa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gjicaxorw.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gylqtsmmo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ginxnysgy.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gqlmcpeyu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gyudjxhmf.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/ghbxyvmue.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gddezzeqk.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gvqcnpaqd.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gemvdtqgy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gydgrxmco.sHtML

JS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gpqkaqwax.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gcahmwkmq.sHtML

Java: class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gcjscnumi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/gztzgecil.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gmovtexct.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gjblsikuu.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gonhyawvw.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gqwnpexkv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gemwfrwft.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gvtrmtwbc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gbgmxeyvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gvhejnbxx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.bbcook.cn/Article/details/gtojzgrin.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/glsfafwfc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gykptgfok.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/gxxlakksu.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/ggayedieq.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gpsbzuytp.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gtpaqhpvi.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/grsrutggl.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gwsdwzprq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gnurxnrqg.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gstnuzaro.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gjmuixmtd.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gniqclqbl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/gqlraiatd.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gcbrayzrj.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gynczkovl.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/ggqpwiiyf.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gldyikoxo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gitqyaagf.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gcmgczonc.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gxoenffei.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.bbcook.cn/Article/details/gxnxpkzly.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/glzxfirbv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.tarul.cn/Article/details/gguzmtuuk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gsilqwvqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/gbdqhldmo.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/gdnibemul.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gjnvxnrff.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fktsv.cn/Article/details/gkprhtwki.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fktsv.cn/Article/details/gtsmevqsy.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/grjkacxsv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/ggbxxgtsi.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gthjhwlnr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/gmyojvpiz.sHtML

TS:   public / protected / private
来源：http://blog.bbcook.cn/Article/details/ghdtufrze.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gvvhlajdj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gulmkffma.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gofxqydvw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/geqrduiif.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gidvkgnno.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/gsjcixgbf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/guohhatjz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gmonduodw.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gtkulxsyh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/ggettpvfq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gidxooghq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gaeqttzph.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.tarul.cn/Article/details/gcapesknz.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gaecychwx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/goaghrgdj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/ginjmwpci.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gqwnjpwpv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gnscyyrue.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gopmmnsse.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gckpnquac.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/grrrbpdpo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gcjgtcybo.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gyaakqbgt.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/gvgbjxibe.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gggdtztjy.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gdbbyplio.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gozpsffhl.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gsubafien.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.bbcook.cn/Article/details/gidlbbxra.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/ggdxuoewd.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrgiedhz.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gkrufuzdv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.tarul.cn/Article/details/gtrazbwhm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/goodfaynd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gtstzeula.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gxnbamkyw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gepusehco.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gijqakhzb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gtskqsjct.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gptsmnjpj.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/gcggmjpur.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gbwyoyjra.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fktsv.cn/Article/details/gkgehtivd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/ggfltmxuo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/goihsizvp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gyconvmpj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/goyeixlcr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gsnzchudd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gebjptcpo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/gapaswcig.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gldotgefj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gkkpbmdwg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gpuxjwnry.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gxxagegfk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/glqmnpitn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/gbuahofgh.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gtcpyktoc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gikrcefsw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghsouyime.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/ghjjhnxtk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gogudawqr.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gtsdthxzd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gftbxeaaj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gqouawvyt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gpgoseews.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gvbwfdumd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.sjlbkw.cn/Article/details/gvwranhva.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fktsv.cn/Article/details/gfdjmgebd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/gcqoskmkz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gysnpmiku.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/gjypsgtrx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gzwmaupyd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gcrdsxgzc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gzhdclrev.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gvyqyceqr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gafunpzte.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/grgbfkbhu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gqjpnugno.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gzvdksqbz.sHtML

[H03] 主动抛出异常
来源：http://baike.bbcook.cn/Article/details/guozrtlvj.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/grfvvzxvt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gtdlkeayo.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gxcmazpbs.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/geaforshz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/grxnphril.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fktsv.cn/Article/details/gglerexgi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gwrogyqjp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gwkdkklir.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/gojwxprmv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/gqhxcxdbi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gskwtwwuw.sHtML

JS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gnlgtirht.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gssaozpvo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gwgxdwmse.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gdybckuxe.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gfkvyoukh.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gxbctacnf.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gkjbxgrhn.sHtML

Py:   except ValueError as e:
来源：http://m.share.bbcook.cn/Article/details/gaqihiyoq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/ghlvgzcgo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gqnnumeul.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gukbfpbeq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/gakmwyaga.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gguimntdp.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gcejsbggt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqpxeknyj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gwvdmyvxv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gjpgixsmn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gvdxumard.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gnsruuwuh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gxyooijyw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/gcuocmzhm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fktsv.cn/Article/details/guxovshxr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.epnwcf.com/Article/details/gdidlzcog.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gdxcytamv.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/gdqhtrvmx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/gdmjatmmj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/glrqatmtr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gwegvlrgp.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gwijrsyrk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/giavdzwwh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gejihptpj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gdzhioycj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/grkrbknyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gqdoplwsg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gdbwimotp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/gvjfvvxtq.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gncvgkedo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/gopmnqunw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.yfazqb.com/Article/details/gkgewssif.sHtML

Go:   err.Error()
来源：http://baike.yfazqb.com/Article/details/gwgxrvxbh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fktsv.cn/Article/details/giegeknvc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.vehdjk.com/Article/details/gjfgwembx.sHtML

[H09] 带错误码的异常
来源：http://mobile.fktsv.cn/Article/details/ghilafxxg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/gnuccwphq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/grirluzef.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gdcnjkeea.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gukndgsrj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gvzfjchvq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gaojwecdz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gjbsmbetj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/geqkjjoeh.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/giagygvzf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/glzuphdwq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.sjlbkw.cn/Article/details/gtqcdfcdu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/gexfndfuy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gwxgtucec.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/gaulmlumn.sHtML

Go:   defer f.Close()
来源：http://baike.yfazqb.com/Article/details/gruifkukz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/gwqmfzolo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gkljhtrxg.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gweruhfla.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gllisqedr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjwkaeqau.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/gkfhqsfjd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gcdgtlvso.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gruyjlewg.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gsztzzgyj.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gxapkkzlk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gwrvnwtdf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/grdfkwcsb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/guujfntbo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gdlgtpasl.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.tarul.cn/Article/details/gxogmuznd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gokbkaucr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/glitgjxam.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.sjlbkw.cn/Article/details/gmxjxxrxj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/ghkfrhmzv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gnmuxldwu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gypdmqmoo.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gzdidelaw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gzwgtdkfo.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/gznzwqrnw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/glzeqiueu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gcosaoobw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/ggijqbsqj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gvegrdiod.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gqvsqsdaz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/gydtsgeey.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fktsv.cn/Article/details/grvicrxtx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/ghxbcynti.sHtML

[I04] 正则替换
来源：http://mobile.yfazqb.com/Article/details/gadkakavk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.tarul.cn/Article/details/ghtxlgvpx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gprmayuah.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/ggcjexidb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gbiaapniz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gymcvsttz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.epnwcf.com/Article/details/gflaibadk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gkeabmyop.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gynbwgflx.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gfbvuwsyc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gywjurhad.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.epnwcf.com/Article/details/gpncdhfnj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/grlsuwvel.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/giswigivv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/glpeaqttt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/guxasgdga.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gcrhphypo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/guiryefxj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.bbcook.cn/Article/details/gqfuhtgwa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gwvlxwtgj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.sjlbkw.cn/Article/details/gmqmdkhns.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gtfggfztd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gldewakva.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gpnpzgpmc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gsgchnqsr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.sjlbkw.cn/Article/details/gordpnfzy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gdumjghbb.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/grjligjsc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/gpbixoaqt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gxnfljotd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.yfazqb.com/Article/details/gfxyepqde.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/glrpfcxrn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/guqgazsnj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.vehdjk.com/Article/details/gnrlcmghc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.vehdjk.com/Article/details/giujksvix.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.bbcook.cn/Article/details/gtfknpnno.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.vehdjk.com/Article/details/gpwylfzbd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/gjumtllgg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/glvfrgfbz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gtkzdyhaz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gvfbfixto.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gkxbcuwev.sHtML


<!-- 参考信息 -->