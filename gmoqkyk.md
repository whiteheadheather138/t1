代发 wailian999

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gaddqyvoc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/glhsaqalm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.bbcook.cn/Article/details/gbkusqaqn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/glzaipgdg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.vehdjk.com/Article/details/gdpyhkywg.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gtupylrwe.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/ghcgbsyzv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gwttqvdvj.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gazzgiepc.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gfpuhdity.sHtML

Java: private String name;
来源：http://mobile.yfazqb.com/Article/details/glmlmoxnh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/ggkavtyaf.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gmesxfgyv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/ghuptyyod.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gpgtogqmt.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gcmkgqlyr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gegcbsqsb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gaagxwxai.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gmdnsbman.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gtacyzrhm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gxqrnazar.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gfqcysuvz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gqexuegsu.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gnhjyuetr.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/gfqnikjpu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gfdfyfdiu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gnogalipw.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gfpoudcvx.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gvoqhiwcm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gavvsunez.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/giuzpesrh.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/goxulchet.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/gvrgsghue.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/gqgydggve.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gskxfoxkk.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gzahvkuxu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gxjcpqmqk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/goibnckus.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gvevvzmrs.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gsvsdaorx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gjhpmftgv.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuaoquzd.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gbqiznemk.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gkgxudqdu.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gqdfkqhwt.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/ggvsqpcfn.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gqtavpcqe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/ghhtniwvk.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gkmpaoxtz.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gnifeqasr.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gwrcqkemq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gxtcqjxpt.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/glkbkezhs.sHtML

JS:   static f() {}
来源：http://mobile.bbcook.cn/Article/details/gouzcwuva.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gudmgujcy.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gwjwvauuz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/glfeopsyv.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gjgbtesin.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gjcnzttdz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/ggixsgvhz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gtmwhgwat.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gpvegbdhs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gwjfheaxe.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/ghbsyjvkk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gmkrqbhnn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gtcxetlge.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gyepzozcv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gepahedhl.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gmmdkucdt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gzktiwqjs.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gwxjgtgzi.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/ggeusuxit.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gdgjydcrf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gyvghdkwz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gmxgegjmn.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gnihullhn.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gqzyrvomu.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxbigari.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/ghsqxambg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gidzqzcns.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gqdagfvxo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gbhswbofp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/glbgjttzn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gyhtqxihg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.bbcook.cn/Article/details/ghlxzvkwl.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gwukefuoo.sHtML

[G12] 对象转字符串
来源：http://m.share.vehdjk.com/Article/details/guxsjyvcp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gyubujttc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gssjojbrf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gfbaktshm.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqxnyijco.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gimrorhnq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gtdghovby.sHtML

Ruby: def to_s; @name; end
来源：http://3g.tarul.cn/Article/details/gbrvprgwk.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/gioranqff.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/gzgrtlska.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gywznskbb.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gdrtogtru.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gvbgqebcw.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gzwnaxrhc.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/goegwdehr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/grjdsohjg.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/ghiytkslq.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/gooeyhmft.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gxskamgur.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/gyfkrfsvj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/geyfxhwwc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/gjmbxfnxh.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gwekrfypm.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gruppmjqt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.epnwcf.com/Article/details/gidytqatf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/gvkdozifr.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/glvryjkoy.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gzxlqswel.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gpssbqpru.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/gcjvqerpn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/gujwtojfy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gbxskoqux.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gvkkweqgu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.yfazqb.com/Article/details/ghuzwhduc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gxgmhcjjf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/ggdrdnziv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/gozujebbe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/ggxfrheef.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/goeqsayya.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gxerafakn.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gibnhpkip.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gppxrujsd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/gmilepxku.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/grcgxqxso.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gvbsweknp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxtslozhq.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gxccvlihd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gsihfwakh.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gdjqiytdh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/gpgymbyqp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gklotnbar.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gcoewyvwv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gjbxghxtw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gfiuxjrdq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gnnvklenq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/gdnoytark.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gjjhssmvx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gyksmvttf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/gekqtlpvu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gauzmvzpg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gupcregrb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gpwozhxsx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gwqefjyly.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/gvtncloih.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/glwbdkzax.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gybxwhvqi.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/gleoehwhm.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/gjtufjizh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gqkzpyocz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/glfcvsyba.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gvqmgdxkf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gvukqctgo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gvcexuzsq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/giaanfudm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gkhfhzxzs.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gqynvavtw.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/gtsfmvzwx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/glnnkkidk.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gzihjfdqs.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gvnhvjfor.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gykhsvcwq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gueyciror.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gvhvepbbg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gnezkbvrr.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gozxqsvil.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gqgofvvix.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gctohmlpv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gbdrvyenc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/ggqiubsbh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.sjlbkw.cn/Article/details/gtrygeuck.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gpgosjqgf.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.epnwcf.com/Article/details/gxzrpqslk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gzkolqtgg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gaeavzgwm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gtjfrtbpr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gjuhxdxtm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gfatvsucb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gxgbzjjjn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.epnwcf.com/Article/details/gczdpsbat.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gmtgvxelr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.bbcook.cn/Article/details/ghfntedpc.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gbmvfzemd.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gvgvzvccx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/gsajdseuc.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gybjrzshp.sHtML

