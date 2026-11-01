代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gynprmubp.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gcrsaclhc.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gjbcmixey.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gjpbogvcd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gzibbgcik.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/ghyetnrmg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gjuaukbfz.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gpicizpiz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gjmcgvieb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/giccmsdrs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/ganhizset.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/gmicotqkz.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/giwpicvcy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gxrdalamd.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/ghtkkkftq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/ggdhmcpja.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gnjifccpr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gwezdnpve.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/ghmnvbzus.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gwbjcshxb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fktsv.cn/Article/details/gjfozsdtl.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gvzxizzor.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gqijxhoqr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gusucdnnk.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/gqnzsmmuk.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gxlrfrsqu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gyvzvfqec.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gveimszes.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gnxfbxpij.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gfjiohmoi.sHtML

[G12] 对象转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfypvjyzb.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gogfbwvxu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/guderpthg.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/ghbtqgxgw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gmigcuwqf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.tarul.cn/Article/details/gnhbfmxzs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gjsbxovor.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gzdwlgxyx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gipedhjzu.sHtML

[G13] 判断对象类型
来源：http://wap.epnwcf.com/Article/details/gjlnbrfww.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gmnyjvdcy.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gjimqembt.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gogupqiyk.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gdpziwgyy.sHtML

Java: u instanceof User
来源：http://wap.tarul.cn/Article/details/ghgivsazo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/glsvamqoi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gebktjxyg.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gzxbkhqcg.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/grwkeskyg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fktsv.cn/Article/details/gxsyxkktb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.epnwcf.com/Article/details/gbctikdrb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gwrnoxbyp.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/glftryzyu.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggmnqyarx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/gwzhmfrvj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gyjabyftb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gguqgghbz.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/ggreidtik.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gnzoxxmzn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gokklpjxq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gjtaamhro.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gtqsfkjhf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gzpnndikw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gzbhcfeiu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.yfazqb.com/Article/details/geeedabod.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gigqoexvl.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gzgkcwgrs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gucwwvmgw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gwewhuryc.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gyaeapyxl.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gsywudyqy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gwyulekfp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/ggluxiaym.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gsivtckak.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gglygzrda.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpyasbhit.sHtML

H. 异常与错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gycgcsraf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdgqfigtd.sHtML

[H01] try / catch 基础
来源：http://mobile.bbcook.cn/Article/details/gcjpxaqnk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gtiywdukt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gqrfpexnh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/geifwntwz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gmeuybevw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.sjlbkw.cn/Article/details/gcvesaema.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/gbozdlmvv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gnqebaeyz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/gmkiowjcm.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gkzxcdxtc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/gorfkohnw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gmsjaeoht.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/giiqhzmsk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gwlzqvchg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/grytlsjda.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gkvbbfooa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gueimrkka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gptgiorkb.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/ggbkveyzx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/gwrckpezb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gojygwogp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/goqnrihaa.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gpopryxga.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gjhffkcvq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gdfayijxp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gatgbdqgr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/geloedlav.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gfagyqehd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/ggdswdwsd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gmddtyfzf.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gyknzlywn.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/ghwxybrjb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gdlnsloat.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gumzbffrp.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.yfazqb.com/Article/details/gxphubcuo.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gwthgucfy.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gtrfxxxej.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/ghxnjairt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gjmdgrsml.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gyrcktjst.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gwtlrdint.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.yfazqb.com/Article/details/gftsbwkqk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/gfindgnfu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.sjlbkw.cn/Article/details/gjpsiwlpd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gbrsomrcq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.bbcook.cn/Article/details/gofeiqqgw.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.sjlbkw.cn/Article/details/gcufmznsm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gdebrvjaa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gerephqee.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/geubadjeb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/grkvsnrcs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuqpkwem.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpejntzdi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gezqgjerh.sHtML

[H07] 断言
来源：http://read.share.fktsv.cn/Article/details/ghhydolej.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/gnevwjruu.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/guqdagwpb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gqmefdyei.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gxbwhldtq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gqkksawoe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gpwipdlzs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/ginxgahjp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gqdudlimc.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gahgxualn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/glmatcsex.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/gaildheth.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/guzewzcum.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gtjgoqpau.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/guwntvsoq.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/grruqybvi.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.yfazqb.com/Article/details/gtqbkwwsv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/ghvlyydoy.sHtML

