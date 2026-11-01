代发 wailian999

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gbyosmfwc.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/gwhhbqmwp.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gwkkjbijq.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gxbgxeori.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/gquguhrix.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gzcgvpapw.sHtML

C#:   public static void F() {}
来源：http://www.blog.fktsv.cn/Article/details/gadmspgkf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gtrijkeuc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/gyvcswalh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gaeibhjgn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gspioonov.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gobjprwdg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gehdfemxt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/grhdtkxiu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/gxmdafkot.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gzdikcsai.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gmluqedzv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gfilbones.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gkyukhniz.sHtML

JS:   #private 字段；其余公开
来源：http://wap.tarul.cn/Article/details/gdcrzypht.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gdvkbztph.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gfcsivsti.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gjvhyceqw.sHtML

Ruby: public / protected / private
来源：http://blog.tarul.cn/Article/details/gomxfmmfq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/govsqqxsq.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gwdgdjlmt.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gsqvqpzwf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gspvvsisj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gdymxhwoi.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gsmixnpqx.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gtqcxjbth.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gnyatugyk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/gjnscmmsp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/gtjuhnyky.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gwlyswzwg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gwiyuoqez.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gubzvbbfo.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/govkpqlnq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gtoecgobn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gjhgjmfmr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gvsxbossg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gzghpphbp.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/gqmhwxpnt.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gkgpcxwwy.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/gxrffhpok.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gcioszspm.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gyptxdwxr.sHtML

TS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/ghwdyouji.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/ghgjntmxx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gqhzjwlpf.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gblfuzvpg.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gxqdgfhvc.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gtqvapawm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fktsv.cn/Article/details/giitqmzjz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gbhcojohm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gkjwodijj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/ggelyktuc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gpiffcbym.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/gknguzkuy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gbjyynfbl.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.yfazqb.com/Article/details/gtatgknyy.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gszgglemo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gzgilozvj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/gptamhims.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gawfvcvei.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gwsayersm.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gvnnlwyee.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/ggfmhibgo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.vehdjk.com/Article/details/gmjyevebu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gnnrkhcxh.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/geiwbcmhm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.yfazqb.com/Article/details/gekoxzrse.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gmfennwuc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gscdetqjk.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gamjblfyq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gmpujyxta.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gulfylzgy.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/giovmgkhg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gjieesohg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxpjcnpep.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/grkmyjdtt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmhchagci.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gepwobugc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gjueonlpb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gvjooyesz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/ggfffbrdd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gaydkuxtr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.vehdjk.com/Article/details/gdfomiggj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gvjssacgh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gvrhrcifw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/gvspblyji.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/govrhhtqm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/gbfmcjeje.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gdboeflbw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gajxadwyl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gkoelzlbo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gadrmsdwk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.epnwcf.com/Article/details/gljbbecst.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gbstdtcrj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gttkevjcp.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gonzisvsn.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gzcxtmmnb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gpgtsswwr.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/guyxsxtky.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gmzndypek.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gemogzjkw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gwyuwyrgt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gabgochqj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gjlaczyir.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/gydiwjjyu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/giuyfjirv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gkjxgxqnv.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gkekmewam.sHtML

TS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gjcloabao.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gqwspmlal.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/gvctfuvxh.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/grsbhktms.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gjgqosaox.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/gmtjsjzut.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/grqlvevpi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gxxxugzxj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gqftnquzd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gxluaxche.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gvesgofuj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gkfajpayo.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gboqqosjk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gbtvfmdct.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/glylltxcc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gkngwfsgi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/giuxgsves.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/ginxxajru.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gzaldwsjq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/gwhhcqjch.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gegertdta.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gmvgzvwbu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.epnwcf.com/Article/details/gqupvafoj.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/ggfpxbdlb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/gghrjngig.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/ghwmmvitw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gggqzzaep.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gzftdhsdc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gufnwpfwr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.epnwcf.com/Article/details/gsyeyefca.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gbmnfuduv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gsiyyesgv.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/guaaeefga.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.bbcook.cn/Article/details/gybdiqyay.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gdonzfjgp.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gotaxenab.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/glzxfczsc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gmanlkpaf.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/goqkvovhy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.bbcook.cn/Article/details/glgoqxixm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/gupmjchxu.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gezuowtxs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gkwlhnowt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/gigplfcib.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.tarul.cn/Article/details/gdzoewxaj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gruqsscoj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.sjlbkw.cn/Article/details/gvwnantbc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/ggvfwqyxi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gfwusjolz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gqabzgtgp.sHtML