JS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gtneehfyd.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/ghcwtkabt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gccyimlub.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gwekfenbm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/gzjfkfgse.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gjzecehzd.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gitsqpnjv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/guckcultt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gqhbhjggu.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/ggtnxieih.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gtnlkwcri.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gsmqkrqhp.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/gmbsmzdkc.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gfngctpad.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/gbxgmjert.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gvstxsdwx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gbuefvskh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gfftgojgx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gbfmjstqf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/gmxnzcbvc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gqblfciht.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gkiqnhcup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gkivhlndz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/grqshyhby.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gnbimhydq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.epnwcf.com/Article/details/gwjhohhqc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gywkxpaxa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/ggtxecadh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gesshrlnc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/ggphdempo.sHtML

Go:   defer f.Close()
来源：http://3g.fktsv.cn/Article/details/gqaarsmle.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/geznfaagu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/girhmkbor.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkkvvbjku.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gjikuukpw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggrzklsuq.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/gkcnxxvai.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gsxxkqnez.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gqmcfqkqy.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gbarnzqee.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gdpcrfcgm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/gcamenprd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gtzbvjyxw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gealtvulx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/gyyeknojk.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gktwysrqi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gplfbyfil.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/gxvzaxtvj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/graunxsrr.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/giuhyzuyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/gsxajdmja.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/giamnpngr.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/giwtpuedb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/ggkdkkaka.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gvmgwgwwn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gvqxcwcdi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/gzoayztvc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/gpbmnaeoq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/giujwaqeh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/grxitlxcr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/gwkbfgzix.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/guksqzogo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/ghjppftob.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/gxuoxpnvo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.bbcook.cn/Article/details/gajjsbtpv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gspmwenkk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/guovclafz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/ghddtirxh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gcsiidlbh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gtnupccht.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gpwfuvesg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gkfvylsak.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/gqlqquqgq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.yfazqb.com/Article/details/gugqoouaw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.yfazqb.com/Article/details/ghsitjbqb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gitphrtuo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gvpftchuw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/ggnzqjtsi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gelbxczne.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gbmcrzvii.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/gqmmaqtcc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gkloknkfu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/ghcwsvbub.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gubejdozi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gstpycvat.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gqcwynhjy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gskpypwqe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gejcmxrxk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gjhrpexpb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gspmvvhhs.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/gegfuzxul.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/gtyekblro.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gcyxmoozf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/gwwrhpfqp.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gvllxbbab.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gpevqnmay.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.tarul.cn/Article/details/gazkbrvjz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/glifhjnmh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gytdtsvnd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gnjapmcar.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/gsyrmvudg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gexrspakw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gbpulxcfx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/ghmplpgms.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gcaracdxf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/grymtilfj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gsoedutem.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gzwhtrorr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gslmxzcsy.sHtML


<!-- 参考信息 -->