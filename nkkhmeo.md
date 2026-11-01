代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/ghbfsuaib.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gatlnwria.sHtML

C#:   public static void F() {}
来源：http://blog.yfazqb.com/Article/details/gurckarlm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gxsmnotbg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gnaejsplq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/ggedcomea.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gaulrpfxv.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gpvpmcjrv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gptruzwck.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/gvxpnuxhq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/gpjqzivxl.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/glanwojpw.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gkjivximk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gcuftcbqb.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/goutejecx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/gpbgrvjkp.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/gvdwfhvzu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gfhydsgyh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/gjcjnfbxh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gqxindoqv.sHtML

C#:   public / protected / private / internal
来源：http://www.share.vehdjk.com/Article/details/ggnmjwrpk.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/gtgkueypf.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gkjgnedsw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gudydpwyd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gcvqczbqp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gmdgsepez.sHtML

Java: public String getName() { return name; }
来源：http://3g.vehdjk.com/Article/details/gorxojjgd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gxwskxlai.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gveqhckef.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gdydfcunz.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gabgmlkct.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gjfbtgfno.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gsnwhzyil.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/ghqlbgock.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwrpreoys.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/gmxergruw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/groitbbwf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gcabjylsj.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gznhewevs.sHtML

[G13] 判断对象类型
来源：http://3g.vehdjk.com/Article/details/gkwmqqhnb.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/gwojyndwc.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gcuiarpph.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gyubudeke.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gpaeuhdwa.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gcyodhrkx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gshijcnty.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gjeqjwfrw.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gagrxlnzr.sHtML

[G14] 数据类 / record
来源：http://read.share.fktsv.cn/Article/details/gpehcmeuo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/gaulhpyeb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gsaagllmq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/giccipiou.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gpzriwyhp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gbgxohrht.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/gbixjioxy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/gpfzqehmw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/gtlnxuujt.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gfoumgpym.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/gyflwhfsh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/ggncokpsa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gvrntzttl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gdjmmbqxq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gfcdjyubr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gjfgsnkil.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gkncjytor.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gjzonpioo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.yfazqb.com/Article/details/gotjjbivb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gsdleqifq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.epnwcf.com/Article/details/ggeiycxyo.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gylnrfffr.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gldvodpeo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gpxhdutzo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/gsgjmgonx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gytujcyqe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gnowabqrn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwdkwzmgi.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gccdouria.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvlrzecwg.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/guqngotkk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gepcdtdxf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gfexhogdu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gbbptbgwx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gwjnkbyqp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.vehdjk.com/Article/details/gxmmcptuu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gfejknbsx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gmttcxpro.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpoamdchj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gedqoriyi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.bbcook.cn/Article/details/grjbyseuk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/ghzhcprcj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gsnwgyvxz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gjmtcjgre.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gjnjqzqbo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/glfsgjlmn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.epnwcf.com/Article/details/gvzccaaph.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gfbfvyspk.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/gnfcwnpwn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/grbdwkrih.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gybppflys.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gkutljbxe.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gbemarxrg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gcphcwpbm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gdykddnza.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gtltdvgcd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gzeredrnw.sHtML

[H04] 自定义异常类型
来源：http://www.share.vehdjk.com/Article/details/ghskyknpl.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/grgperfhc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gcvrcxvft.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gnwiegncp.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gilzffusb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gynfntwgm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/ggglbcjft.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/gnroztsmx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gymrhxfnc.sHtML

[H05] 捕获特定类型
来源：http://mobile.sjlbkw.cn/Article/details/gancujufw.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gwbvrsiew.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gdmkmdnfk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghrutecdp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gsjlycyit.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvymsytlv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.epnwcf.com/Article/details/gmldcfjpo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fktsv.cn/Article/details/gwauorbgg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gspcklduo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gqmgzgcbp.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gesyexicn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/guaxxzbbz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gcfdigykk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gkymftrwl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gshyhbwdc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.tarul.cn/Article/details/gdfcapnvq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gbnwzmacz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gzawozjfb.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gqgmemylb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gsyehnzmq.sHtML

PHP:  assert($x > 0);
来源：http://wap.fktsv.cn/Article/details/grttkzuxi.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gnxnrlrad.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gpfbhtltt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gqynkpopw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.bbcook.cn/Article/details/grnybqhky.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/gnjrwopoh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/ghoserarq.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/gjiqonnut.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gexrkjfgd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gpudxtcwz.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/grvmrdqmu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/gtsnetlqg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.tarul.cn/Article/details/ggnwrubmt.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/gknuhehxr.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/guqnadili.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gqannvfen.sHtML

