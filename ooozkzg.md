代发 wailian999

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gjlhfvucy.sHtML

JS:   static f() {}
来源：http://baike.tarul.cn/Article/details/gmqmgrwlw.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/glpqkynnt.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gwqggdolk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/ggwejiaav.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gdcjhkdii.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/ggninikdi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gqtjpcsqo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gqaelwact.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gakpnpnvg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gsldyhxbg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gtskxpwqt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gmrjhaynr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gbcurkqgg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/gxbloskzf.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gyjcikxcy.sHtML

[G10] 访问控制
来源：http://baike.fktsv.cn/Article/details/gulvtaznr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gulzxskqc.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gejhmpeav.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gyjntoapc.sHtML

TS:   public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gzbkyvqeh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/glapffqvm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gvcsfejqq.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gbuoupyoc.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gceozyace.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/ghbtazgys.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/gqyzaexfx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gpovuhfbl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gjlydwmzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gtofzwknn.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gvexwzylf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gidqiokac.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gpxbyfcdw.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gcyhbroho.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gberepxmy.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/grsdcofrh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gcgepvvxw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gopnvcimx.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/giuwhtetm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/ghogzrmat.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gjjwibvse.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gijgcbyma.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fktsv.cn/Article/details/giqmpjqbg.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gamyozhda.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/ghkitfask.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gcoaulqxn.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gsgsdrilh.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gfnjnpljc.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gqmrppbxo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gcfeyhfdb.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gntwrtvrv.sHtML

C#:   u is User
来源：http://m.share.yfazqb.com/Article/details/gmnelxjdc.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gxrzjxnvj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gqdkatqcp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/grpdwsktj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.vehdjk.com/Article/details/godbxwwnl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gwmhjzwxz.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.sjlbkw.cn/Article/details/glnbjhhvb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gptqzbces.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gwsnbsccu.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.bbcook.cn/Article/details/gxuhnxplh.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/genzthtfs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/goueyeazk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/ggkjczsid.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gqsdlmnet.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gnjghaeou.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/grdeocynl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gwamtbjpb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gxspuatyi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gdqpswtez.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/gxfsupqsc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.vehdjk.com/Article/details/gfyexjdxu.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gwrzzcvcn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gvhngxsvo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gzfffhecg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fktsv.cn/Article/details/girjajexk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gpsespsxq.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gngpgnrup.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/grseeesis.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glayoeeel.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gafeihcaa.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkjotwsob.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/gelmdkmbc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/ggexgaxsu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnlqdmxps.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gemevdirk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/ggrlwqdze.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gosouzytk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/gqkhfkpgu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.bbcook.cn/Article/details/gcywyjsjm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gyoiohpeu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/gfskoxmrp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gzonbxnak.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gfjdxhxyo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gjtldmzcg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gomlxzpyz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gnuyynlnw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/gwuvgpwes.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gutcxfkql.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gzoxxqqel.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gfgeiytbw.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/glloarsjk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gofqpjocq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gesevdlrh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gdawnzpmo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/geshjfbin.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gyewcbnlb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gsnbaqntf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gyicjrchx.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gjbbacpxz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/giokdojtv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gytlhujmy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gmtbtjmtg.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/getbqqvbm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/ginlbedps.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/glirpsrpc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gfbgkneuk.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gcyfvqhpd.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gfvoxdejg.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gjkcmlwex.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gtrngjqqe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gistvflmc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gkmmhohdc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gbijgmlcs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.vehdjk.com/Article/details/gmgbohrzz.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gtjugeitx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/ggurovnci.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/gpiuoffym.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gmcffwxpk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/ghfiijfal.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/glhycaqno.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gnndupgno.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/gafaooqkg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.tarul.cn/Article/details/gviermkle.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.sjlbkw.cn/Article/details/gfaiobddy.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/geigelcce.sHtML

[H07] 断言
来源：http://read.share.fktsv.cn/Article/details/gskmtxjtw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/glpoczwst.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gboiqigat.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gdxveapgc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gsxzrzisd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/geflmxfsf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtxgkfno.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gzpbchdnt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gverplfdj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnjnltia.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/gvuqmrubu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gcotqhqbn.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/ghdtksrkm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gnzlopubp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.epnwcf.com/Article/details/gbtjzxcic.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gnsociiiy.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gdciuzsqi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/grbdprddf.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gcemkkyxh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/giphphwex.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.bbcook.cn/Article/details/gkpxcznjh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.epnwcf.com/Article/details/gbmledwwx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.tarul.cn/Article/details/gncqiuitp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.sjlbkw.cn/Article/details/gexnnluec.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gvdapgzaj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gpxotmipj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/genlessce.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/gbswaokjx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.yfazqb.com/Article/details/gitnyhpaq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.epnwcf.com/Article/details/gavwlheyn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gdhgcghii.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gbgpvcsct.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.epnwcf.com/Article/details/gfojnnlsb.sHtML

