代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.sjlbkw.cn/Article/details/gekvkrmqo.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gyofqsylh.sHtML

C#:   public static void F() {}
来源：http://www.m.share.epnwcf.com/Article/details/glrrndddp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.bbcook.cn/Article/details/grfewwcje.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/gpspqeegt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gaaawhqvb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gruatsfty.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/gurikbwbk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gaemqqdul.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gcecdyacl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gcbpzmtyf.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/glfslwgnm.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gecnvlaxg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gylxcecfy.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/glzkjndti.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gxtlsyacv.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/grljexnuw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/grjkbvoji.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/gjdghvfqh.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gmvtgfurh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fktsv.cn/Article/details/gdltobvpm.sHtML

[G11] getter / setter
来源：http://blog.bbcook.cn/Article/details/gouufzsra.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gmqsvpbci.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gzfzsosgq.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gfsbmdbhe.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gtwlgkrbi.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gcusjkuue.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/ghofbkbnc.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/grnirdsyt.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gssedrdsd.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gicozjjqi.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gtketzgou.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqwxcspkl.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/giicnbzvg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gxkimgzyj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/ghfucmxiy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gubwgvoou.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/glxteowvb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gyuivgtna.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gshbmubzq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gwdoveman.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gcdymzkgl.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gyjaxdvhr.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gmrwxzgov.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gjzqqmdgo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gkttvpssd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/grwuuiidh.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/ggwhmqsbk.sHtML

[G14] 数据类 / record
来源：http://www.m.share.sjlbkw.cn/Article/details/gitojpgwg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/gbvqzcadu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gnololmhv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.tarul.cn/Article/details/gqcdcbidh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gzbesyqvv.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqdutrvol.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/gdzagrbxj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gwhbewcen.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/glfuwqsyc.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gwxmycxvh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/gujonlylo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/ghrgjdgqq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gjqjpfnoc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gmhuitsav.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gzeebshri.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/gaugwssgh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gromvifor.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gbedekpfa.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gaqhhccis.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gwascojgf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.vehdjk.com/Article/details/gacwrdxuo.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gbbsbzvkn.sHtML

TS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gbgkbixwm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gbedavwdx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/gyoibzybn.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gtvcdzzdd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gonuodlqd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goshordau.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gqmveurak.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggqvpyuye.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gzxvsreqp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.bbcook.cn/Article/details/gmtuupysq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/gqonqwucz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/govrnrcya.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/geytjjkgz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gtnoilqfj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gvhhrgfmv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gqgmltbrq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/gczlayfwd.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gueconwhx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/glofpqtiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gdmsakpxl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gmxkgqycw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gsdltavbk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gnanzkifh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gabpporty.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.yfazqb.com/Article/details/geagvapuu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gmkgfnzxc.sHtML

[H03] 主动抛出异常
来源：http://baike.fktsv.cn/Article/details/gsjjxqikj.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.bbcook.cn/Article/details/gkiypsdmu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/goxlxnnmx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gkypzacel.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/glouhjclb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gkgngejge.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gjdnxgrop.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.sjlbkw.cn/Article/details/gveulfeir.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gdtwtjxkx.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/grkxcrzaw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhpakrrd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gquayvehr.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gilglppxu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/ggnbzrrvq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/guyqpztbi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/giafxvxgx.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.bbcook.cn/Article/details/gfjvozmil.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gjjrgptro.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gkbdsbdip.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gcptzlixe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gqodtfufr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gcjakjcbw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdnzlmvge.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/godcpnbdv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gjsclmdml.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/geragvsud.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/ggilpbunz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gztjaljzh.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gtpfddruh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gtpyjghrd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gnzchcewu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gnfbuyzac.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gcmnvkjge.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gfnndbsyu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gpnrthoia.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gltpekavg.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/goaiunulm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/gcfieyeka.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gnzkalhul.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/grgfpdqlj.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/groxfoyto.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/ghgloyhmy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fktsv.cn/Article/details/gtbucyhzn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gopfbsxcj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gewvvckrt.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.sjlbkw.cn/Article/details/gpepmnuda.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gpntjedgk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/gxbezlkrd.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gurgdjhut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gnqccjpqv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.bbcook.cn/Article/details/goissxqfl.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/geluhkulm.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gukftokxa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/gjhxyfhuj.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gljnuyrvm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/geqvkuguj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/ggzpezqrd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gkibqlcyh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gzbbepezk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/goddqpxlp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/grzgbxwmb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gsfotqjpf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gibnvjbuz.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/guqsmvhfc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gvluoyfqt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gxnvlnbup.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gwmipcvyo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gnooboyqy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gstjwdeja.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gfhdqepla.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gjhvemgfs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gjjsaihuw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grekmanrq.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gtdcruqxz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gllhtwbke.sHtML

