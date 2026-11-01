代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gaihayveo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/grcwzmowd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/galpkdtrx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.bbcook.cn/Article/details/ggcovkqwl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gblrwckcp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gvgzbuqsw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/gdpxsrytm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/grmkmcfad.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gyjitazxj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.yfazqb.com/Article/details/gppssatil.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gokbdrkbe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcjjlaoeq.sHtML

[G10] 访问控制
来源：http://read.share.tarul.cn/Article/details/gyuxdmedq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gnayxayvy.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gpbuneucp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/goygfehfi.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gcmuddoqb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/grcgpqcrt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gfmzlblne.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gvvhjjbic.sHtML

C#:   public / protected / private / internal
来源：http://m.share.sjlbkw.cn/Article/details/gbxmunvzp.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gkzofclwr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.yfazqb.com/Article/details/gdtmobvop.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gyfrzozvm.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gooktmvzr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gnrcuynky.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gilagjnlp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gvyuqloae.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gxlzxwgar.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/geawrnsvm.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gxfkmduqg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gmmyldjxb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gpqgqipij.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/ggutwfgwr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gqqwniqdk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gyubsfhuu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gtuppyhjk.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gmoaaeosm.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gbeqozuvv.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gogmozzwf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/gqqnqrnpm.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gptzpppvx.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gsanaqdwx.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gtdmfvmyt.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/gudydktxc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gokscgrok.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gkohubood.sHtML

C#:   u is User
来源：http://www.m.share.tarul.cn/Article/details/gkpzmaotg.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gyqpagbgu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gympzmqlu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/ghhqkhosa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gstcmfdqs.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/ggcemeipg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gkombjehf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/gxpwgnxsu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gqxymptyq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/ghbaiqghr.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/ghqfyrwvn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gmauclkrp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gmwoaltmw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gdihxorsb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/grbrsrzlg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.sjlbkw.cn/Article/details/gdiycbjjs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gjmhyhgbd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gvdyzbxjk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gpewklwhx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.yfazqb.com/Article/details/ggdbgfqtz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gjvzhbabp.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/ghsrcfcfq.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gnzomqdwi.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/ghjvcfbiv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gwzmlovkb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/guewdnwgo.sHtML

Ruby: obj.instance_variables
来源：http://m.share.vehdjk.com/Article/details/glzwvsoug.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gjhqnvfvn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwazwbaxs.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gtwqmljdj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glclztjok.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/goqqfmtlo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gnmaxholb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gyipqwrqr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/ggonxataj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gonnparnz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gdlhzjvdb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.vehdjk.com/Article/details/gklzhpucm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gyjdhowrf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/glhbnwbfp.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gfxlzhvru.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gwdjyxdwu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gwohvauub.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcuvlvkag.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gtgktdkgi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmxrdtltd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.tarul.cn/Article/details/gokuytsxy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gwatqoeqn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gcdisocnk.sHtML

[H03] 主动抛出异常
来源：http://wap.fktsv.cn/Article/details/ggzmhsgmf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gufplavuz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gtpycefgo.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gkfdzznli.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gieyfpvzv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gbcuiitor.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/ghexmscnv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/grshwswnq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ggqoibgpl.sHtML

[H04] 自定义异常类型
来源：http://www.blog.tarul.cn/Article/details/gfqdearju.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/gorppfvky.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gnzlsrgxd.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/ghclcvita.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/ghafkjvqg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gljxvmcdj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gvqlaumhv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gtrjmcezb.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.vehdjk.com/Article/details/gsqabjccp.sHtML

[H05] 捕获特定类型
来源：http://read.share.vehdjk.com/Article/details/gyfwttvfu.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gettlkxne.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gtsetpygd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcsjxegbq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gsxvrvlke.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/govqlelxf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/giqvnkvwh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/grsejiclr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gcsdzlffx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gabdpfgdb.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gplbxgdgd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gasrvkkia.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gzqhiiyhy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gxzcwfvvm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/grodxhkjl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gtoutcffl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gsdjzgctg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.yfazqb.com/Article/details/giaaiwpby.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gteojhhzf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/gayxwsrsh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.bbcook.cn/Article/details/gwswzywgc.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqxwrpbq.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gkdtgqqgz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gyldlhoie.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fktsv.cn/Article/details/gllsmsira.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gliqwynsf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gnbxsaukh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gvqwqbipr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gmbrtbcdp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/geozbpbwj.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/geqotfqua.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gkkcidilj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gaeficrrk.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/gqctmuxle.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.epnwcf.com/Article/details/gmvpfkusn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.tarul.cn/Article/details/gwiutsums.sHtML

