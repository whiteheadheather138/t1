代发 wailian999

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gbsgxhjnn.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/ggubblhix.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gkmrxtwdb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gpoazpnjl.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gjbxbpedl.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/gknzazjzb.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gtboiosei.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/garqlcmoq.sHtML

PHP:  public static function f() {}
来源：http://www.share.fktsv.cn/Article/details/gwrglvgqq.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gerxqqmza.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gimgjpmwi.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/gqqmnlgxw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/gcczzzand.sHtML

Ruby: def self.f; end
来源：http://www.share.tarul.cn/Article/details/gbpgqnsao.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gvyzydwfi.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/goxxwmajn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gftuhjwif.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/glbgoafpe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/gomaedcii.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gjghxthxn.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/gmmzkdlrv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/gxslwfcly.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/gulqfexiv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/godoqkfhr.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gkqaprlls.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gtixtpofr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gadiaiktr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gdsslwzon.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gxlpstsnv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/gzsmzlxek.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gsqzmnfni.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/ggrmzlsvw.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gocqqnezn.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/genkhahrq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/grbgldmbr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/ghqoeopen.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/glkspthxf.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/geeimispd.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/ggnaxdvtn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gksrsmcch.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gaossoqiy.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gjounvtzj.sHtML

[G12] 对象转字符串
来源：http://m.share.vehdjk.com/Article/details/gppwqgvqq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gjdtctfwi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/ghzkdutxg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gxtxahpqy.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gyzhzezjk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gydcetbee.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/glnpczgma.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gidenpqgh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/ghnrsckzd.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gzdklpfsa.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gcwivkssb.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/giiqxmzla.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/ghdkwbsqv.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/grvdoxwzu.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/geaavkjuk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gymffpjgf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/ggqivomjf.sHtML

C#:   u is User
来源：http://wap.sjlbkw.cn/Article/details/gbyhffjtt.sHtML

[G14] 数据类 / record
来源：http://read.share.fktsv.cn/Article/details/gblyvkysj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gnyuzqmyf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.yfazqb.com/Article/details/ghlezbqde.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gvkvblyqf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gbmvucsyy.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gqyojkzsj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gbxzyabqf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/gdtugvvmg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/ggfdhjhjd.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gdhohbvul.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/gyijiljjo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gxjxotmfa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/ghspmvlzw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gaffhdcrd.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/ghjtmqnkv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.epnwcf.com/Article/details/gcvuvagmo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gemfkxwtj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gpyuxbspn.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/gybayxyfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/ggxeltpah.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gaaudywnv.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gakebkslb.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/ggcymbrwt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/ggwdunkxf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/gjfcronft.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gwjkizefu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gjtdjsdqk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gohhmbzdz.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gmbmbpyto.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzdhngcmk.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/gomvstksv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gglspafph.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.epnwcf.com/Article/details/gxlyxzhnx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gahbkcsea.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gflalxkfz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/gnmxhtunw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/gmysrhbeb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gctyhxrzl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/gagntxbpq.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/ggxlxwphl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gcwvkjbpd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpltgeqce.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gbcmxmhxy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gcmuxfwdy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gksbntgex.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/ghaxbxmjj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gikhevtsh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gmhumxqkc.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/giednkiad.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gunoncovt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gncperajk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gdcejugun.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gmzugccti.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gljcgjbdv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gomloxogw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gyfrgycpy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gxlkcskxq.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gvhcucziq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/gcvmxkemy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gsabgetya.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gmjixswyu.sHtML

