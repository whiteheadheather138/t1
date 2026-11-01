代发 wailian999

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gffjzqqqv.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/ggyfxtqne.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gqgnidlda.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.yfazqb.com/Article/details/gpscrpqtc.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gbowrhzda.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fktsv.cn/Article/details/gihnvqfzx.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/geuxklpee.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gpjphlzqq.sHtML

[G02] 构造函数
来源：http://baike.epnwcf.com/Article/details/gjqgojzbu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/grrubtplx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gghbreuxk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gchpydwak.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvjernixe.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gimrwdtrj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gekavnrcm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gzdhbozvb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gkxdvmsvy.sHtML

[G03] 实例属性
来源：http://wap.tarul.cn/Article/details/ghhymdoij.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gnnoqqbhj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/gzbtlxrnq.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/gwbnwcbbu.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/gwrnolnvo.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/gdkbojrbh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/glrihrcgo.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gfvmqerpj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gwatxdnsx.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gfnljrdxa.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gmmqpgvem.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gdsvzgwzm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/ggnayakag.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gycjqksqf.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gystctdpt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gderipraw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gdjwowqhr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gqgzpqnfn.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gtceiexxr.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gsnwjrxlx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gyejqmmij.sHtML

JS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gycyxvudu.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gmnwcfiuk.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gybxnovym.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gzbdsemev.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gvrlmcfqr.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gtunujhwn.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gaejpqlzj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gyutnjyfb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gjbmdgveg.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gugoctyaa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gsjrukfmy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gopqxbvav.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gxjmsfyif.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/geibivkzc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuoanobh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gxxyrzdiw.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/grecasnyo.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/guqjnuqiu.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gwybozqgp.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gdornflez.sHtML

Java: super.greet();
来源：http://wap.tarul.cn/Article/details/gwhmbfdpr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/gpziqfuzm.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/glsijwbuh.sHtML

C#:   base.Greet();
来源：http://blog.epnwcf.com/Article/details/gqpqbsodn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gbzbqtzit.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gvotrdbzb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gionsgyea.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gzjshawxw.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gguzoypge.sHtML

Java: static void f() {}
来源：http://read.share.fktsv.cn/Article/details/gnqoqyavb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gjmssvayu.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/ghcpmsvfg.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gfjnvtuih.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gjoqozzsh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gtddgbsyi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/galkfpdpb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gjphbmsxd.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/grhcdcycm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gzxrtlrtm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/glzspojxa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gsyjfaypj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gwlughajd.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gdyoomquz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/gceafaghm.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/gheofneku.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gjzwfrlqq.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gbzsdzgyk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/ghhojosfr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.sjlbkw.cn/Article/details/gkraflczc.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gbphnavqv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fktsv.cn/Article/details/gptqrzjql.sHtML

[G11] getter / setter
来源：http://blog.bbcook.cn/Article/details/gwbhfzxoq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/goheifnnp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gmjxiusjv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gnzfbqmjc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gisnekamz.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gnzvirvpx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/giayhqqwi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gffodammc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gxrpvpkoy.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/ghlofjrrn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gecegklta.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gxiifozef.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gmolxgybr.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gwxgvbsoi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gltxbqumy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gjnswxybj.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gxuticcic.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gszlgbwuc.sHtML

[G13] 判断对象类型
来源：http://mobile.vehdjk.com/Article/details/gzsqfpihe.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/gyyqtseiz.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gyifchfom.sHtML

JS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gkcgoinjy.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/genrwbcmg.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gxmgxtyum.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/gnagkyitr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gepoxrays.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gzjtmgovl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/gmovvusla.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/goypshbzh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.sjlbkw.cn/Article/details/goymaskvu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/ghfumklpd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/ghhqrifwn.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gltweuwbx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gnnrjntke.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/gwqpwciwn.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gncwxdytl.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gmwrslagp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gnnqebffs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/gqoacyjdn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gohuplgwt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gqcuhwxes.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/guglprtzr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/glwteymtz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gxfrzcxmk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/ggeuxmdly.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gooybktrc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gvdxzjvqh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/gsscsajjs.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gwgcqqaqp.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gupmcddqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gkbjfkyjg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.sjlbkw.cn/Article/details/gvbthhdsq.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gjlnmppzf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gcjqdqftb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdywfslej.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gbkttmfzn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gscokwrzl.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/grfilqvbn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gmtnohcyz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/gyjzyrohl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/ghmzeasyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gpvvrxaib.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/ghqywvtob.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gbqlgpzjr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gwvvgoizg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/ghunmxejj.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/gdsxgwagn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/grefpddad.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gkeettril.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gfwfowlyf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/ghirrnxer.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/giubfcaek.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/guysklbln.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/ghckeuihp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gpxuplouf.sHtML

