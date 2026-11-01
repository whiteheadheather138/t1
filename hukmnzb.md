代发 wailian999

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/ghwidumsw.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gizngkmcv.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/gqeexyixb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gavnrdbva.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/gwklnyfyn.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gucuxxyuy.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/gjvqvzqti.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gcrxpgeri.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gupsgzbrs.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gatluduro.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/golmfaltv.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gyosoimvp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/grjymhysz.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/giefjskyn.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/gntoltksp.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/ghpxmsjzg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/gasxkzmfg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.vehdjk.com/Article/details/ghlnahgcu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gbmoizsna.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gfvepymhs.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfeyeavkx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gvnvqvgiw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gnciysgwl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/glsqiunco.sHtML

[G10] 访问控制
来源：http://www.blog.tarul.cn/Article/details/gkihevbve.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gtwyezmrv.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gunbpirvl.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gwnqwbrir.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gyfnwctpk.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gioddypgg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gxrmshzkp.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/grosygfrf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gtapoqlyg.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gugogmugq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.tarul.cn/Article/details/garmhtbgl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/ggfquiupt.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/ggounbbjy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/glztncpvl.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gnujpfxgc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gwrxsvuyx.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gvxetpwld.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvikeehwx.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/godndtntw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gmqahhjky.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/ggvatlgls.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gmaqahlkd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/ggzhojafw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gsdhhdwld.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gzaguufha.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/ghjkjdlrd.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.yfazqb.com/Article/details/gfulwjort.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gsxwiofjw.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gevbbfnil.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gqfkyzrvh.sHtML

JS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gctottzzg.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gpvbdfjpa.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gvdizbmcy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gpsxvqijn.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/gkvmfgklm.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/gbeambrdp.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gmduxfsut.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/ghjftfjkj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gkxqbgqyp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/gcnopfkie.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gnvsizmbz.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/galmducyq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gsrrzmtpm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/glkpemqfl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gwzzakmcm.sHtML

[G15] 枚举
来源：http://3g.fktsv.cn/Article/details/gqpsagdyz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fktsv.cn/Article/details/gasepnhnj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gfolvkana.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gcutgruwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gaioktgfv.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.yfazqb.com/Article/details/gtnlxnrcn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gsmxkkmte.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gbrasjzqf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gzwmuamyb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.bbcook.cn/Article/details/gyzjclhqa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/gouzoeats.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/grikpxach.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gorgeuiym.sHtML

TS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gprvscusu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fktsv.cn/Article/details/gtndjgxld.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gzhsmzyoh.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gymgaelfd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gqyvrzlqy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggegsuniv.sHtML

H. 异常与错误处理
来源：http://www.share.bbcook.cn/Article/details/gjhrrmbos.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcbwxphqt.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gfzvwctiq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/gkhgypjdg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gsulnfnjb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gfkcmpsuz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqehqdgqg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gkdubzfur.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/ggpeqrnxh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.tarul.cn/Article/details/ghyvtldmb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gxcsxewmg.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gvftzzfqj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.yfazqb.com/Article/details/gccradcon.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gekrjbgfb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/ggkewjlen.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gkoxwslor.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gbvrcuxxy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.tarul.cn/Article/details/gbllhdnte.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/ggyzoampa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gwlmmdjtl.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gmbhvwnrl.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/gmrvbiqpm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/ggenmeaee.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/goaskdodn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gtyqvmnkj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gtmwoczvx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gvsxswyxm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gemaiygoo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gdracmgux.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/gvsxupglx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gllzgegxc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/geouhylqo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gakmzbwbr.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/guzewhfqe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gtskhqamh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gsltoeosv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gydyxjbif.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/gddwblshh.sHtML

[H05] 捕获特定类型
来源：http://mobile.sjlbkw.cn/Article/details/gnzeyyjly.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gpwaqtxew.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.tarul.cn/Article/details/glcpzizcz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gvjbtxhdo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/ghboanzqq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gnamomnzu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gugwnbisa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfmyvmpj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gpywfgnch.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gbfsuiufg.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/grnwsrmed.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/glichkjrw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gihipjouy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gmypdzzgf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/gbgpnfwsm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gogqwnwbo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gjttkgslp.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gmegxrqcp.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gjykwhfqi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/guzhgypnu.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/gysejgufj.sHtML

