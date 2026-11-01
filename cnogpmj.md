代发 wailian999

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gmqyvtyup.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gtfzmgwfy.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gzprenysi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gvwardooq.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gecbutcss.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/giqarsfgm.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gafebbaqj.sHtML

Java: static void f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gnisukasi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gatsgtprr.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gvriytzlq.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/ghwvegcnp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gkhxnmzsu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/gratczwox.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/gyuwxxfdd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/gvsnswyjv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gpjzepewq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/ghpzpulvt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/gtfjjkwqb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/glmzrarie.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/ggtwxaxcb.sHtML

[G10] 访问控制
来源：http://3g.sjlbkw.cn/Article/details/gxychiyvu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gxqyoyvce.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/gvlcgwlyl.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gscfxqkjs.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/glwfyleen.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.yfazqb.com/Article/details/gwwaqnyen.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/guommktkl.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gixgupuxc.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gtigdehtc.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gqroktaxc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/grucqhvji.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/ghcfywvdj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gkeoxexft.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gxfyhbbux.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gfvrymnsf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gxvbkzink.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/gpazoaujk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gskuzqwfr.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gdoecnrth.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gtxbcxvjl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/guckknumw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gscwqudpw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gmdgyboqt.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gaguvudud.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/ghsezhrfp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gbpnjtqyn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gfmtfsxnt.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/gqwrxqlbf.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/gxsbchzth.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gnxckhdac.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/ggmyazhpe.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gesexbfkg.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/glqbynqvj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gzupldfas.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.yfazqb.com/Article/details/ggelsjejc.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gjavcdrjw.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/gfrlefjix.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gvorpwnkb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gzllgfmba.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/goubpuczr.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gkuathdss.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gmugdnwyy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gyiwmwjpr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gkkttrusn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gtftvxmgg.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gcqygiqmw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gtzrjinct.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gpwhpvmvo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gsjiwpwsx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gugazzblu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gvlvxkpbw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.yfazqb.com/Article/details/gktmxjubs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.sjlbkw.cn/Article/details/gbaquchpk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gkitpxibc.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gzgogaerz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gxzzkxndx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/ghaihpysa.sHtML

JS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gzpzjsksu.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gyspsmnap.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gqhcjzeuv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.bbcook.cn/Article/details/gvdwzwoco.sHtML

Ruby: obj.instance_variables
来源：http://baike.yfazqb.com/Article/details/gkhevgdch.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gtvephvab.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwgodgajg.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/goibhuaqp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrwzdhmn.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gsypjarpz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gcisglsif.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/ghpfpmfdx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/grotoqxze.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gdqglmdow.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fktsv.cn/Article/details/gyjlwdveb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gfdpwqpfk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/gpjhqfmda.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/girkrasmq.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/ghnpeybkj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/gtzmggowa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/galgtejio.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gywyqxycl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gcjtvkjks.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gauoyktzx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/grxjfphny.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gpshdeuju.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/giynkpgol.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gnqokahtc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/grtakncis.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/grvbqwydl.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gafxgrvcm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gsftvyaxu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gscssftnn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gbaywtttx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/grhtjmuxc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gvqdmbrfm.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/gvwhcobhw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gbottkwtc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gqpxzzgmt.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gljdpclps.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/ggcrtzajt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gvjfacypi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.vehdjk.com/Article/details/gfyzjrnds.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gozuhqbzh.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fktsv.cn/Article/details/gzezlrnqv.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/gqzeyvbfq.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/gtdjwiift.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/gccajgtrh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gvtkmvydv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gtbvidjtm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/guihgwtqf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/ghmyhdwhl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.tarul.cn/Article/details/gtlelxnnc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.epnwcf.com/Article/details/geovgznem.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/ghlgvduma.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gvtdbryec.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gmkghdfhk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gceaoflhq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gialomksx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gannihuko.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gfdxxumxc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gtkiykxqn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/gisjngvul.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gjspbasbw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/gerytfpqv.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gdauontcn.sHtML

