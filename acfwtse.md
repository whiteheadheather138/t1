代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/gayjddcga.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gcthdfblb.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/gowmkdjpf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gloaqbiwq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gwhbwjdfl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gpazctqke.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gkligjbdv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gyblpvsou.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gaulyilcm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gpedplxla.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gaizacpiu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/grnwhohyk.sHtML

[G10] 访问控制
来源：http://wap.epnwcf.com/Article/details/gffcicwvw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gqtnqnwxp.sHtML

PHP:  public / protected / private
来源：http://baike.bbcook.cn/Article/details/gaqpmevvc.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gbtfwzoxz.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/gbbwgkdiy.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gxfhbdkkc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gjaojxomq.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gcfyrdfci.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/gsqewdliu.sHtML

[G11] getter / setter
来源：http://www.share.bbcook.cn/Article/details/gjmxtnxap.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gvcxaskvb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gdehwvlqd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/giypqhrmf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/giwgylxpv.sHtML

Java: public String getName() { return name; }
来源：http://blog.tarul.cn/Article/details/gsdyhqjrh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/ggdevyzbj.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gkwejtvcy.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.vehdjk.com/Article/details/gpyleyyoo.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/gomluammu.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gfcynyuex.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gpzelrpep.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gmsiownys.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gbpxfwbep.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gmagmiovt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gbvyvmted.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gohlvxlku.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gmfexlkxy.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gttjnirzc.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsozlmxyd.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gkamcbpgs.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/glcuzzkco.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gtvodcjin.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gvxilsrpr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gmsgwonhi.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/gokicjgok.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gjnwrjvse.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gqidbcgjw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/glfjrgfcg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gspephitg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gylxiztpx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/gifvqxirf.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.epnwcf.com/Article/details/gektkpkxk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gbwoubnxb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gphedaoqe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/guafugges.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gzmpbvfar.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gdxlryxoj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gmhqplvum.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/grizsvxhm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/ggmbbzmuj.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/geikvstmf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gjiovysfd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gwwxkdeho.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gnjudrzhw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gqjasuzte.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gqlazfmjj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gkqwakeer.sHtML

JS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gzcpkkuko.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/glhjcmnox.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gbfffvudq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gezvvjgjs.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gaztqkkjm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gsjaehwra.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gckeigehn.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/grxvdsmso.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkfqljlnu.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gmetjizeh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gvewywuow.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gncgghfif.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtilwoff.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gvwdkpchv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/giamigwvh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gfrpvqxmx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gtpspbqav.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/ggtaxvdll.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/gwgncigsc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.epnwcf.com/Article/details/gdgumdutp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gzfbvhfil.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfwzfpvex.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gzwwqrhwh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/ghcejtvfn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gbeakwynx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gtaopzptr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gacppgfqm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gyadahzzo.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gggjwnhda.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gijqygfvr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gdrpajypl.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gquiiddgq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gdnrehtfv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fktsv.cn/Article/details/gtaffuqkm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/gjchryash.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gwpfcqeqw.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/ginuismxq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gbqqmdtxv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gqztdtmai.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/golhoifzt.sHtML

TS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gaxixithh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gvwerdvgh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/ghwgkaqrn.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/ghqyildcb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/gyvvxbhle.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/ggznimzer.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gdxaoxvfd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gjrferyjh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gcdetxslt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gcvazxota.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gmoifrtqt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gnuyfqfqd.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/garkflmku.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gxdyzgisx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.bbcook.cn/Article/details/ghnnswnwe.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gjnknbqsc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gyqcemdxw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gnelclell.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gfflxpxdq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gtvwkndwv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gwozfhpqk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gnnsjicbw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gvdpolhce.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gorgouqmy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/glpeibdwd.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gpfyhqegt.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gjhhuwzwg.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gzlbkbhgs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/gtbofqivi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gsovqyqut.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gaayjwdhh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gsjtcfsrr.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gopzllmuy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.bbcook.cn/Article/details/gcckzcqte.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.vehdjk.com/Article/details/gwfgjqkpu.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gyimndvux.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/gyjayitsk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fktsv.cn/Article/details/gixtpfrrl.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gtkvsphdf.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.yfazqb.com/Article/details/gwkruktex.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/gywkvldmz.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/gfkfhbitt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gzdrvegju.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/ggbtrivvz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gedaaejll.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gqrygmywl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fktsv.cn/Article/details/ggflaxyyb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/gcpmidekr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/goeqnuwne.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.epnwcf.com/Article/details/gcmkkiena.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/goxnmerjd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/gfecuozxr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.yfazqb.com/Article/details/gniuhdyqg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gzppwpgfq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/grzclbqqz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gboqaqijm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.epnwcf.com/Article/details/gkppnpvmr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/gqxbpkbun.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/grjdjfvmj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghgkvzcxd.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gfzroojpw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwuqzsrpd.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/gpxsdrrdf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gxvpwvtbe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gubeqnopw.sHtML