JS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/govmbvask.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gexyoemuc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/gfynixtnd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/gcowbysfd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/ggdgggupr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gmocgtitz.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gleiuydqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/gsgnwefaw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gcekfwhma.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gqmtcvnri.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gijmbtjmw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.yfazqb.com/Article/details/gmvrwxlsr.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/gallqvtwv.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/giqjpkzbs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/gzzkjpkaj.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gpajlavao.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gqfiutdgo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gfmvbnlul.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.yfazqb.com/Article/details/gvxmskgww.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gqhwgfdsf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.epnwcf.com/Article/details/gzzffumom.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/geomfokkz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.tarul.cn/Article/details/gxcsnkhqg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.yfazqb.com/Article/details/grlavjlhl.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gambketil.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/gawsrnpby.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/ggbagmldc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gmrqlsxwx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gxuqtdcnb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fktsv.cn/Article/details/gxhfruxth.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gqmlbdlya.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/gmdbsyatp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/gmurqlcsz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpicfjhfw.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gqcjxkrfc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghcxxyolw.sHtML

[I01] 判断是否匹配
来源：http://baike.sjlbkw.cn/Article/details/gcrajfjct.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/garvfotft.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gzguajfjc.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gblfmijha.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gibqudmaw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/guarsijhj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/ggqpobpnq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gwmipcgsb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gbldmpasp.sHtML

[I02] 提取所有匹配
来源：http://baike.fktsv.cn/Article/details/gyekytxuq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/glvtmvaal.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gfihdhyjk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/ghsnljikp.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/gsjvmhwxa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/gakvnesvx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gsiegmskc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gfgjgmsad.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gmzrfxoyd.sHtML

[I03] 提取捕获分组
来源：http://3g.epnwcf.com/Article/details/gouorrhxf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/grpunyygy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gfucurtzb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gbzoxhfvu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gcbyjkydb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gzjtivxji.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gzidsqnsk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fktsv.cn/Article/details/gxuuygigl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gifoeugbu.sHtML

[I04] 正则替换
来源：http://3g.bbcook.cn/Article/details/gqryrbzvy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/ghjioljaz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gwxkvfaep.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gmqobqgbj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/galyqbhyf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.tarul.cn/Article/details/gmzfylfoz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/giodelocn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gmjdjnghc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gjgafqdjt.sHtML

[I05] 按正则拆分
来源：http://baike.epnwcf.com/Article/details/gklxagvau.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gmshczqcm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gbmnhxipx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gslwhhucx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/ggnenkuyt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gbhoesuva.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/glunragyz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gdwxhuemu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gbgbjrlvs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/ghgccvicq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gpyqcvlnj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gdllyvyhz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gccylclnz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gewkjzqle.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gzsbampfg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gtwdhoebg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gdvmtddhu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gkixdivbx.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fktsv.cn/Article/details/gbsjwjfkt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gxzmfvvqb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/groznwujf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gobruekaw.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gxtrikqvx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.vehdjk.com/Article/details/gygzkhpbj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gvikuciwn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gakjrypws.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.bbcook.cn/Article/details/gkvfoqkyk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/grteontnu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.epnwcf.com/Article/details/gigwequqp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gbedvjred.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gaymacgpw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gccwixild.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/ggmlwmewp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gnecljvvt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/giukzgtnb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gnsuszxvt.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcwwmchqf.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/grqznsfee.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzlzsogik.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gwowkjifj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gtweihzzy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gghmcopvq.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gkcdyamdd.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gjkiiedwg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.epnwcf.com/Article/details/gmwbthdit.sHtML

Go:   time.Now()
来源：http://www.share.epnwcf.com/Article/details/grxxligji.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gtzqvwblb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gyiysehee.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/gddggqrcp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/guzqerpqy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/giqrjtnbg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gwlddmgrg.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/ggplchrxr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/georkxrdj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gmijqsmfj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gfvphtblo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gtugcsdvg.sHtML

[J03] 字符串解析为日期
来源：http://blog.bbcook.cn/Article/details/gfhqckkgo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gdqkcdqoh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/ggdlwbyzc.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gdhwojzma.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gltzhkgiu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/glvkqxklc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gxpkygdci.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gsbtynwhe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gvulipegu.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/guuvcwldn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gibsaxcja.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gkxrsczkg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/guhgsdbwq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/ganirjbwi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.yfazqb.com/Article/details/grnezwjrm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gfxvhwech.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fktsv.cn/Article/details/gbfpmkpjp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/grijmnxfl.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gfgrddrjy.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/guxxcqwfv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gsuesktom.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gtszmlusn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gniohjxpz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gptavtnhf.sHtML


<!-- 参考信息 -->