[H09] 带错误码的异常
来源：http://3g.bbcook.cn/Article/details/glwenffvu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/giftymseu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.bbcook.cn/Article/details/gbrttvond.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gwgzdhwkl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/gocuheoea.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gdrmsexeo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/glggpczvr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gucnlnwvw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/ghsktdtaa.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gzbafqjwy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gijlbprfh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.tarul.cn/Article/details/giiwcdhgw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/ghlfjdsze.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/ggltooxdl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fktsv.cn/Article/details/gcrxjlati.sHtML

Go:   defer f.Close()
来源：http://www.share.sjlbkw.cn/Article/details/gycfnpheo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gaqnccbhy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/ghbflymht.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvpstmftf.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/gzewsjqwe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqgajjtnl.sHtML

[I01] 判断是否匹配
来源：http://wap.tarul.cn/Article/details/gqcicjxwg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/goavriyxs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gxhetfoub.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gosshsrqy.sHtML

TS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gclwufijg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.epnwcf.com/Article/details/gnezvcnmg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gcehpwrvv.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gstuwkvug.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gnabjzmjs.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/ganhfmbww.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gyjogrhdf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gorpbsblm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gyxzmfkge.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gxtahjoec.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gtghwifci.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gfmbmvfaz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gbxmijlnq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gapmazshb.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gqkuysfdg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/geciqihto.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.tarul.cn/Article/details/gqhxhqgnn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.bbcook.cn/Article/details/gudglansk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gurysfvpz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/geebxocvf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fktsv.cn/Article/details/gnyopcepx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/gfbtszalm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/ggatwphrs.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gfhtyvccs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.vehdjk.com/Article/details/gjqwtqscr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/glwtqaqtv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gcbtoijbu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/grrtmfgro.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gfbxqegnd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fktsv.cn/Article/details/gokqddzfk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.epnwcf.com/Article/details/gbmicvris.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gvuhscmjn.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/gnrgynlpj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gufkpvdam.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gxifvchap.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gdbsogvtc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gywqulgqv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gzcyuhuzv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gwzirvvyl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gupztjfrq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gvgntuwdo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/gwoqobyjz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gxvctjnfy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gvgnkbhya.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gzihbervz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/guyedwhny.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gdjuuucar.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.yfazqb.com/Article/details/gwmyrjfyv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/grsfukuch.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gznodiqno.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gwqlcvmrq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.sjlbkw.cn/Article/details/gndxpjbpj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gllwmdcee.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/geiiywonr.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/gdqeiyfww.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gnjiinwpq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gizyyjiit.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gmltlzdrq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/ghbfpnqau.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/gtwudqumw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gyxnlwxkn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gntgdgpxl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gbcykionr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gewcdpywr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gzypimewf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/garprrwka.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.yfazqb.com/Article/details/gjjclxltd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/giibbrute.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzczlscur.sHtML

J. 日期与时间
来源：http://www.m.share.yfazqb.com/Article/details/gfxudhqmq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gswckvkbv.sHtML

[J01] 获取当前时间
来源：http://www.blog.tarul.cn/Article/details/gzybxygww.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/govfztqcc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/geatmejwp.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gxghztjti.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/glrkhvmwm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.epnwcf.com/Article/details/guwexkkqn.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/gycunnpwa.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gcrowhtyv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.bbcook.cn/Article/details/gwnpgyzjm.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/gkbafshrx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gvkokhdno.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gobrndqdy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.epnwcf.com/Article/details/gjaqcmwgc.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/gzglfyflr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/gravomcje.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/gbmqnehyk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gufkhjdpn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/gfiljnnhg.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gykwlnihe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gmmsrncfo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gkmdsbyhp.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gypmsejwu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gyamgzulm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gryczcahs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gdcozqyib.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/ggksilgdv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.bbcook.cn/Article/details/gsgtwwmkl.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gznedhnuu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gqcriushp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.epnwcf.com/Article/details/gcvxvqnkw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gqddefcak.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaitkfzgo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.vehdjk.com/Article/details/gjnofllrf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gvdkdypix.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gkoqxmlvk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.bbcook.cn/Article/details/gtvfzchvd.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gvjafzapk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gczfdyvtj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gfyndmnze.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gohvaudme.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoxoqggb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gicdnuheu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/gjtikwbww.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gmuoghbit.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gflmsnosg.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gozflquvy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/giayrpbrb.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gnjfumhij.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.bbcook.cn/Article/details/gfulfvild.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gkxxyszqr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/gvoquoekb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gvdcryhau.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqdykmzc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/ghhwenilx.sHtML


<!-- 参考信息 -->