TS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gwaceqceg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gkawuzjne.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gzhpvamon.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gyhqujtgx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gkwlgksae.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gidwcgdfm.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gbkvxuxzd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/grbjotizt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjzwgqgyq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gyuyouitz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/ggvfglgam.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gluaoldrl.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gphobqspg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gbaurgtjd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/grhgtljzo.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/goqlcsjul.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.tarul.cn/Article/details/gprihzxch.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gbqaetarb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gsmgshfpi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gqptyoosi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.yfazqb.com/Article/details/gqzolclao.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/gthqdozyv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.yfazqb.com/Article/details/gakbyrxpm.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gjwddiktz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/guccygewc.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gmcxurski.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gzzqhturh.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/ggakmdlvj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/ghylqhnzg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gxaejxfzo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/gpzcthzgz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gzbhmrrgj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gpggvfjnr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gurxdxbfd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gjuirrzrd.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gwupvplwe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.bbcook.cn/Article/details/gdttuiasd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/ggcmuggmw.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gifricvmq.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gufgggzuc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gnnubnseu.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/ghhsrlvgg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/gqlxceggy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.bbcook.cn/Article/details/ghmqxohrg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/govwepjuj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gpagcdqbn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/guhybtbza.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.tarul.cn/Article/details/gesalknqz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/grpweepnk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gbryvrhhq.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gpiqfeeoj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.tarul.cn/Article/details/gtgihowjm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/gxflifwxj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gonzultcq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtnyqves.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gheseqqur.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gjdythywd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/ggabfwhga.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gncmvjnjp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvfwknhur.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/gzgvwyfdu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guslvmvml.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/glmqqacqr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gkulvtemp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.bbcook.cn/Article/details/ghwbdobdx.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gahgvktro.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gmihdfomf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/glrbcmsah.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gmrgddpzi.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gqgzibhwn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.epnwcf.com/Article/details/gpvznajol.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gcamgwfdk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gxsxgiioz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fktsv.cn/Article/details/guipsabiu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gjvqlatbe.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/gjianximx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gcqdeuhgk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.yfazqb.com/Article/details/guyjddoxj.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gmnwrpxbq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gummtqcgl.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gxynvjahp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gowlsryks.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gobanprlb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/gscngultf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gzaeqkopa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/gxtplkqgh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.yfazqb.com/Article/details/gmopyhdwm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.tarul.cn/Article/details/gfmeysjti.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/gnlonzzxd.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gwkdaictu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gcbibhoju.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gbcnlevbh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/goomxvjtu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gohtupkse.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/grpmsolbx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/glhabgmsj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/genstfkiw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gvrsuueuq.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gmltsehjy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gdyhgzlqs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gsieahnlr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gfhfkzipw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gfhismugb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gtwpohtps.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/gqafqpeug.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gslfwwfov.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/gpcxfrzxe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gwzbgzzbm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gaipxifgb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gmkqdbnmv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gwnoklbms.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gjmohkgjx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/glomqfrlw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/gouiwipwj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gbgudklyg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gcluhubyg.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/gkgvtwfsc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.tarul.cn/Article/details/gzuwwudcq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gycvapwpa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.yfazqb.com/Article/details/gmjapcthq.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gdqqgonan.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gddhfmeow.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.bbcook.cn/Article/details/gjfknnqym.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/gvnwlqgra.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gttvhjmfp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/gpxiuipls.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/glukvnjke.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gyvjscewr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/ggdqasauq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gnghjmhud.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gnoubfxhv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gicqpxaql.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.tarul.cn/Article/details/gfgounuur.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/glzzmnxxy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guubzuyrx.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gfpentepl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gaomjdzbd.sHtML

[J01] 获取当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gztzgivim.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gssbjtawa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gqubbvxec.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/glhozwrzc.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/ggkvxmket.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gfrbthpyu.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gjjymyhvt.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/gxpjoyqnt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gceflmowi.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gunlwkkaw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/guxkvbwia.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gbkvnwfqs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gfepufbtx.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/glatdpjga.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/grexdbkao.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.vehdjk.com/Article/details/goizxgsmb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gtmfxtjiw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/golpqzfjr.sHtML

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/gxjurlibu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gqpghlheh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.yfazqb.com/Article/details/ggqlcuywg.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gqyanlsox.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gdzcyyjvf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gnaonpqou.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gmlbevoqf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gqocpjpqk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/gaaxftkwb.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.yfazqb.com/Article/details/gzbohxigv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gmzebycqe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gngukrwar.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gdzdfydgb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gaksowjln.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gcqbensnv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/gvzhouzwn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gmkpkicpr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gihsqyxvb.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.sjlbkw.cn/Article/details/gqirzhiid.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.vehdjk.com/Article/details/ghdavvlqt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gmhxxtpxo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gpddgspoh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/ghwigzthn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.sjlbkw.cn/Article/details/ggwizpamy.sHtML


<!-- 参考信息 -->