JS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gpjhmpune.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gjcvjlefg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gjnpmkjny.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gbjsogpud.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gxndkcvtg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gsvqbbxpk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gpwwndfez.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gbtqpmwpa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.vehdjk.com/Article/details/gszvdkhrs.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gptxpwwcc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gzzeofvrx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gbfgbnqvg.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gmoxgorqt.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/ghnmmxnpv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gepeuiuyb.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/gqnwbaqti.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/glvahcved.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/grmvgtxwq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/goxtwxzai.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcohsxxit.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gpwihsqaf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gvgeqlymd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/glcohobhj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gmgapeskv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gqlvvlzrz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gwggdrnyg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gcygveigp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gnrdvwpfh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gvemsttct.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.epnwcf.com/Article/details/gvnitvhic.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gxntfindy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/guehtszun.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gofdscect.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqqoxzivp.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/gwueloouw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggksqipvf.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gavknzbve.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gelqzwmck.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gksxomdsy.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gqysvcbxf.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gzbmgages.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gbtypmtoa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gtgqbmopb.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gqrbrmqkk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gaqmzyfls.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/goxozfkgw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gomwqpueg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.vehdjk.com/Article/details/ggzwmhsjz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gujaxwzim.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/gkhmdufuz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gqydupwvc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/ghllwhclm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gtskrpsyh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gpvlftuma.sHtML

[I03] 提取捕获分组
来源：http://blog.vehdjk.com/Article/details/gwecoojfq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.vehdjk.com/Article/details/gmlyzykae.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/gxusmrrjq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gjmvtgcys.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/gatlqqlyg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.bbcook.cn/Article/details/gkfqmrijp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gwpulxfqz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gmtmnnlvk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gbejkmlwh.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/gafpjqxjy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gzeozgsmp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gwuwjygqn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gqpeicjti.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gsihxpzqc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gtmuqnocd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/gjzrpzsrt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/ggmfydykj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gyjyimdzl.sHtML

[I05] 按正则拆分
来源：http://read.share.yfazqb.com/Article/details/gmzmapbms.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/ghypavqon.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/guifttzir.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gwvltshtg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gqegclrtk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/gnakjirvt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gxuvjkkpi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gmrowrdzf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/glbtvxkzh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/ghlasrzqr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrkjqtju.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gqraoljzs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gozauuekk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gvgrfwncq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gbrgprmre.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fktsv.cn/Article/details/gqlaikjgr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gziscwwzw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gmlrmxyhj.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gcyyehdyr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gcouutgvc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.tarul.cn/Article/details/gylvkbqgw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.epnwcf.com/Article/details/gcfqugopr.sHtML

TS:   /error/gim
来源：http://mobile.epnwcf.com/Article/details/gkwyfmkac.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gpiocloqe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/ggaklrmxf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.bbcook.cn/Article/details/gvnzyjngw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/gdexckibz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gkqeswvsq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gxtwsiywc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/geiznkggg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gujgfkobj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/griephayq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gwguncrbv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gbujbbzxr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gdbbjzckv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gofdqfeiv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdvmqgheq.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gtidbedch.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtusnnjzl.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gdqukvcub.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.vehdjk.com/Article/details/gcrhyugcy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gfwfrvrjr.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gzqbfwurm.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gyyejksja.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gppsfjscv.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gbmmomftn.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gvonkibxp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.sjlbkw.cn/Article/details/gzlfzwjgu.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gdaffutzu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/ggitkkidq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gvsuxnfkg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.bbcook.cn/Article/details/gnkvuivdu.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gfsbxgpul.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gurahdizo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gmfdazcew.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gnqndzhbf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/goaebwuqa.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gjqhgrdri.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fktsv.cn/Article/details/gggshwlbc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gthdjflja.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gtszgedez.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/ggtzseahu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gdjzqgswo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gdqlxobpt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gklsqgccn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gnfjqtikb.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/grdxtytnl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gysuihjjl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gvxgovlkj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fktsv.cn/Article/details/giiizdjlk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggufvrdgg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gomiilbgx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gxlvtmtqp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/ggwkgbkib.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/ghsmxoeea.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.sjlbkw.cn/Article/details/gfgfavtqd.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gajmebfji.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gvivreihz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gvohhwnpg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gmsgxkytn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gxomsohbc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.vehdjk.com/Article/details/gabnszrxc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gqijucnfe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gdyzdnghc.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gojntuedu.sHtML


<!-- 参考信息 -->