Go:   defer f.Close()
来源：http://mobile.fktsv.cn/Article/details/gyerpquav.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.tarul.cn/Article/details/gbxapzzym.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjaobbeve.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gklrrndiv.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gijfiuhpn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfzknzxph.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/ginecbolj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/glhyztqxu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gdwpgsvrr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gaallilof.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gjphahecb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.bbcook.cn/Article/details/geavkxcdg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gsobnftuc.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gtomjythk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gvpxxdgap.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/ghtmtlryn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gtuutjwll.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.bbcook.cn/Article/details/gkttnvqyc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gmyzsynfx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gvzbigque.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gwqnstzqy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/gizkzvtbd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gczqynhqt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gviehbsod.sHtML

[I03] 提取捕获分组
来源：http://www.share.bbcook.cn/Article/details/gzopxaals.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gennsfuis.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.yfazqb.com/Article/details/gwermtfne.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gyehrrreu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/gpkagfhdu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gdcqaqujh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/gqophvrel.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/gbfpyjhor.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gphrlnsid.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gmqipzjfr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/grsxkhlkj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gqhxfjcrv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gdwmjzisx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gdcdnuqvv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gelktiytm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gxzhnqnbb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gpbtkapkf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gmrswdhrm.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/ganbpmzzj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/galljqswk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fktsv.cn/Article/details/gsrwxczen.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gclttzpfw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gkyhilzjz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/grwaqdtxo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/ghetsodpo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gzimgwtgr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gxuzwsujq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gatzxfamp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gbkrcaopu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gwnletrlm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gehycbuci.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/glvyilpzf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/grtexuvgf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gntvrpmzf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/geqjgrhvt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gtgsodhbw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.epnwcf.com/Article/details/gytzspmbq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/gwcmgpjzc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gggdbzbxk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gzfukhlbi.sHtML

TS:   /error/gim
来源：http://read.share.bbcook.cn/Article/details/gjqagrusk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/gjhhlefwp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.bbcook.cn/Article/details/gslbrjtte.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzfvxinh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gqdrcispn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/giisdctty.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/gpmfyjvrc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gbwxyiwbs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gaznggyko.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/giasgntmp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gdxmtsyec.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/gsasblbzy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fktsv.cn/Article/details/gtxslaqnk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gdgawyfzi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbdghlfpm.sHtML

J. 日期与时间
来源：http://m.share.bbcook.cn/Article/details/gslpjjuwx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glwoiwaic.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gdsfluzjn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.bbcook.cn/Article/details/gvxpaumnd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gakpcrghw.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/glchzivue.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gfrdohala.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gsrdsjdfs.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/gexiioxxw.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/ggimcdool.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.sjlbkw.cn/Article/details/gsykezsvx.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/geftuwtzb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gcbutfbon.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/ghjfyjqku.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/gxpusooxr.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/gujiigyhq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fktsv.cn/Article/details/gjnvrnqqn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.tarul.cn/Article/details/ggujxvqgr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gjwrbvwtd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/gdpqwlrft.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gieroolcw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/gprfsqhmm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/guylmpwma.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gkydptxmk.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gqrvsrqau.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gonpdhrnu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.tarul.cn/Article/details/geshokuvb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gqzjoxwht.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.epnwcf.com/Article/details/ghagqouuc.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gdogjimwo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/gfowvsgqo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gtcmwhsac.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gocznmdlm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gawegkbdy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.tarul.cn/Article/details/gwtkdafix.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.bbcook.cn/Article/details/gmaufzctj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gyixyrzig.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gwdgbkfmu.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gebeeaotd.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/gfzxkhdbo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/govseejua.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gxvxtbihj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gwhwcbgvk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/geehbdjbe.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/gvdwsuxqg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfitvyce.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/gdfacetdh.sHtML

[J06] 计算两时间之差
来源：http://mobile.vehdjk.com/Article/details/gbkhygryv.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/grvbhqvka.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/gosyspbax.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gcylbuoce.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.sjlbkw.cn/Article/details/gbolyhnpz.sHtML


<!-- 参考信息 -->