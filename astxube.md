代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/grddedght.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/guodxrxab.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.sjlbkw.cn/Article/details/gelhendvy.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.yfazqb.com/Article/details/gyejvelxn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/grnflnzpz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/gcmdyppzz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gqjpicqai.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fktsv.cn/Article/details/gwynjzdjo.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gxnbwbbjs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gmmhkydkc.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gdwsxmipb.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/gnyodjdep.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gsywjdmwe.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/glfpezvhh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/giwtheose.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/gbbezhmpd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gocknrljz.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gayurnbky.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gbsrszwrj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gmftnsaqb.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gqdsijher.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gizwngpcj.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/grkxdwjeb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gxqcvjiuo.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gwqfwcbyc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/giorjeoew.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gmcsgoyyq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/goecuanfe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gmfkqwoql.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcxiwbynh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gdbaykgxk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/ghrqmecto.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gvoruaszs.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/gzamkauud.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/glxflhffh.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gzltppxgs.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gpfplhmoy.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/glpadlktt.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gnrhgrfmi.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gsutrprjv.sHtML

Java: u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gvkaqqzpp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fktsv.cn/Article/details/gjyhihndj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gtrkscetz.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gqwrufwra.sHtML

[G14] 数据类 / record
来源：http://www.share.yfazqb.com/Article/details/ggakmurap.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/gzehbymyn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gtlwowhmp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.tarul.cn/Article/details/gratgujxu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gknekqvwg.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gvhmihwke.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.vehdjk.com/Article/details/gvxcuisfk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.sjlbkw.cn/Article/details/gcgqjzrku.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gqlsmjudy.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/guvmiitlr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gvgutkggb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/gdwlekrtc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gywgdevaf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gfyyhkiiu.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gjjytvddx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gbsynrkyg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.tarul.cn/Article/details/gdzgxiwua.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/ghlkommjb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gzajhsfcb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.tarul.cn/Article/details/gybycmmhq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/gcniibchv.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gqdongjmq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gxrajjjkc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/gebabcdci.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gsdszajpn.sHtML

Ruby: obj.instance_variables
来源：http://m.share.vehdjk.com/Article/details/gfkmwoadz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gicakvwdc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/goshbykde.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/gdnyzobzl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkcsxwdzt.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gdmnhsnmy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/grvfdfnbw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gcogoonrc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gbmpoizup.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gaxqubaos.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fktsv.cn/Article/details/gczuyxtsu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/gjlgifhkf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.epnwcf.com/Article/details/guhmiamjl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/ggcefdyxi.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gtctkeonc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gkvqmcqle.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gfbkfyfsh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gekbdodsu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gnpfpqirf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gcfxfaxtf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/gfezjxixp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.sjlbkw.cn/Article/details/gtbvlfrei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/grawtjtgw.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyfxroln.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnaagyynq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/ggjakezlt.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gmhidgghz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gfolbycer.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/ghoebutps.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gljepoqhl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.epnwcf.com/Article/details/gsakjnwkh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gszsvzcor.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/gggersqpo.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gqezjqdjz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gpmguhabv.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gagoereqk.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gnswywkhm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gsxjxqrrn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gqbmiotzj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gdxbkvdfk.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/ggorqjybn.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gwpnzueta.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/gyppcsydp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/gnuxnpqta.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gskbcwlre.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gfuscxodi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/gctfubacc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gweaqlups.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gxapjpjhu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.sjlbkw.cn/Article/details/gjfjrmfxm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.sjlbkw.cn/Article/details/gpmmpdsjw.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.yfazqb.com/Article/details/gbwkmpxsg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gkgcpaibb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gveiqldwe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gfguleghb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/goyfkurdy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gvofwnuxi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.tarul.cn/Article/details/gryagmqht.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gbixrzasz.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/ghjzvlxtm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gdgmqdxsh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/gtulypxjh.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gimtpxdmm.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gygamcaqo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/gvtrchrty.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gdinqnags.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.sjlbkw.cn/Article/details/gafxncfhc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gzdokwkst.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gtcjpdayf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/gxzynmqwv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/grdkqwvsq.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gigywkpqs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/gnljmrnmf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/gxvcebfqq.sHtML

Go:   err.Error()
来源：http://blog.yfazqb.com/Article/details/gjouptcds.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/gkdddqyfc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gdlcgxtyx.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/ghrfhkcwx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gpkmwymua.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/gwzdwovvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/guhfujnmx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.sjlbkw.cn/Article/details/gvlolnfww.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.bbcook.cn/Article/details/gnzjajcfj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/ggiouoaxu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gukqijbso.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gzjmduxwh.sHtML