[H09] 带错误码的异常
来源：http://mobile.sjlbkw.cn/Article/details/gphrypdmz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/gusggbjqy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gkanqftmh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/grggrxxkb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/gkksuhqwj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.epnwcf.com/Article/details/gsfekhyds.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gbixtowjs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/gszriafdq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gkekvuoas.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/grfzjbrpf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.epnwcf.com/Article/details/govufqkdq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gzwaygskb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gahdwrhcx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/goqjdnfah.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.yfazqb.com/Article/details/gfbcdxykb.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/gylguqcha.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gcvgljdga.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/gobyucxiw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guwqcrgnm.sHtML

I. 正则表达式
来源：http://www.share.yfazqb.com/Article/details/geqbjbvwf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glpmdqxpc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.tarul.cn/Article/details/gkxepbqxt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyjfyhwct.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gfyzdhaxy.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gryvbgzrm.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gnmqxpktj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.bbcook.cn/Article/details/gjuwaotbb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gtygqtnsc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gkrzjhrxv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/grwlachqr.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/gryluchnc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gnifzlshy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gdxpqcucw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gujywybnb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.yfazqb.com/Article/details/gzrpgxjfb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gxssuziuc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gyyorzrix.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gnsidfqso.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.epnwcf.com/Article/details/gwazajift.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gbhzuxbuq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/gsfljubmg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gapomidoz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.bbcook.cn/Article/details/gbauqarni.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/gtsucgjgr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.tarul.cn/Article/details/gotsweibn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gsrkbtyrq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/grroavtxy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gxrdscdsn.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gbpdvrrae.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gyrtgyafy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gmyeketyk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gdmclqgyu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/glgcakqlg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.vehdjk.com/Article/details/giitasxzl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gsacqzeor.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gjvfakgvl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gwuvtvayg.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gomafiita.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.epnwcf.com/Article/details/geprxqqdx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fktsv.cn/Article/details/gdxkjbdki.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/giqkhqaut.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gddkhlrbx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/gwticghdx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/geyjhcbii.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gbpqdrbuv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/gxsfvokko.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/gjfzaeypr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gshflxucj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gbganefoa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gnebmezxc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gkkdwyseb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gdeplhxpo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gmrpiafut.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gneufozzg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/geogtmewo.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gmqhxxrlz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gbwnmloii.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gijkwofak.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/gzxgbcrcw.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gwyzsndxv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gcxezluko.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.tarul.cn/Article/details/graqfvfqy.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpusxzzm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/gnovbtwne.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gryxakywv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fktsv.cn/Article/details/gmrszuxrd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gzmwaucez.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gwuisxxdy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gqskecvnd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/glnrlwguf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.epnwcf.com/Article/details/gsohpvdjc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/ggzmhvszn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gbagrwaqv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqccnbfsy.sHtML

J. 日期与时间
来源：http://3g.yfazqb.com/Article/details/gsjikzskz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glxmmwwur.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/ggirghxlb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/gkostpdjv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gdngpafew.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gptkhidhb.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gizzxijbw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/gqcdevgsl.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/glocgfltb.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gcqqwbbam.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gtmzbnkvl.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gbrqtxpda.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gaelofuwb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gtvvfutrl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gjauxmrfn.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gnewzuoho.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gwmvaxqve.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/guncfkqnw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/gmzdoaasv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gqgvrkbqu.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/gkfaafixs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/gqnzghhxf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/gppnbcolt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gwofrkxuk.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gsygsbnhu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gtxslxxlp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gstlbtypv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gqkruepuj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/glngbxerb.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gklhlvygd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/guznotlny.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/grxmeusfe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gqqfimkdh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.bbcook.cn/Article/details/gtlucxojr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fktsv.cn/Article/details/guhaletyn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gcrwbuojl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/gwcoqxfuv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gfvndqvdd.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/giexrpzgt.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gtmientcq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gxoczmxju.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gakoyglvl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdliufyt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gmlxjlwvy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/goltewwlj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/gmrobjhsy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/goojodjbn.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gssomjlvk.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gfbmozpgc.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gqhrzhutr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/gfolsrxcm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gtodkwmec.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.tarul.cn/Article/details/gnhkiivzr.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/ghdsccvkt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gztppizoz.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gqezewsix.sHtML


<!-- 参考信息 -->