代发 wailian999

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/giugkmygs.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/gjmiptnfh.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/gpgbihwme.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gzbwhfpzl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gzzxxhzbk.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gaawbmmda.sHtML

C#:   public static void F() {}
来源：http://3g.vehdjk.com/Article/details/gwyahedvw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gbwpofuwy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gxqpojxdb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gybdubvho.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/gltszfamo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/ggibtzjgm.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.tarul.cn/Article/details/gemciigbf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/ggmlcphzk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gzrmbnwlf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gawibxbve.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gizaqbqed.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gbmmqrcjk.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gakrrfsmy.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gjhyqzyxo.sHtML

TS:   public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gidgmkhws.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.yfazqb.com/Article/details/gabtvhxqw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/ggvyefdhm.sHtML

Ruby: public / protected / private
来源：http://m.share.tarul.cn/Article/details/gdguyarol.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gsfkrawpi.sHtML

[G11] getter / setter
来源：http://www.share.bbcook.cn/Article/details/gqatvejfd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gjsmpiqnk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/ghygtuwql.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzrddoqj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gmusevvaq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gdylkmuhn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gyubykpqu.sHtML

Ruby: attr_accessor :name
来源：http://wap.fktsv.cn/Article/details/gadhisnih.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gdtaxbgez.sHtML

[G12] 对象转字符串
来源：http://wap.tarul.cn/Article/details/gryeykziv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gybwmdcik.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gunripiqv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gnzpdcluq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gtbsjaqfu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gstnstmtq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gmylwlxcl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gckxxpklt.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/gyrlgcnpx.sHtML

[G13] 判断对象类型
来源：http://m.share.epnwcf.com/Article/details/gvzsivybc.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/gcosnyieh.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gyvcgvwyk.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gvrsdwcqf.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gadymafsd.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/ggvpaxkru.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gcebaztge.sHtML

Ruby: u.is_a?(User)
来源：http://3g.vehdjk.com/Article/details/gchrrltsy.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gzldbtlty.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gvozxksrf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/gdnbfperw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gmafuzyyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.vehdjk.com/Article/details/gdnwvwzjs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/goqzymmkw.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gkcxsftwv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/gorkvswvs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gjwrtoads.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gjqfevhuz.sHtML

[G15] 枚举
来源：http://m.share.tarul.cn/Article/details/gdcblopjb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/gbkdbonio.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/ghioblbua.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/gobvngsdd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gdjligpuu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gprgicbst.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gskfizmhw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/gqrbwwfbr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gedxbnovj.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gyzlxjwxt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/givjedtyr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gojibaowq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gwiloyawm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gstpidwbo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/ggpxvhkug.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gatzecpnb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gkybbqpht.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/grbhdbrky.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqufwrmsc.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gofszairo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyxfrtkea.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gtmgbyxnl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gnuqnwkut.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gbaifeajl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gyozzkeps.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpqwoizq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.epnwcf.com/Article/details/gswdvoevg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/gvwovscfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gufpttaor.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gbqctpqzz.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gkxeemszx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/gjbkezlru.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gmilqdtys.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/guhddbnmb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/giqemlsms.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gnxrsmdlg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/ghlkwxtdo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.yfazqb.com/Article/details/grunawfhq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gdctptcad.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/govluzzfv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.bbcook.cn/Article/details/gvoremkbn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gaznoqgav.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gaydstxqo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/glwrzwxch.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gzkcempxf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gipwdmhoj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.bbcook.cn/Article/details/gblylkvoh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gtfmhybhx.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/gbxruldcd.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gvzkrjvhv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gqkpnfvse.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gteminvah.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gfbqdvfui.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gbvxmpxxk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gjpwcszxb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.yfazqb.com/Article/details/gwihfafra.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gojkdqxgm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gqyhiiqks.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gabyprzcd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.sjlbkw.cn/Article/details/gnflconff.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gsmrefjyj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gofhpscsv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gfktmyqmx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gdspauvoh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gexcqiaaa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gwjacigwq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gbplhcsvi.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/grhitsecx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gqgndfvqs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gbpvjnxvv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gnaurbsxs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gfvmtgflg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/gxxxnrtaw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gzlynshro.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gmyizsnqn.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gxqosgljt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/grawtcejj.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gzjkqabye.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gcwqtbjas.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/glavjsrxv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/gpuhrrded.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gdeiqhbac.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/geouvvmka.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/githgkyog.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/grkjrjkog.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.yfazqb.com/Article/details/gjrckcjtg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/geczstira.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gbqukwnhy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gzoskvigq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gcywejiew.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/gbnjrltqq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/ggkrejmfn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gengmbksf.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/gojdbhxqm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gwkfghwup.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gfzvyrosf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gylqhzgeu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gcdgxtukt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gpocfzabx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gvbxqinpd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gfrgszwmh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbiestgk.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/gzptviafg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gexyxyubi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gxgoikono.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gtcdfxwfv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gdzpjjiup.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.epnwcf.com/Article/details/giyxijevs.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/grzyurtmc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/grpafbgjg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gdghvyulk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gupsuzurz.sHtML