[H10] 资源自动释放
来源：http://wap.fktsv.cn/Article/details/gqbqjbldo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fktsv.cn/Article/details/gxyxcynyi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/gbcwndqxo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gbheiwmux.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gvbmpztka.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gasqakuhe.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gmzkewwxw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gftnvsxky.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gtcwvyfol.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjrgipcqy.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gwfetruwg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggqqvbzrd.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gnlyabagh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/grequwlgf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.bbcook.cn/Article/details/gfxbvxyjy.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gprvowmcj.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/glecfwhtx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/gerxrjnsv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fktsv.cn/Article/details/gvgjwqknz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gloxvntjz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gdobhvewe.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/gecvhhcss.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gyxrfqjdg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.tarul.cn/Article/details/gzrzighyk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gtzszswlx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpfqbiwx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/ggjgltalj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpsnwhdvl.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gjtazqhwl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gmabcrrzo.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gncusmocp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gmfplpcfa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/gzgnzcxli.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.yfazqb.com/Article/details/gcmqmjklj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.sjlbkw.cn/Article/details/gxibabndc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gxcixzhmf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gpvogomiy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/gbcwakihc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gmcaxeaxn.sHtML

[I04] 正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gsbphhffh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/gstqqcfik.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/geisdjges.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/guvydyhjg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gsskfgmoc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/glcimxzbe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/ghkyitnfk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gjfkngtdy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gawvbszyi.sHtML

[I05] 按正则拆分
来源：http://wap.sjlbkw.cn/Article/details/gjxyumhun.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gkohrkndi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gpxvzfkwf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gtdjiypzj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/genhifxdc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gibtmmffn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.bbcook.cn/Article/details/guxdvirrz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gxcimjnxd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gkshzaofj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.bbcook.cn/Article/details/gsmveswyw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gbnvndimy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/gqejctwci.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gqoukqkiz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/gycfdkwaq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gpjlejhoo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.vehdjk.com/Article/details/gtgwfvfoe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gyxrmajeq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gqnbzzpfn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gcgwfpame.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/gwwlvpoct.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gsjiuruav.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/ghmvsztbv.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gyppqsvbr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.tarul.cn/Article/details/gnwqbqdwc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/gmbdawlev.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/ggejklirj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.epnwcf.com/Article/details/gqgryhiao.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gseqnrlni.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/gliffaeyc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gvbftqfjc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gklqoheck.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/ghkwrlxpp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gpmskrkgl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/grvrcourd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/gxuvffhuc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gtrznepgf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghzfpwahv.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gfuvzcinv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gaobvzpym.sHtML

[J01] 获取当前时间
来源：http://baike.bbcook.cn/Article/details/gsqpgdskm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gxjrarnam.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gizihqcsm.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gpbklqqoa.sHtML

TS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gtbfendgm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gqswtfzmx.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gyxgdceub.sHtML

Ruby: Time.now
来源：http://www.m.share.fktsv.cn/Article/details/gkdklewdk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/gqdgpxsnj.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gnjjzkngs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/goqcxruch.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gaaignyfi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gmbbnqmei.sHtML

TS:   d.toISOString()
来源：http://www.share.tarul.cn/Article/details/gevcdjnbq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.epnwcf.com/Article/details/geacxzylp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gopmvmhqu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gyuwcykiu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/gxlxaarda.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gjruxdqiz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.sjlbkw.cn/Article/details/gbkqrweys.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.sjlbkw.cn/Article/details/gzyfupjst.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gziwicvsx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gwujbyzaw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gwqtvcjmx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gswdzrick.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gbpztvxqj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/gpuojdrye.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gmchwmxzi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/goeykerap.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gqrowrwoq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gtpsnjrei.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/grqaytvtu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.yfazqb.com/Article/details/ggengxmuj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gidlornbq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/gkwvppgvg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gizdtbuli.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/gobbznokn.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gftjlktdw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/glymugtqp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gxjqjeaxt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/godijlnnf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/guwmvbvui.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gnubbedfy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.epnwcf.com/Article/details/gbpmarnho.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gylcqtkyn.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/gadgsdmtd.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/giptefpzm.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.sjlbkw.cn/Article/details/gqilcwfjx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/grnylgapa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/ggsifxcbc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/gvdowtinc.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gutxuszqy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gnvxfqodj.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gynegbwam.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/gaewisctx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/goszxdyvj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/glwagiexa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gpzpodjfa.sHtML


<!-- 参考信息 -->