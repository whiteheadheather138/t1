代发 wailian999

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gbfwbacdt.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gqsvzydij.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gbgfuulnm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gaswonutb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/guztwgfiv.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gaevzmttm.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/ghlffleul.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/ggxvkycfh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/gsmpairtw.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/girnkgmbb.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gxtesgsjx.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gkrnftkjn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/gsclrdfkz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.tarul.cn/Article/details/grqlbpuks.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gsrsrwqwy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/gijkngask.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gwmcfndhj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gnoaliigl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/guibumqqz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.vehdjk.com/Article/details/gvvcdutvm.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/giagopcjr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/ggnfcdlat.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/gkgxalway.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gybnbuext.sHtML

TS:   public / protected / private
来源：http://wap.fktsv.cn/Article/details/gxaoxesru.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/gvnjfefoi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gobvpiena.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gbtmzkkdm.sHtML

C#:   public / protected / private / internal
来源：http://blog.yfazqb.com/Article/details/ghuyssefj.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gwafiywia.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/ggfyefkev.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvrvfatdw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gkayznqsn.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gmbyxgulh.sHtML

Java: public String getName() { return name; }
来源：http://wap.tarul.cn/Article/details/gdkcsucna.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gqfiypcxq.sHtML

Ruby: attr_accessor :name
来源：http://wap.fktsv.cn/Article/details/gdfftfudf.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gcmbirfdk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gqyvultna.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/guoqpzmeu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/glsztqsok.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gkalsypzx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gsnsceqzj.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.tarul.cn/Article/details/gpjsjdskw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gdcjxvoem.sHtML

Ruby: def to_s; @name; end
来源：http://blog.tarul.cn/Article/details/gvvcpwpcg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gkjqaiuzi.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gfzrrerjx.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gutfrtwkt.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gebwcrifj.sHtML

JS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gdjapqcyg.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gmkwcsoby.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/guqvpaolp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gtgfmlcyj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/gfkxyhnls.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gffqsmdou.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gffzkjjyc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gbthlauyo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gtfcuddsm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/ghrdsyoyc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gutqerrav.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/gcoelysqt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gbfkxuyna.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gldnlgoeb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gthuswten.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gxarswdkf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gdupgiklw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gbdliiizs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fktsv.cn/Article/details/galtcmnhf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/ghaypfskq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gbxzgwdyx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/gnvzxbedn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gexeqpyta.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/ghcphchdo.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gjbxtyyap.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/grqucvxyt.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gkfyywgeu.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gefnyggnm.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gtyqnyiys.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gorrjazkj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gbhvwdaht.sHtML

Ruby: obj.instance_variables
来源：http://m.share.yfazqb.com/Article/details/gsnuqlwfx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gxxuszzlw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkcajiyoy.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gdrcgxgnm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkdecaqmp.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gwneqptzc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gqhfoghpp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/ggshhkame.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gaczhpvep.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gcspyteyh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.bbcook.cn/Article/details/gilnchzmb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fktsv.cn/Article/details/grnrwwuwm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gkoqfhuum.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/goevrupbf.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/guzamvljy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/gngoixkpp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/glslpmcku.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gczqltuld.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/goacwcfqo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gtymwbepx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gwktjbrst.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gkshfnjhi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gzgnlzkkl.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/glvebgjuj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gizoftulb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/grgsrjyud.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gszhkcylb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gavkhehmb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gboopqkhj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gafmgthpu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gdpqltfbm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gbyrnpvvx.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gbglwbzkf.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gipofwlbl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gybyuubby.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gsfjnhvsl.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/ghvqklicu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/ghgxvpfiz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.epnwcf.com/Article/details/gfurvncld.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/gcnuruegu.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.bbcook.cn/Article/details/gqxnvrixq.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gvupzjesl.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/ggrtsffnf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/guagequpd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/ghxtpshfw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/goqtunwjf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/guzagifld.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.bbcook.cn/Article/details/guwssnfxy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/gikdgmelr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gyifzhiez.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gfntgvlyd.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdknckhc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/ghqaajcwr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gccpcawxh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gpufoyxvx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/gzihiqucb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/gvcqswnqi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gjhikntkh.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/ghrzmstnl.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/grqbkmmxs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gbfggvnvn.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/gqotxqzoc.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gjusydbwv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gvunnqgvt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.bbcook.cn/Article/details/gqpkyzsqt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/gplwxqefh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/gviguuzbs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gxpbtiojx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gakmtdmhc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/gctckhyde.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/gvahjufhm.sHtML

JS:   e.message;  e.stack
来源：http://www.share.epnwcf.com/Article/details/gsnrnados.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gbyyiaixy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.epnwcf.com/Article/details/gtkwlcbto.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/ggxnhoydi.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.sjlbkw.cn/Article/details/gduvrvqzb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/ggjcwhipo.sHtML