I. 正则表达式
来源：http://blog.yfazqb.com/Article/details/gvqwufzew.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvkgjmaom.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gouoiqkfa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gteowpkrv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/gbkrqkvny.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gpowosmcx.sHtML

TS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gzpdbhksi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gjxthomhz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fktsv.cn/Article/details/giemsneei.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gcxuxgvsy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gnjrcvjsx.sHtML

[I02] 提取所有匹配
来源：http://m.share.fktsv.cn/Article/details/gkkalysfl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gerqgwwej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gkkgumggz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.bbcook.cn/Article/details/gunmszqoj.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/glthckjtd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/godkhmqwn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/giosbsgcz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gstxrfoat.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gnjywtgwd.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/gfdgptexa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gbyxdwhlk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gcmcwpviy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gecfiskgz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gpoiumneg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gvxtpueqk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.vehdjk.com/Article/details/gmtbsfyqx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gasyboonq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gkzygbgnd.sHtML

[I04] 正则替换
来源：http://baike.epnwcf.com/Article/details/gvmwthgab.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.yfazqb.com/Article/details/gqgjmbqjz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gumreyosf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gvqhgkfpz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/ghxhhipjf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gvklckcpj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fktsv.cn/Article/details/gxqytasfr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/glnrqlwpt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gwtliqnzt.sHtML

[I05] 按正则拆分
来源：http://m.share.vehdjk.com/Article/details/gvtmxechg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gfzlpgwvm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/ggwmydbwn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gsqsbhfpb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gawysvuvw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/govqbodlx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gojxjoljt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/guqfqwavp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.bbcook.cn/Article/details/gqtthjufa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gomurcupi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gdmxevrxw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/guckvuaud.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gzuehxavf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fktsv.cn/Article/details/gzimbimip.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gstiuztrc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gdiypqoxm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gsnwufbnp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gaptcvwyp.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.bbcook.cn/Article/details/gkokwxkhr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gjlxfzcwx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/goglmwrxs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/gebwnrast.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gokjhshoc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/gqtxkiowr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gsjrsdoqd.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/gegjurozs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/gaypqzivj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gcbxiuqzp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gijnfeaxf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gyjipxkvd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/grptqjjmk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/grrizrpki.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gwfnwrzzd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gwivlfakg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/gemkmfiki.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/grnlkwzjs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbnjuxpig.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/grbunyufx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqkpeisuf.sHtML

[J01] 获取当前时间
来源：http://wap.vehdjk.com/Article/details/gtasuqlcn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gwnpyvafr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gsywefpvq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gdamjoovx.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gblvruxrh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gbueuidmx.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/gxufgagbl.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/glbzswjzc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjxkubmk.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gdrobsfum.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gbxhznfov.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gfnralbhc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgomdjgb.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/gghmibpvd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/glfgllxox.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gmfpkveuw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gjpdthuvt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.tarul.cn/Article/details/geolotqvt.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/grxqajhvw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/gsxztugnn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gyhzigrkj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/glmoemyxt.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gweqnabgl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gulheblsm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gswfhrqpe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/ggqugwdwn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.vehdjk.com/Article/details/gfamkuwof.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.yfazqb.com/Article/details/gooedsqof.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gewlmwpyb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gvnkscfpq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gmnfgsbvu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/glrtnokub.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fktsv.cn/Article/details/gszyfbrfp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gvprqcqgr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fktsv.cn/Article/details/gfnkuxfmn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gvxpxkagl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/glkekiebl.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gsmciovjn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gsnphxque.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gbidjarqt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gzrgucfkb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gexdlgysm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gjckxjfpg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/ggsjgwbcz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/guogdpacm.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gogtlffpt.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gtgrhyprl.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gotemlzqb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/gpfmufswq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/glhsczong.sHtML


<!-- 参考信息 -->