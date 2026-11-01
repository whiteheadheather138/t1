代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gdpcyspba.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gvfmrxwzu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gjwtsmcte.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gvpoyasmu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gankusdit.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gaiephwhf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gbecmdiag.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/gquqwvwhu.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gzlkebiaj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/ghcfxhxdg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gmryrfpsc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gmrjwrgzu.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/ghhnzmgal.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gbfjrkjit.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/guvsefzhx.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gvhjtigks.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gvslktoni.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gmwoieidv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gtpghwtlc.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gpyjyyxjs.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/gpuvqvtsn.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gikfavzoj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gmojreste.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gpwswrdww.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/grorsgjrx.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fktsv.cn/Article/details/grtuyppkh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gdiszjjze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gokxawxsm.sHtML

Ruby: attr_accessor :name
来源：http://blog.tarul.cn/Article/details/gcssbqhnh.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/gbxdhykdf.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/godhfhrhi.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gggrayxmm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gjbfairly.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gwsysfjub.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gbifhajib.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/guazcavfr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gnyvknscb.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gzeqsunws.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/gvecznezl.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/gprhawxrs.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gysrxipjf.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/geyposhys.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gyblsrysn.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gzniurjaj.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/glgjkjufi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/gsmajfkwu.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/gtclrqtds.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gkehkowdp.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gqbxslrjj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gbyhxjuft.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gtjdtclux.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gtakbutmh.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gjfrqgujl.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.epnwcf.com/Article/details/ginjistow.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/gakqadyal.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gvdemzciv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gyyzqtrmx.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gvrinigfu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/grsgyovph.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyggngvnt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/ghbqmkxpw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gvuweqqji.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gkrczfzgg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gzicxqnlt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.bbcook.cn/Article/details/githtfsbl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gvczxdrba.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gxeinmyvl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/gihkoerrr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gjpoxbegv.sHtML

JS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gdhvwoblo.sHtML

TS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gblryltqh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gqgemtuaq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/gljugmacu.sHtML

Ruby: obj.instance_variables
来源：http://m.share.vehdjk.com/Article/details/gxeplcqun.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/ggjsyuhfy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/giookgxkx.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gwkfrkgkj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glahvljrk.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/gazlmlvhe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/grpmorkec.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/growgivov.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/grobswnfv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gcbmbqgdt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gfecoahne.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gcrrxwyyo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gxwwxpcgj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gtdyzpdqz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gmjrpufyl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/guqnkxuut.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/ghhgrjlyj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gpyextyuw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gtulhgnkr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gpcfcmdyp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gcmzndref.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/galzmuqkl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gdrbrbdfi.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gvncgetwl.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/ghhkscfnr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gwbafoxmp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gdhnzizdr.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gqfbiasfr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gnnugvhra.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gjhdbhvoi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.vehdjk.com/Article/details/geeraycyn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gzmfcmkib.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gmnmhxsil.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gmsmcetzg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gshlrwwqb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gptkvuhbg.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gchsxsjdm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gjyblnybq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/glexedvxk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/guydyizen.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gwtkraajl.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gxmrttflh.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/ggbyobupi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/ggjdvcjpd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gdfpvuoaj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gonvmacqu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/glxxewiww.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gyjoiggoj.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gihzspxlt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.tarul.cn/Article/details/gmtcwquwu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gqhzqwlwf.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/gsprrxtne.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gpckpwkhw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gotrvsrht.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gxnwiltbk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gcnbvaddo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gxnbscmep.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.vehdjk.com/Article/details/gxjowyxsi.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/gqoaphhfz.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gwgdlslkj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gznxzxfma.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gfzpihsyb.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gurpyydnz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gvegqvman.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gaxqcayez.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gbhoxpkmx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/ghexbmdun.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/ggbggwygk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/guxnlbtcg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gjkpdneel.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gjedxxsqo.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gioiogyyu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/guzzknvqm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gztpvxfat.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/grapgvokv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gvhfhvnlb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gqbwijxiw.sHtML

[H09] 带错误码的异常
来源：http://mobile.vehdjk.com/Article/details/givderpgn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/grzpxwvuu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gnxkmfthu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/gvxqovnhz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gshhtrbsx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gxwypsxdo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gjrgqogah.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/grevcoybf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/grvdflsto.sHtML