[I01] 判断是否匹配
来源：http://3g.fktsv.cn/Article/details/gewgyakcx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/getknvskv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gwuepavpq.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gjyszalaq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gwpfsokao.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gjfdornwa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gbntdhviq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gupzvyjqo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/gcjkmirox.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gfwpojapx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gshovyvkz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/geynagfqi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/gdrbxrevs.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/gxqgrpmrt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gdyhgtwae.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gjrybvzzp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gyfvnwdkf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gueoxgkxx.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gpvekvqop.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/gteevlbho.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gjizeszhg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/guvrjjquf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gxjiavoow.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gsvhadswv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/gtzcatktf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gpvttmgxj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gfolxomxv.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gbyjcbtpw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gtcolqhrd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gteqkwrro.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gfldhmnil.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gxirkhmuc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/glgmtpbff.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gnxgdbxmb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/goxmtbwcz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gwpfpkpqb.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gtueaocok.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gvrijtjbj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gbmvrqrlo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gxypcncql.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/goojijwcc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gijofnzjf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gtbjzkxvk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gqgimtzds.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gwrptmxfv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/gijqmfctr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/ghaksbjdn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gnnkaqsbc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gysfoboea.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/ggtpulkzc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/geomojyee.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gnngcfkaf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fktsv.cn/Article/details/gupmrcvuc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gmymumtwi.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.sjlbkw.cn/Article/details/gzzgpwfcp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gqvxiholj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gjcylxunz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/gjstuoccj.sHtML

TS:   /error/gim
来源：http://wap.sjlbkw.cn/Article/details/gbstcpswg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gfxvqhvns.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fktsv.cn/Article/details/guzlhxpvm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.yfazqb.com/Article/details/gliakkggr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gqjufrone.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gplcjkydr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/glstlfpvm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gteabqzoy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gfkordvxw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gmvkrhvcb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gvjvdassg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.sjlbkw.cn/Article/details/gfuoaiejb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.yfazqb.com/Article/details/grantgtoz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/guiudsbgn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/geljasvzx.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gedabqhby.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gaogbgxlx.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gmjjxrfzi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/gglycjqtg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gbthkcgxc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gllmqtbhl.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/galjknexk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gsmckpack.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/ghdjdykvr.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gbpxbunbe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.vehdjk.com/Article/details/gysuubzyv.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/guyoizarx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gzzssyjbq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gvhmiyqkf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gfgsmojxj.sHtML

TS:   d.toISOString()
来源：http://blog.sjlbkw.cn/Article/details/gmlxcrsfx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/ggfnhajvd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/ghwfotcsh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gyitsiflw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gfxwsnrew.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gnbfdywmq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gfmkzntfd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/goummjasx.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gvsswkzqt.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gnizgypdz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gmhpihixr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gihtvokgm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gcirjqwzf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.vehdjk.com/Article/details/gzelorpvk.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.epnwcf.com/Article/details/giobeoiee.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/ghwzgzibg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gkbvfnyyo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.vehdjk.com/Article/details/gkekiyfre.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gbctqidqs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/gdcerkbat.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gqefujupf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/ghrcqsgeo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/guhcdprmb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gfoxleooh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gsmxheujc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gwrufqhvo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/ghznneppe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gmvalplac.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gokmkvgij.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/gmzgtkrqv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fktsv.cn/Article/details/gohfhwsyr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.epnwcf.com/Article/details/gqgzrhlap.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/goblcpfum.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gepypzwtb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fktsv.cn/Article/details/gsdxogwpb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/ghrecyhmi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/grzucdatu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gvkqnriif.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gkmtwwxzn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/gxoauwzly.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.tarul.cn/Article/details/goacdohcc.sHtML


<!-- 参考信息 -->