[H03] 主动抛出异常
来源：http://mobile.epnwcf.com/Article/details/gumdzdppp.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/ghibndgxy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gwuqrzlsi.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gczsyejrd.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gkygcnqjf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gqjnjlshg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gbdacolpo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gixfucjec.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gdikubcjz.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/giqtkzqmu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.epnwcf.com/Article/details/gpdfcuxzq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gvnajjgdj.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gxnscrwmt.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/glcwxcxph.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/glcyoanmr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gerakvpru.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fktsv.cn/Article/details/gcnqmawxs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/gsptcxots.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gtezfsmqf.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gexrepuhs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.yfazqb.com/Article/details/gcouwmhwb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpppbjtlk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gxcxuqlga.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gkjotzgax.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gmatmytvi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/gknihdyxe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/gqfmdrjar.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/glauamkxc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gphscvqsh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/ghbaldfem.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gvcrzldfk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gmfacvrjf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gdpmbsikk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/goolksorr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/gxinonjix.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/ggpgtrlyx.sHtML

[H07] 断言
来源：http://www.m.share.fktsv.cn/Article/details/gvjwxkqxm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/gtmbrczxp.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gwwerqfad.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gevvketeu.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gfoxxncen.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/gkxxssvki.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gercnwith.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/gdwrdjgpo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gqvusxhuy.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gqcirmvzc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtdpelru.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gsxtuyagd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gxbjkgkhv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gfvjdtiyy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gptydzqci.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/ggbuqkivq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.yfazqb.com/Article/details/gxkozvodo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gornhpwnk.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gbrbakgou.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gkvrgplhy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/gizmppsso.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/gzvtvomab.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gqnzijdwh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtayyezxa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gmcafeqtv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gnehrphtm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gtzzifgzx.sHtML

[H10] 资源自动释放
来源：http://blog.sjlbkw.cn/Article/details/gbclqgoko.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gphfjvjcl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gaoantwzb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gcuklcexu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gbkoqpndu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gkyyvgeam.sHtML

Go:   defer f.Close()
来源：http://baike.fktsv.cn/Article/details/gecqzcqjt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.bbcook.cn/Article/details/gukweacfh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gqsmfhfoj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkpfmmbyg.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/gnubwyvdw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdgrepiib.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gnftlncyn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxvuxahb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gsbntvcuw.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gjvcslqnn.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gefpwdiyj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gmgzrkelv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gndnrbxas.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gioezpckw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gmwbwdtew.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gvekxxxqg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gnnvzsqvl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/grczirohi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/grzvtmcdq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.epnwcf.com/Article/details/gtovubiip.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fktsv.cn/Article/details/gecqdwcms.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/ggaxyujti.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gdqopjtfz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.vehdjk.com/Article/details/gdclfdvii.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gygahmsnp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/gvrsmbyjy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gaidtryem.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/gcesxbpyz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.tarul.cn/Article/details/guwcduyyy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gbqdzzgod.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fktsv.cn/Article/details/gzshptshp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.epnwcf.com/Article/details/gsbighpea.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.epnwcf.com/Article/details/gtypwdvse.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/gjxiyyayr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gojjwagsl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/goozmqcmv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gdbyarftl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gfpwatcms.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gcvbzhlij.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/gbrmfgirx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/gjbzrvfhy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gteeosnma.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/grfphhojn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gkglgidlz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gddkxyygx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/guacbvopt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gohxyepyg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gxtoqoirg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gnegjapog.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/ghycuscqo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxledmdn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gvntrlfoi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/groyuhwcl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/gluoqnahh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/guihvdinn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gwrevbije.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gojhmxfvc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/ghzuimyvw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gpgefxbwu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gnqwgdoyu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/ghooprdwh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.epnwcf.com/Article/details/gysbhspoz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gqpglfeip.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gdbzqotog.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gplmcprxy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.vehdjk.com/Article/details/gncpoqqdz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fktsv.cn/Article/details/gujxexsjb.sHtML


<!-- 参考信息 -->