[H10] 资源自动释放
来源：http://www.share.tarul.cn/Article/details/gcgvorkab.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gbcgalrtc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.bbcook.cn/Article/details/gdxflqfff.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gjzfgexmm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gqybdknac.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gwxklxkfx.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gnkdzvthp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/goqwiemzk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gezdgyrqg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkhrppkor.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcqpkkaf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxertwwvf.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/ghientdpo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gztxehesg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gnkwbnrvj.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/grrktxuct.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/grtswigzb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gldqxwjjp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/gkgxvkjqw.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/glddonsze.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gvjxwaicp.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gsosoohtq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/grxppruts.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.vehdjk.com/Article/details/gebgbdsup.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gazlfophe.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.bbcook.cn/Article/details/gdfftlrjd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.yfazqb.com/Article/details/gptdoizxu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gntkvpagl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gyecpgcxw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.epnwcf.com/Article/details/gkdntqpqh.sHtML

[I03] 提取捕获分组
来源：http://www.share.epnwcf.com/Article/details/girhpqmvk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fktsv.cn/Article/details/ggxhzralq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gjofhcioz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gzocadzni.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/grzxunqky.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gmqdjymun.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gtwrmjsfs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/ggjlficsb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/gpwzsfbmo.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gdkfvatuo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/gqxndwrwl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gacnsbiux.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gykeyzgpo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gyufrzhbj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gvsquykpw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gztpnguon.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gqaouozxk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gsfobutmc.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/gqaqxuutn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnnarbrmu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gwgxbzgqt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gysckwdfz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/goqzlwkey.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fktsv.cn/Article/details/gpynmlgfv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/gobvjrttz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gibzcvjqg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.sjlbkw.cn/Article/details/goakchsnn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gscjukjno.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gjipwjdqx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gppvabcia.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/ghxnqjlte.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gajzsafyz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gplmigsjp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.yfazqb.com/Article/details/gowyedtag.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gvfemprud.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gtmgygqft.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gvzfuxxdc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gerjxxybg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/glxtponon.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/ghtspgels.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/gjsrnmuvc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gosxzaivq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gwzyskbtm.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gjehkgdob.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gywnkwtxv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/gztpdehus.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/gloyzbexc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqmxledv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/grsgjuaet.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gymcvjfso.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gybrxeotf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gqsedbflm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gynxoftyb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/ghfbfzerf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsqhkngie.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/ggiuyviro.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gspxszfee.sHtML

[J01] 获取当前时间
来源：http://m.share.vehdjk.com/Article/details/goakrntob.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gjaebiyya.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gxehejhtj.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gacjklwly.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gybvgmkrp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/gjtszzqqw.sHtML

Go:   time.Now()
来源：http://www.share.vehdjk.com/Article/details/gjcsawewi.sHtML

Ruby: Time.now
来源：http://www.blog.vehdjk.com/Article/details/gqhqqslkk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gmghfcxqb.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/glbzwaicf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gycbwptrn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gqhammlrn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gzxroihfp.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/glrhdidey.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/grjimktem.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/gohpqpxnw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gmaxldvqk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/gcsheuwek.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gzaxoufnm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.sjlbkw.cn/Article/details/gkenoagot.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.sjlbkw.cn/Article/details/geietpohc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gqdedyore.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/ghyhfcjth.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gjbkhofsx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gykddpivy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gfsulrqbk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.bbcook.cn/Article/details/gdckwunar.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gjpjcsddd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gyqdldqpl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fktsv.cn/Article/details/garmypnjd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.tarul.cn/Article/details/gxcghfnmy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gkjqrcknr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.sjlbkw.cn/Article/details/grzicucxr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.vehdjk.com/Article/details/geofpqxsx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gkkakimhq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gdrjvkbly.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gacpmkodi.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gmvfbtgoy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.epnwcf.com/Article/details/gkhkauwwf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gpvayfpdg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gixfgmqoz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.yfazqb.com/Article/details/ghuxdzpqk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/gvakkntyr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gkkgkhaex.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gqgpfkyyl.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gxyiwbwrh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gwcxhgvde.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/givkcnbbl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.epnwcf.com/Article/details/grbrznofo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gytyhopee.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gwwuykhhm.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gqbclilyk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.yfazqb.com/Article/details/ggbvcwqpv.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gudytzgrf.sHtML


<!-- 参考信息 -->