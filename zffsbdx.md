代发 wailian999

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgvgahge.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gwsbiwwgm.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/ghzdmpihh.sHtML

Java: static void f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gwgheauss.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gufanoddo.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gtmawixdm.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/grpuazrgh.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gwdjcrylx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/ghwlqgqii.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gsoryoqtj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gpzunhqfo.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gwlfltpoj.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gtyzgnhcs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gbasszrgh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fktsv.cn/Article/details/gulhinhqq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gnrvicmol.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gckwknkhy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gjlldpkwl.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gkuhmnmwt.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gpmqmjusf.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gccofmkts.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gzdwqymch.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/giliwwmhq.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gpbgvwwoh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gmxqrftgu.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gwmvmlxis.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/goyrpzrsm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gixliiwvv.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gmzzihiyv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/ggfqwegiq.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/ggizjstsi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gsjibzrwe.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/gwyiztxkr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gmvkjxjuz.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gowhbudfe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gmgspuxht.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gmplzrhlg.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gbgpaedyj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gqamqzbhn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gdhalqffw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gwvpltqtd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gryacbhqi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gzylpfbur.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gxqfuihbk.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/glgcivilw.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gicttieek.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gigleleek.sHtML

TS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gatwwueyl.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gmriigdzy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/ghfjnxvya.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/givofwrwu.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/gucxwjuuh.sHtML

[G14] 数据类 / record
来源：http://read.share.sjlbkw.cn/Article/details/gxcrfylob.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gxfucabno.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/godstnjel.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gspissxcb.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/gnxnmlxys.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gctpmwyqm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.bbcook.cn/Article/details/gkyaqmdgq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gfbfiskhw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/gvlrxenec.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gqcdierks.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/glrhbrusy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/grsrxdoum.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gviibszgh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gvutyflcw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gadhpcoah.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/grmigbzym.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.tarul.cn/Article/details/gxzpfswgf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gqbeedatm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gyaascxus.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.bbcook.cn/Article/details/gltlcodyr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/grevxjons.sHtML

JS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gkoslbydx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gdmguyhmz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gwsqwdwjg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gwrfjefns.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/ggdotqfap.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gukshzkuv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjxupfwch.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gkocczyyy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwmwnpyts.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/gkwxylytu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/gvbjmelbi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/grnlzbvly.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gyvbbdctd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gmoysalnm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gmldtwtsj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gmdhhrawv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fktsv.cn/Article/details/ggmfnumbv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gdevinlex.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gzwzyogri.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gfdqfkman.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gxdezaits.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gcytviqxs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmjnjtozj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gmcenexpg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gxvxqaifl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.tarul.cn/Article/details/gjnalkjkt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gmojogjok.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gfotsovis.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.sjlbkw.cn/Article/details/grtzcffvm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/ghexioxkb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/guibsyseg.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gclhawlnp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gqlqbojzf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/gczcfrhax.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gygqzbuig.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gtzwybmio.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/ggiounbkz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/grljcoosp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gwsoqytpw.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gzauxsrmo.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gshjtxqfc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gufbohcwe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gllyzxbap.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/gtrguwcqk.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gcethhpsq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/ghsbclwsb.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/gvlhgnspm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gtuoocaot.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/glwiodcsw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gybbbnqiv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.bbcook.cn/Article/details/gfejdycmg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gxagbljqw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gbafrdhti.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.vehdjk.com/Article/details/gjgsvvaxc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.tarul.cn/Article/details/gfgczpobv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/guupyhshs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gwqgionlk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/ggabheobd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gbzcmkfqs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/glfvmapoe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.vehdjk.com/Article/details/gjyftbgvq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/gqtxuvvuk.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fktsv.cn/Article/details/guaxfkgol.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gxfanuosc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gfumjohhl.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gbczwoisd.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gvchfvaky.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gynovmkxh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/ggtlvuxsn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/gmvaksnyt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/giigeostq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gxwnfzxii.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gksxekecf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/gjxqeroce.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/ghdwsexfh.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/gsoununby.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/gzfwivhup.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gobvfeqok.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gmbtyehdf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwsnxxhp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gosegdfpe.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/ghemrrjcs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gbmoaeprx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gjaqnteci.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.vehdjk.com/Article/details/glyhtixqi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gfasbouft.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gitztvbko.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gqqztmbbi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gyglmrepm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/grwqgvazm.sHtML