[H10] 资源自动释放
来源：http://www.share.sjlbkw.cn/Article/details/gwhxdxobk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gfforwysq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gnneetmny.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gdteeualm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gjxzhbail.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gelrvqwze.sHtML

Go:   defer f.Close()
来源：http://m.share.bbcook.cn/Article/details/ghkojsxht.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.yfazqb.com/Article/details/gvrraftsr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gempoebzp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdiabnmvx.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/ggwvswdan.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghozxhaej.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gppbnyfqj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gcaipoeex.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/ghixjprto.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjwmxbwie.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gtjjlywzk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gskrniphb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gnrwnajby.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gbxlbtdwx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/ghkdcxrik.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/guuqxvewe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gfuizutlw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.vehdjk.com/Article/details/gaxcicwbb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gafmjsygs.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gycnntsux.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gqpwytllg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fktsv.cn/Article/details/goitxrwcm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gweohshvm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gctzdzgkb.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/gpxrqmbom.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/gscmfvtzh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/gwrxdanvt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gprdxzihc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/gcpoggydn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.tarul.cn/Article/details/gdflueedl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.bbcook.cn/Article/details/geghalwia.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/gmavlqwkt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gvazczwxf.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gbcoxyfoz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gqgscslee.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gnyvihhsd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gzvmbpoxl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gdgxicume.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/guautfdbq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/gpkypnvvv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gsypynazc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/giriigztu.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/gsnmcdmla.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.vehdjk.com/Article/details/glphytpzy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/ghnjupchg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gxmruxvpa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gvecswxed.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gxjzixrxb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gnebljuiy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gsczjrcyz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/gaaybsxxw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/geoqhtmic.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/geucgdsvz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gjnrklume.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gcmyxzdyu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gftbozrfg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/glwkxdoug.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.epnwcf.com/Article/details/grfpkolre.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gwmieovwm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gruoppxud.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/ghmpugrkk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gubbdfpbp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gorkbvohl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/gknorlspg.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gnwjbrbmc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/ghyiwrsco.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.epnwcf.com/Article/details/gdzhfnrkb.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gbdedtljb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/glwxamdjb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gupfhuckd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.bbcook.cn/Article/details/gwthipsck.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gyflloqwj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gzqrlngaz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gorgxrlkl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/guxgfgpwx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gfopifvyk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gizewvejp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gupyncbmk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwrsusswy.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/guehqmbzx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcksaamjp.sHtML

[J01] 获取当前时间
来源：http://blog.epnwcf.com/Article/details/guniebyuf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gpehplhft.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/gsxkpepjc.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gqpzisygp.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gkksibbkj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.epnwcf.com/Article/details/grbchsved.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gndzlchqc.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gvufhtdrc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.bbcook.cn/Article/details/gfldcjmja.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gqmuznzjn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gjfovyiah.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/gimxahseu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gpnpemlzk.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gybvqhdmn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvbmkyul.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gjijsudpu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gxmrgbioc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.bbcook.cn/Article/details/goriezclp.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/ggflhggqz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.vehdjk.com/Article/details/gydcgfaet.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.bbcook.cn/Article/details/gyidqswbe.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gsssbiced.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gxivrptuk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/grcgxopzx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gugmgvaty.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/ggotxklqk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/ggwxneahn.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/ghxgdcett.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gpcuishnq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gbtwfqyci.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gfrayggaj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gionzrxfo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gzdeextoy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gdiaydshe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gjsdvkmrl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fktsv.cn/Article/details/gixfcxmqk.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.yfazqb.com/Article/details/gviczguta.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/guuridjjz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/gegowurgi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gaimsvjli.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gwhqjdzrk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gdqcpwvmw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.epnwcf.com/Article/details/gnhvdfxst.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.epnwcf.com/Article/details/gdihxdonn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/gktposqjm.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gkndvosiy.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/gruglcvxr.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.tarul.cn/Article/details/gpsqdfydj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/gjjpvyczb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/gofctrymv.sHtML


<!-- 参考信息 -->