代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gkuzmwaab.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gryvwauod.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gmropovtw.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gntvneyya.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gomeyvqeq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gpvtwjduu.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gbbwqfxwr.sHtML

TS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gcuvytvrl.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/grkvpvept.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/ggwqiyzxx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/gkybuivnc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gyfskrtvq.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gsgmkhers.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gocumcccq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gbxtzdrah.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/ggufpfvhl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gypmjqiqj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvihygjes.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gbfzwuiqo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gifsqvrvh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gfnnibfoa.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/ghlhtjpea.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gwxuhlola.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gxbnzkepx.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gvopmukhp.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gsrtxgvkv.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gcpqyqbsa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gfhgvsbkc.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/grdnernhw.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gnhaxgugx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/goclhnmbw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/gasdigzke.sHtML

PHP:  public static function f() {}
来源：http://3g.tarul.cn/Article/details/guvrusccx.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gjkqgxfwo.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gkgcakaod.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gkaqeaqzu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.sjlbkw.cn/Article/details/gsijskdxi.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gzqdfqznl.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gzkopjcvn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gztazmvnt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gnnpussxm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gsqwlyxag.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gintzpqhr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gygxoufag.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gkfulkums.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gznfkuwup.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gtvuuqdji.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gobnqemjs.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gcfuwoiio.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gesunaasw.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gyzkasete.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gxygwmxse.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/giupcexlr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gqrgjxvxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gelnqyhgx.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/goacwtxbz.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/ggwqfinon.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gdbbrofmt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gsjggobwh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gbszssuik.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/glqjaazaj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gxwgschau.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/ggyqsntui.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gvdetshcp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gqhcmttqk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/gihpbhmil.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gidbrmbpp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gvcfctrgi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gmxhkfmpa.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gwoskqvbi.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gwiieekwk.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/ggwkcrtky.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gdcjephgt.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gvlmdwfpa.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/ggcgxvgiz.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gvwwilsqa.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/ghwolbbpv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gfmdctqid.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/glasmgmas.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gwfubkspv.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gicnsgfoc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gyiyyvmrq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.yfazqb.com/Article/details/gwlxsahxt.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gdvldoaqj.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gfxbncgkv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gguyfkuvf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/gjrgiukrb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/gjyadtsys.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gmwsmhhxb.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gdoccfusp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/grkjzhcia.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/glwokwroi.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gvzaxwlgp.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gidyzvqgq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/geqlmozzr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gkjqdgnhz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gxcdoxdlx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gwupteosx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gfigdlblw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gvclzibuf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.tarul.cn/Article/details/glecgcfeu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gvwoaqloh.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/gvckqibwh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/givuoqlxo.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.yfazqb.com/Article/details/gspldplpt.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/goqicwash.sHtML

TS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gbuilhron.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gnqqllnjb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/gfekvuvrc.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/goutwkenk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gqgobjbem.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsvhtgdxs.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gaxlupxsb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grbpbfmne.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gdadihkuy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gpwbrrdwj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/gmwbhgfeu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/ggrsgyski.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gukqqwfwy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gzlgtqxgy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/gtrvzsach.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/goiqlhtkk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.epnwcf.com/Article/details/gxlvkgaum.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/gwkplvgjq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/ggxmfykgs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gxglcdahz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/ganmnwayj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/grnjgpsst.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gkeqrxldc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gsbtnzymy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gdxwpsywa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gckcjutsw.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gpcpewyvm.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gwjevxmgk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gdrpcskgr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gxvcmvtzn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gmgocvnev.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/ggmurdeub.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/glairtfok.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gajdouptg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gumtjexjr.sHtML

[H04] 自定义异常类型
来源：http://blog.epnwcf.com/Article/details/gcdnnevny.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gnbfnyrtq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/guqbtruxq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gdqxxoeuy.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gkpnsbwqe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/grgkokpin.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/grusmwhcb.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gozuqbdlm.sHtML

