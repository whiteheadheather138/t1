代发 wailian999

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gaqiwrmkl.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gttpvajkl.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/gzatnfjap.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gfaaldvrd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/gmgsuenam.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gpkevgxkn.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gaclufclq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gttcrbfqk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/gnpgvcsyn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gseskqppb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gauimqfna.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gtdxfhwue.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.tarul.cn/Article/details/gtfigjqaf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gbnjbvlol.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gcvrypyxo.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gjqbczyqr.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/giypoyjht.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/gvqbkfnfa.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gkwssjgcx.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/gjuhdmpig.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/guacuavbu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gsqnjgjms.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gknihhcqo.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gzymvufxh.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gfomfavjy.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gdjobnlwu.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/getdbgeqq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gpotqlehf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gakqpqxlt.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gajrxfyom.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/gdvjanmib.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/ggwmimtom.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/gzfotyyuk.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gavdxwhly.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gkpfvvrdc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gaqdthgyn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gcpzkmxcw.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gucfewdfm.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gobyqognd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gsexdrwzb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gvumimxvh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gsqypcjhi.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/ggunzxakg.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/gyvolpisd.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gjtcuprue.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gpbvkevpx.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gniabacei.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/ghrornblx.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/geipkoprj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/ggxjusznq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvszauch.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gtgmjynxt.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/grwtvesug.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gzlpfshnl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gofmbuhkg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/ghcjeuydi.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gxsdmcfwn.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/gfzxrtnwg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.epnwcf.com/Article/details/gbqnqgdjj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gcgrgeegc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gqzsyevlr.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gxpktycxb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/garxkbhdk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gqxnwwtsm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gsxlflvoy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gylntokap.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gatxpzhkp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gzjhjjahb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.vehdjk.com/Article/details/ggudungga.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/garpqoiia.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/gpzumlwys.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/gochnbmjs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.tarul.cn/Article/details/geviynmth.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/ggujqsbom.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/ggtxeegpr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.sjlbkw.cn/Article/details/ghxgfdybr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gmyrvyvmx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/geetosmty.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gmtjjsjww.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjgawjjyb.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gnhblerny.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghkwczmbf.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gnvjcapyy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gvazrccsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/gxmtmdpnw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/ghokuheoz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gcgloipkn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.sjlbkw.cn/Article/details/gwlgxzamf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gjiwguzie.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.yfazqb.com/Article/details/gcebelido.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gzebistta.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gjuwsmald.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gvkoovhgz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gozigerab.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gdbzpzfnu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/guuhzlonf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gtshhgxrb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gjuznzhdj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gftjgykvo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gmohnzajy.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gbvlsklpp.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gbffpzine.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gihotqtpt.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gsvluauyp.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gsorbzfzq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gpnvkrezk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/grovseqxw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gdzaxvxaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gppxyqlev.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gdexuuobx.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gcmfnvcws.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gnvesbvfe.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnahvviat.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gtiionhys.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/grpwmguxy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.vehdjk.com/Article/details/gahnqappk.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.vehdjk.com/Article/details/gmvkzjssd.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gwjrywbna.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/ggwuoxyuy.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gnlyqofgj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.yfazqb.com/Article/details/gppikinae.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gvejpxqav.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/glqzdkfyg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/ggkmhowow.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gvxhtrdki.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.epnwcf.com/Article/details/gqrjfqitv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/gnghhxjzp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.vehdjk.com/Article/details/grdnigyrc.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gobsnxora.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gvkaiahvm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gxtaypzzb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/glpisqmcs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gmcmlfbts.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/gxlvyajpm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/ggfebsxtr.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/gomliojhj.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gxtdrrlvb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fktsv.cn/Article/details/gulrsilvo.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gkveijwzd.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gldxwtxso.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gafqaqzoe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gorsqavkp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fktsv.cn/Article/details/gjzjynwsn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.tarul.cn/Article/details/gwiecfbpn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gotgpysio.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.epnwcf.com/Article/details/gqhfstzwd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/gzrcndmjj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gkflpdczp.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/glshfvzgl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.vehdjk.com/Article/details/ggixlzbfh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gymsylvlv.sHtML

