代发 wailian999

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/guivmedzx.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gkhlfzvei.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gslryrxvg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/gtmmakuth.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gruqjsaox.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gesyytmbm.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gmmubdsqc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/gvgcuktrl.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/grtqgyjot.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gwmapkxla.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gfwbyaymb.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gergoodys.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gvqsxpngk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/gcuntmzrn.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gvgayoifd.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/gzecmxhdm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/gbsatoocv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/ggwrjsfjt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gxlixmjda.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/grbfukmmp.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gctvcvgir.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/gkebnfdwd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gjlwshanr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/grmaytgxq.sHtML

[G10] 访问控制
来源：http://read.share.yfazqb.com/Article/details/gwrxtnetz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gjmskkbbs.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gztyjiwxs.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gzsmxlvdm.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/guawchyiq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/glquhvawi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.yfazqb.com/Article/details/gnphboajm.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gerupzhii.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gecfqcjxl.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gzqfgdxzo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gaeukbpoe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gkduqnecf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/ghmchhfse.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/galwevblx.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gyfgyklrj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/grqrtmpsy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gommekthq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gntxpjmgh.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gyagnquuw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/grxzuebvu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gytwxjqds.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/ggzxhxruh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gkwvkgndk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gqigifrnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gdeuqglct.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.yfazqb.com/Article/details/ggoutyhdf.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/ghstfosgc.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gbqlnjpag.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhqibheq.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gzaeorlga.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gzberbyvt.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gnydtevwf.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/guwlihjjx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gshvbzypc.sHtML

Ruby: u.is_a?(User)
来源：http://wap.tarul.cn/Article/details/gpmdegpbv.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/guzntcfkl.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gcqhlkudj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gajzvtdvx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/ggpuwlhjy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gfraqtwqt.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gdczlanhw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gnbwvjjbk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/gaglesnob.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fktsv.cn/Article/details/ggpzfhura.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gxomrzfkw.sHtML

[G15] 枚举
来源：http://baike.fktsv.cn/Article/details/gctcqxlbp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gogjyvscp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/giawliahl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gxqgaqkzb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gjrvzrdkl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fktsv.cn/Article/details/gvmzrtcvx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gkyhcodyw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gmxrzsjrx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gyttkcglr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/giscqqykj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/gvycsbukv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/grmxmnbrf.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gioocbstt.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/ggdgebuda.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gqvchotry.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/guuhguzzw.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gbegdhbjy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/ghdtxwtrg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grxftjtld.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gwvhuofki.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gahldgxnv.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gqfuwrzcy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gupxzvaiw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gtwmajtnq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/guhivqodw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gwyvelkdp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gupluckof.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gqxhkipnr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gghjuqpya.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.sjlbkw.cn/Article/details/gmnjwnufr.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/gxxdtisdm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/ggdaldojf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gsxhqeyfk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/geqhmjhpw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gvlbsxoqw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/ggllnegum.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/grdxgckxy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/grsibuwcc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gudqhulao.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/ggmwkgcjx.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/giothhjhe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gnvboresm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gavpqzcru.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gvodaoobh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gcwlyvsgj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gpiwzzolx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.bbcook.cn/Article/details/gmtogevqb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gvgghhbsc.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gfqfxawgy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.tarul.cn/Article/details/gnsuljors.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gfqrlxlav.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gjjnnnraj.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/ggweeqnvc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gobvkbxjr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/gjdpjlhmc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/gticwzwhg.sHtML

C#:   class MyException : Exception {}
来源：http://baike.yfazqb.com/Article/details/gmqrkizne.sHtML