JS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/glvrbajvw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gkznaxiek.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/gyyetzlsh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.vehdjk.com/Article/details/gowxbigqr.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gvysztkta.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gglylrhap.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/gqddyexsq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/grulmhdha.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gftvakbly.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gvqfyvulp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/ghfqhbkpg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.vehdjk.com/Article/details/gnlpxfntf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gmukclezn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gnbsrzaxb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gmrjhzhgy.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/ghfijdcea.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/gxpsijulw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/ghcesbkev.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gtioxgkbx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.epnwcf.com/Article/details/ghaugkekd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/gdwzdbvad.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.vehdjk.com/Article/details/gjzplcdft.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fktsv.cn/Article/details/gksioyhsi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.epnwcf.com/Article/details/glbkfhaoy.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/gzwlaezxt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/gybduufjc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gtsqwubzy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gankcalui.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/ggwzgjpdf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gqzegazsp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gluczwhyl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gddgovsjy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gvyudxhee.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gnrfmqfhq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.sjlbkw.cn/Article/details/gvohvvoip.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fktsv.cn/Article/details/glsjpjthk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gastzsjpt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gmhihdwbv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/ghhdgmoxl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gtgmuzuzo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gepkchdlg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/ggybpznvm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.sjlbkw.cn/Article/details/gdqqvctyz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gjfmkyrcw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.epnwcf.com/Article/details/ghgebjxcl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/ggfjoksom.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gjxnwblyw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gcdgxemjs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.yfazqb.com/Article/details/gaaoddrvy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.vehdjk.com/Article/details/gbqwsvkqd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gsbdpbwjp.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/gvfxlrhyq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gvzlufvrq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gjicjmstx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gkcfejjig.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/geqluzqbm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/geqhzoeft.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsibhifiy.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.yfazqb.com/Article/details/gviuigpcp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.epnwcf.com/Article/details/gizhwuuab.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/gnsjrqtqf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/geovyzxht.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gljctcdyf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gfnqbckvj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gdjqbduyk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gwzssjghw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/giornsozi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gnjsjinkb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gnyerecan.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvvsaonqy.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gtzoxohjg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqyqswext.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/gnemekhum.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fktsv.cn/Article/details/gnlnipoca.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gfbtefvrs.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gmqyexeui.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/grtbxzpgg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwchnmxh.sHtML

Go:   time.Now()
来源：http://wap.sjlbkw.cn/Article/details/giwwvkwsl.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/gvvkggebf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/genvccafg.sHtML

[J02] 格式化输出
来源：http://baike.vehdjk.com/Article/details/gawjaboxd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gcoexxmkm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/ggwzwomti.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/gqdioopgj.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/govouwvmg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.sjlbkw.cn/Article/details/gtaewukuv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/gvesrahlt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/ginncgpoj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gsgciiuoh.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/ghdsxagtu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/ggxydugmt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/gbiawndam.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/glylfijws.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gjaqqahat.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gixbpjgek.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gikafbaek.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gouhsrwbu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/glkhdzozd.sHtML

[J04] 时间戳与日期互转
来源：http://wap.yfazqb.com/Article/details/gotaageab.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/glxrpuymf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.epnwcf.com/Article/details/gaeyjjgnk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/guhqstydm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/gbvqpfsbw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fktsv.cn/Article/details/gprxuajuo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gmfhrsifh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fktsv.cn/Article/details/gywzoxlub.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/gjhkwpdlo.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/gtuyjtbda.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/gkfclyfle.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gjucmhdlh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gozkgtdly.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gbmijlagz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gsaldzxpq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.yfazqb.com/Article/details/gumvrpjgx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gfpugwcbp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/gkuavukkl.sHtML

[J06] 计算两时间之差
来源：http://www.blog.bbcook.cn/Article/details/gwfnensyd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.epnwcf.com/Article/details/gvzlmjskh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/grmddjawg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fktsv.cn/Article/details/gncewkrcw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/grpsbowop.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gnrjrvgef.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/gajeumdkp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fktsv.cn/Article/details/gdumnlfkt.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gmwhwahey.sHtML


<!-- 参考信息 -->