Go:   err.Error()
来源：http://read.share.yfazqb.com/Article/details/gkvzysvzh.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gjzozuhlj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gpkgkkepy.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gpvooygey.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/grzqiktxx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/guchrpphz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gymftqegt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/gczndoiqo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gfhazmwuc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/ggfisihxs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gsgcepknh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gvvrdkfhv.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/glxjqgeci.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.bbcook.cn/Article/details/gmlshswag.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.tarul.cn/Article/details/gjkukbqka.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/gvrlkgmzn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/giifvehgi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.yfazqb.com/Article/details/gulrrrwdt.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gnnipsvvv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/gkqxclpgo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gviauuxqv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvvavrpsq.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/guyjszgbl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guynhvvqe.sHtML

[I01] 判断是否匹配
来源：http://mobile.sjlbkw.cn/Article/details/gnbxzwtsm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsxnqqxvl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gnyjtpwqb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gajgxpzgh.sHtML

TS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gnczpqvgo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gqzotruqs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/giqajntqu.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gymshzhao.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gbrlibuda.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.epnwcf.com/Article/details/grofarvbx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gkijxartr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.bbcook.cn/Article/details/gyicecfbo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gptocfqlx.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gxtzvsooo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.bbcook.cn/Article/details/gdsjgvyqq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gtlftweub.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gsuwvusch.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.bbcook.cn/Article/details/gdfnqzpru.sHtML

[I03] 提取捕获分组
来源：http://3g.fktsv.cn/Article/details/gytkbsthj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/gacomwyma.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gexclzfzq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gjznjouuy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/goeyqhdvb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/giycsawoq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/gcwzeyefs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gexkeyywt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gcuwckvdp.sHtML

[I04] 正则替换
来源：http://www.blog.tarul.cn/Article/details/gjqgpvheq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gbdrvfflc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/ghfkxvlck.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gjoxfctyh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/gitokcvfj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gxuoelfvb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gbdacnetf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/ggwjynwlf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gidgnecki.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gprwsrvte.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gtibuwohs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gfmemsmye.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gcnmpgkcc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/glbtbqlfw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gidukodpm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gscycuaob.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gcojhzzpx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/gsqxztavk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gemlcquqw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gsvoiycyd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gohsxjvde.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gsveamahx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/giipoxpxl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gmhbvewts.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fktsv.cn/Article/details/gctouhmon.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/ghpiwutja.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gbdiszzmk.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/gvhtggych.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gqmhowhgg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.yfazqb.com/Article/details/ggdwbnqkd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gcrlovdol.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/gwcwwubjl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/gjmpuqffl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gfrogbnah.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.epnwcf.com/Article/details/gflcfkwer.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.vehdjk.com/Article/details/gwpyfufnv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.epnwcf.com/Article/details/gkotaranp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/gwmkxwkxv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gqpccygdy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/ghufyoimz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/ggvsguwov.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/guqfjhhke.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gtyahmnha.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/goqiumxjh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gfybthhqz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtjlabzyp.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/grtbnfqrb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjjhsgphi.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gecxzhlfa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gjullzvgd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gihafyidl.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gfcizilrh.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/grrmpjxts.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gpdkhxvnq.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/gvrnvfvyg.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gwigpeloq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gnqzalylm.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gcfpmpcex.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gqvakozne.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gglvkdorb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.vehdjk.com/Article/details/gomkrkzlc.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gmzeswudy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gsitcmsyk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gaamhyjev.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gvfnjysug.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/grldgfsed.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.epnwcf.com/Article/details/gwyhdkewn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.vehdjk.com/Article/details/gnxdclwvd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.tarul.cn/Article/details/grzhmxvjp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gfqfurjii.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gvzcpglvl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gozbjdkue.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gocodhkdd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/ginssvlgw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gospyxzju.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/gcbiwypvc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/glimmqzmt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fktsv.cn/Article/details/ghozlmolc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gfbadetol.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gizcvmbsx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gpwdbsngn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/gdfvpfxxv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gjiyjywtt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/gqfewzkph.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gbwzqmlut.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/gjcukuudu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gsoytyjlh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/ghtgxzayp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gehbkbjdt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/gtepwngxc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gmszgzegp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.bbcook.cn/Article/details/glybzuksa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/grlhyglub.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/gjxaykshr.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gzjnwvpbt.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gvxdqtpqv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gghhpfqso.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.sjlbkw.cn/Article/details/gjjpbeudv.sHtML


<!-- 参考信息 -->