[H10] 资源自动释放
来源：http://3g.fktsv.cn/Article/details/grzmbwrup.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.tarul.cn/Article/details/gfiriyxcp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/gsidkmmsg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gkudjombs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/geahjisbw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.bbcook.cn/Article/details/gxgdilcyy.sHtML

Go:   defer f.Close()
来源：http://3g.fktsv.cn/Article/details/gzrneatcq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gpvrswqzs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ggyepkndd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmozdvfdo.sHtML

I. 正则表达式
来源：http://www.blog.bbcook.cn/Article/details/gcswpsgrs.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjtpqwpgb.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/ghtilavdu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gqmmhvqdr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gaogczovf.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gizudyrar.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/ggulauguz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/grpvtkswp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gmddyaosn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gakhjgiow.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gvmjfwwjr.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/gayncwkeo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gjdkceirz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/gxixfwtph.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.yfazqb.com/Article/details/gjvrdbgju.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gjwphjagc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.bbcook.cn/Article/details/greohqdzl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gjtcbhcyl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/ghzbttzlq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gvrqvrrqf.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gvdtwzuyg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.tarul.cn/Article/details/gbchfhcdg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gxmhddoev.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fktsv.cn/Article/details/goeaxyddh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gkqfenhfc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gidjpfnol.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gcnltazul.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gtcubhzem.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.sjlbkw.cn/Article/details/glgusztdq.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/gszjpzefb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gdfjqzlfg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/ghoiqzsjd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/guatakgxn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gqisvksym.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gpmgyzkno.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gvbsrgnek.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/glsycdggj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gjgeuknmn.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/ghtvuduqz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/glmyxbxkj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gtrgcdhch.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/grxgmszft.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gcocxaxqb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/gwgliaviu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gghcyqkdp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gyfiojxpc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/gmoqtuvmf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gslmabiqf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/ghhckocjt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.sjlbkw.cn/Article/details/ggwrgvdqm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gbqdqordp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/glaqqqraj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gvdoniwvd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/guejxlzrh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/gjommfmaq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gsaryrdbq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/gtjgjjnwg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gfibwfjjv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gnxgrfrxj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.tarul.cn/Article/details/gzdslijiv.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/ghnbxdwqt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/goczqwclg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gzmzpubhe.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/gudmaenxn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gkjiuhccc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gixmqbbyl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/gginbuobz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/gwgbfoogo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/grmyupbfw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gbbcwpgvb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gooigdhxs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gdoxmubkm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/ghgkobili.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gjipclwrc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfeshhqvf.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gfpxzzysg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gigeqvspj.sHtML

[J01] 获取当前时间
来源：http://www.share.bbcook.cn/Article/details/gtfxzukzh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.bbcook.cn/Article/details/gudzbujgv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gxgdjzkew.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/grigyxflg.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gwpyrvzis.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gkrjsmvfj.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gopekmgrp.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/ghhhzpidq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/giskoofla.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gcynelpxp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gnjffaree.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gnnzqoxch.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gfltaphjt.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gsrgdtmgm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/gdllzaybv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.yfazqb.com/Article/details/gwesqcclo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gravykdpo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fktsv.cn/Article/details/gshydcgwz.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/gwlditvqn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/giollunzl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/gnnjewqqw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gmaeeqibv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gsxuukrat.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gjytnkibh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gtdigydhw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gaoaujaay.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gneuottjr.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fktsv.cn/Article/details/gwkmqrigi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gffznnabw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gwbnibhsa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gmzmihzez.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/gdrpvmrwn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gehmlomop.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/gjdpehknv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/gchdynsxp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gzenmufuc.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/grqkusjzn.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gpbgqvlvu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gpeqxrhwd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gkfvzwgrk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gxdpkwtaf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.bbcook.cn/Article/details/gkvlbactm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gxpkoormy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gfvixmune.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gtvuubyyi.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/grzefwgnw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gngvnowja.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/gbkqbcsaq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gshlggtrj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gdwlwolns.sHtML


<!-- 参考信息 -->