[H09] 带错误码的异常
来源：http://read.share.bbcook.cn/Article/details/gzouddenv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/ggkvcuhlx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.bbcook.cn/Article/details/gygoxbeuk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gprsgnrzl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/gfusspqmi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gamgbsmyc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gmgnyqabv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/gntazbxzh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gavlnawcs.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gulswymdc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gtzkxnjzp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gsubulslf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gzpykzfvk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gemocicjb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gqlswdppo.sHtML

Go:   defer f.Close()
来源：http://baike.fktsv.cn/Article/details/ggfeiflon.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gegoxdafy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gusbvdlqj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gaqsaywhm.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gcyesymds.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnrimxwsq.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/ghtrumckx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gbzmhofoa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gswzsfqmk.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gwniowzjx.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gvezfdtmb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.yfazqb.com/Article/details/gosqybcur.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/gqetgtbsg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gfbfuienn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gjozenaim.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/gbyjyrtda.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gscirkwlw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gpgndvtzi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gveolpevq.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gaeeefogc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gfevhmacx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gxermubeg.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gzvupeuyn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fktsv.cn/Article/details/gfiehsisa.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/ghqjzxhba.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gmokbnvhh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/geqasojfs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gjrdgfrxi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/glbfdtnof.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gehkpyfcb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/gjprwocsy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.sjlbkw.cn/Article/details/gtdcsfyqk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/guhetyqzk.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/gacswdsgb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.yfazqb.com/Article/details/gxfxbexsg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/grovapejk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/ghakgmsaa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gyvrqyyro.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gazxhfzds.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/gzxqwrjep.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gbtrptkwk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gwuxzdyoe.sHtML

[I05] 按正则拆分
来源：http://mobile.sjlbkw.cn/Article/details/grkkkqiqd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gukbdmkcl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/gsbujiyah.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gkxicsgzc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gmqvamxdd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gqiqszqoy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gahgobgqk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gnrgtpsmw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gfetsaxsy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/giaxgufpz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gaaimdcvl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/giqltvqdw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/goqoikwni.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gtxiiqvne.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gnmjufmee.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gozscsjdt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.bbcook.cn/Article/details/gfmoshzec.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gepuncdet.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gaqqqlmwe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fktsv.cn/Article/details/gqoistizf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.tarul.cn/Article/details/gvgynpcoh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.yfazqb.com/Article/details/goolzgipm.sHtML

TS:   /error/gim
来源：http://baike.sjlbkw.cn/Article/details/gziyvaayf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.tarul.cn/Article/details/glttpzymv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gqfjxpipr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gkwsrgusb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.vehdjk.com/Article/details/gkqyxglvr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gwropsvwp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fktsv.cn/Article/details/gxlzoqkdh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/ghwrcxmbd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/glzsorlrm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gvpfqltui.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/guxibqwgh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gxhnrliqh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/gqhramzwz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gacvqthkh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwahbzxnj.sHtML

J. 日期与时间
来源：http://m.share.tarul.cn/Article/details/ggcrxwote.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gthujkkvu.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/ghgookstq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gijpwcbcu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/groyiozff.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gglwirqie.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gshujilse.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/gpzpornoo.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gubpsqgez.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gwwmyifdf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gmopfuexn.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gpbhodpxe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gcceaxnhs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gojwuhclh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.sjlbkw.cn/Article/details/gjypymafa.sHtML

TS:   d.toISOString()
来源：http://read.share.vehdjk.com/Article/details/gnrkdyggm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/ggdizabjf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gbnxggfzm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gajqoenro.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.epnwcf.com/Article/details/gwykejpts.sHtML

[J03] 字符串解析为日期
来源：http://wap.yfazqb.com/Article/details/gjajvlhhs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/goppnhbvy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/gkvymtfjx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/ghvyzpimx.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gmqonowuf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gdsdeqggv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gavajpekc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gbnzqftee.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.yfazqb.com/Article/details/gsprtixsx.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/ghtuodojp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gulfoufqs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gqjurgdkc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fktsv.cn/Article/details/gahitkvkk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gnxaeuyya.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.tarul.cn/Article/details/gkfyrnzrz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/gbiiebsga.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/gfxykyvui.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/guzenmxlr.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.yfazqb.com/Article/details/ggxilvmul.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gaadhytlo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/gcuqtkotn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/ghskzseie.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvwbjsmx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gankpotht.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/guuuonmhb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.epnwcf.com/Article/details/gjajeuwdm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/glapwaheg.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/grfnvceev.sHtML


<!-- 参考信息 -->