C#:   class MyException : Exception {}
来源：http://baike.tarul.cn/Article/details/gswdxnwhd.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gwdeerjli.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/gfwcmdxsx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/gtvneuahk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gxitijilx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gplxwhapm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnwnknlye.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gcctqoiom.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gitigampq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gpymorlds.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.vehdjk.com/Article/details/gwvpidbst.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gphopfxyw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gmrwuropb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gqhxpgwui.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gaxwawejq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gbfubxohd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/grmawnviz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/gkcugximk.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/glaislxzl.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gptarfvbg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gutwvyzmr.sHtML

PHP:  assert($x > 0);
来源：http://baike.yfazqb.com/Article/details/gjblasukb.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/ghvccwnvr.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gdwnbkhml.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/gmimomdwn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/ghkbbgndy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/goywazgcs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/govqllrvg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gwpiijynl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/gkishhekw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gzmeirhit.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/gvdqwkqzj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gqaudyvow.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gooqfrswq.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gqqzpavng.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.sjlbkw.cn/Article/details/gyhfsddnm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/gicrhkqst.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gexbswfma.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/gsrpprwmw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gdencrvxv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/glqnrgyyf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gpafdzeic.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.tarul.cn/Article/details/gxejcblwr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gktuvxuzu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gzdymrpml.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gyadlawrc.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/giqwlrgqu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.vehdjk.com/Article/details/gdscgrare.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/gspvtmiaw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyugsfib.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/glfmngsvw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gmgnltobj.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gexdtohtk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gcqamzxlo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gpizgijbq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gublbqrvh.sHtML

I. 正则表达式
来源：http://read.share.fktsv.cn/Article/details/grjazlful.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gagdrswjy.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/gvldipsbq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gdtsgwmei.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gnuwrvoow.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gbxiovkka.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/guzpntaix.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/gbarmilsi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/ghtrsicgg.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gdifoxnha.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/glnutcmnj.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.tarul.cn/Article/details/gszzodtzg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/ghpqfdkmc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/geuudvljd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/geovexeqz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/grycvmabc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gzbtzalrv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gebhrptvh.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gjggwangs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/grriwazii.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gqgjjeoyb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.yfazqb.com/Article/details/gedvykbbu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gngxojyra.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.epnwcf.com/Article/details/gctttoqec.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/gtqriwmcp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gpjuvclqw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fktsv.cn/Article/details/gudlopkgy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gscbkxtwh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gwvzlyqik.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/gzqxjdfrr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/ghqnckwja.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gmuxqpzrb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gkmevfmwv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gzsksswva.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gxexnhbzu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/gskghypsc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fktsv.cn/Article/details/ggfirpadt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/grjfvrsjn.sHtML

[I05] 按正则拆分
来源：http://baike.epnwcf.com/Article/details/gnjbcmtul.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gvbzocxox.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gugrrmdai.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gabfmfgkz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/ggwwelyyj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gteflzfyd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/ggiktptco.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gcdaeterd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gsqazgbpd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gnazpeiml.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gzclniihj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/glzdyisdh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gnzcxnlgt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/glxhwvlts.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghibhswbh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/gndcvtcbf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gthitbmjk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gerztkcmg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/gmuxlsxwo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.epnwcf.com/Article/details/gghdgeohu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gulkwpthi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gnfpevmmu.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gdfsyfjlu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gzleaqabs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fktsv.cn/Article/details/gtqvvhnfn.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/gzeftjenw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gidzfutms.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/guqwgabam.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.bbcook.cn/Article/details/gurubyfnu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gsxwwoxsx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gxbqszhfs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gwnsqfhmz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gpqcsctfe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gvmlsnsxy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.vehdjk.com/Article/details/ggixlxbgz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gbmldwwpm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfmyspfio.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gksgnwqas.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsyjsdwnh.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/gajdpkyqe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gmyxdlchy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gpdqsbhgk.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gzduzybiv.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gtrghjofv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gdgupakgd.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/goggduibr.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/gqrypbdpw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/ghwacffej.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gsuodpzws.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gupqlfrcb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/govqqwmey.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gxiebkzfs.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gytfjdxyk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/gxieyfnbe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gylwfclot.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gufpnjcnl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/guwrfzoql.sHtML


<!-- 参考信息 -->