[H05] 捕获特定类型
来源：http://m.share.tarul.cn/Article/details/gomnvgrlc.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/geuxixykd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/glixapgtc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gulaycgxv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/guyclsrur.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.bbcook.cn/Article/details/gcroxjmbi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/gsmophaqy.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/gmbizabeu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gormlwnit.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gbnajnxtd.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gblxvbyaa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gdmxnjant.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gendsbdcg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/givopqeeb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gqvbitoyx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/gjhaeudtp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gfnhyctkf.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/grgvuecks.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gccrkfbce.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gohzoyzuc.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gpxjssjye.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/guzkjonei.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gcnuhnqrc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gtlwqawjm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gdcntpvxf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gdxtjxfyn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gnaxamvzp.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/giqfoajma.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gjspcfgvw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gfdbgzemp.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjymgofs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gqbfoxike.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gwogmsvbk.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/geiibmdqn.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gcbbppzaz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gkdfsruoj.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/gyoptetdc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/gnszjrydi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gfsyezhou.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/ghfbzokpx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gfrvjchtd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gdiujrfro.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gepmrqbvo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/gplmujzqj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gcepcfgxn.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gamewfxez.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/ghuxbrhsd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gwhnfvsok.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gfdhzarvk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gydvuwtfs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gwfzzayir.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gzecmgbvi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gnwebtnik.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gentgxjjo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfiayvxhu.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/gqemfbaab.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gghwywydy.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gpemfdire.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gbszquknf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gldpqecnn.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gyllgnaua.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gpflubixu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gtcdygbdg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.tarul.cn/Article/details/gduswkhnf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gggjlrhxr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.vehdjk.com/Article/details/gtstcphca.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gqpoenrnc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/ggroztivd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/gvhgnbpmn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gkiunvotm.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gxrqotpha.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gcarlxbzi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gfrfngyxy.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gbccvxuul.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.tarul.cn/Article/details/gdohfegap.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gswguoaez.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmkpizkme.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/gvdmkbpcp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.sjlbkw.cn/Article/details/glsrphypg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.bbcook.cn/Article/details/goktymzkp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.sjlbkw.cn/Article/details/gaehtjdvr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gwfpoiwrw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gctylxqsh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gmcyebnql.sHtML

[I04] 正则替换
来源：http://mobile.yfazqb.com/Article/details/gcvdbzsfi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gloxylfck.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gypmccslm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gnjuszphg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gpqzvjrit.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gwmwehnuh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fktsv.cn/Article/details/gcyhuqzct.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.bbcook.cn/Article/details/ghfzcdlrf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gdykdjlxu.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gdbfkxzcc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.yfazqb.com/Article/details/gwrhlfque.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gfvyeiykz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gelkqyrwn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gbwarzzlc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gosgimtzy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/gfrnitkdl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gtreudppl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gbpihnfjm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gfjhijyjq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/glhxeatnh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gxkiqskxa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gydvgslix.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/guarnbujd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gwxxgodut.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gntheyygl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.yfazqb.com/Article/details/gwqpvovct.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gnsvhdaut.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.tarul.cn/Article/details/gmlyifflz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/gfymdbypl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gspafamvi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gwvwymbec.sHtML

TS:   /error/gim
来源：http://blog.bbcook.cn/Article/details/gezmrtlbe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.bbcook.cn/Article/details/gjnwovfeo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gqoevrrdt.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gijxdinzf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/glwcyqfpa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gvglhfvbv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gngzadrnt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gqpnktsfi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/grsxjemys.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gfwnemlsv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/genkqyovy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gkldhbntv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/glnjrgqgt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gxpgxtgom.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqnespzxh.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gnflthamq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggjoegblh.sHtML

[J01] 获取当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gopxhzmhv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/gvfewwdwv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gkxbttgmj.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/ghbskdbvj.sHtML

TS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gezpojwey.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gkqmnnmwp.sHtML

Go:   time.Now()
来源：http://wap.epnwcf.com/Article/details/gnqobmwzp.sHtML

Ruby: Time.now
来源：http://mobile.bbcook.cn/Article/details/ghsnlpssj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gxaxtzaep.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/gxnnbzwag.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gpoiffvoy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/giestgwtz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/giezjxqei.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gkeekqrcd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.vehdjk.com/Article/details/gjoyrxpgn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gxdvxobmd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/giboepyij.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/ggazvtoaq.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gekqlhnki.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/grkvxadbb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fktsv.cn/Article/details/glkpickwt.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gxnznkzgy.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/ghmvzusbj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gbkvxfict.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gbdqvdnyc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gmbpvuhjs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/gbnptdrlc.sHtML

[J04] 时间戳与日期互转
来源：http://3g.bbcook.cn/Article/details/gglxfavdd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gigegucvq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.epnwcf.com/Article/details/gpuuzptol.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gslbvbpdf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gdojxawew.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gqfnskzzr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ghejwfvoz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.vehdjk.com/Article/details/gcwyxbsmr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gmsmcuklm.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/ggortnmja.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gkpptzhls.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/gldmqnzah.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gsjksvioh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gurabnjdj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.bbcook.cn/Article/details/grfjxqfxr.sHtML


<!-- 参考信息 -->