[H09] 带错误码的异常
来源：http://baike.yfazqb.com/Article/details/ghjtczzdq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/gkytggrha.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gnkfzixur.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gkrbwroea.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gadxxxdjb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/gnehthwik.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.yfazqb.com/Article/details/gpwuespds.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/glrvrvkpq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gxntgzbbv.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/gicltfldz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/ghcjkngfj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gqqunpkib.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gjpmjjwzc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gawgvvfxa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gurgllwct.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/guyiwwhac.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gbcumdecl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/gakoklquo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gorrsstbf.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/geborbjzk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjvpjyzlq.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/ggpwrvxoq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gnivjummd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gfwedflfb.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gxaycmidr.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gosauifsf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/grtkwfjdw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gmeydujlj.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gnivjamon.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gzutnmupp.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/goimvipnv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gmhkmysob.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gszijzviv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/gntevanzx.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gyogzcpaq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/guzqjxout.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnylqhbgt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gyukbdkvk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gfpbalgof.sHtML

[I03] 提取捕获分组
来源：http://www.blog.bbcook.cn/Article/details/ggamkjkur.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/grnxcbxko.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/guicujdht.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gnrhafnrv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.yfazqb.com/Article/details/ggvihkude.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.yfazqb.com/Article/details/gkfbzyrjc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.tarul.cn/Article/details/ghdmlggbg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gozaxiizj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gtcqnvnun.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/gytwxfbus.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gteffowts.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gdstskpin.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gswytdapy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gnvaojofb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gjluvfuyl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gybhylxjb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gkbemvttv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gvelkemaa.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/glpkrhcaf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gimqzkdbb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gazlfhkuc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gkndnlxlw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/guxweiqjm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.bbcook.cn/Article/details/gagnvmbvd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/glgwpauic.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gmmsdvucs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gctolkftv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fktsv.cn/Article/details/gikqwfizh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/glpcuxihz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/ggtvkfgkl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gyggzweue.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gmprwikzh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gsjddgzhj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gsedpvxxe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gfteaaxka.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gxitflpot.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gaegvoufz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/gdpiemzwm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gystvycuq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gerifvhbw.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gzdudabnc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/gwafpxgcc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/gpqwnagns.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.yfazqb.com/Article/details/gltzlpfzc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gjxqcoizx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gozmxktzq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gonrreeul.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gdtukadgx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/grbmhrakv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gaqbjkduh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gilyhhcli.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/ghvhzushc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/gbrtndxnh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gekvjapsl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkjocydvg.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/grmxcrxbq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glkqcxamx.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/gtpncynlp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/gddqycmtf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gyfxjzmfy.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gvlgkdrmv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/ghjsifblu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gvhdflxix.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/guvtuhlrl.sHtML

Ruby: Time.now
来源：http://www.m.share.yfazqb.com/Article/details/ghghmnhoa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fktsv.cn/Article/details/gmjcdvpii.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gbmqeauue.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/ggsjacmzn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gtldyibtb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fktsv.cn/Article/details/gudjbltlw.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gzsbhuyxl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.epnwcf.com/Article/details/gqxufwats.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gdhdihsib.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gcgtgepwx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/ghuvjkpau.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/gqoefzdlf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/geeofsnvy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.epnwcf.com/Article/details/gkryncbiw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gtizdcdrq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gkluzypqf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gtmjsdkwz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gfkgckmka.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/goieblgrg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gkbzboldu.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/gegdvurvp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/giyqqyuow.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/ghehsemza.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gesjbnmvc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.bbcook.cn/Article/details/gmccbglqe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gvbmsyiiz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/godnnrolc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gpsiegcps.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/grvjxuyyo.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gubuslekk.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gdiamqpnv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fktsv.cn/Article/details/gimbgglpv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gidseiccp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gqzbnzazy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gyqsurklk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/ghahyogan.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gmhnmclkk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/guuaaovzp.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/gmhgteyyo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.yfazqb.com/Article/details/gehpulumq.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/gsrbdvlev.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.sjlbkw.cn/Article/details/gtwbcxlzz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.tarul.cn/Article/details/gibzzjpgm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gazzreuux.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.sjlbkw.cn/Article/details/gkcsbytyh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.bbcook.cn/Article/details/gonkutotj.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gkoqusvhg.sHtML


<!-- 参考信息 -->