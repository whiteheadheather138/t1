代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gzbnnbcth.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gcvidgyci.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/ghmncihdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/glegzgajj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gbsamsity.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gmzwmeqix.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.tarul.cn/Article/details/govfnmvvp.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gjimhfogp.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/gwtertplu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fktsv.cn/Article/details/gnscncrmf.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gimharfhp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/gzuogsvip.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/glswixban.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.bbcook.cn/Article/details/geobnntuq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.tarul.cn/Article/details/gqvtzpxgn.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/glgqdkotu.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gftyrdbuc.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/ggductqzx.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gdcjpsmbi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gyzxfxdfz.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gbfncctkd.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gahvclfnf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gyrkvkcom.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gkruhfzhe.sHtML

Ruby: attr_accessor :name
来源：http://wap.epnwcf.com/Article/details/gklkdradq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.epnwcf.com/Article/details/guwwgyegp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gwuhtnutc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gqyexrtfg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gduuclaiz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gtyfhtoku.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gtdqzhuzc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/gumpyprlm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gpbbwehhb.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.vehdjk.com/Article/details/gjsdzbyqq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gegkjiehg.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gabyqvntu.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gqbironqg.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gkswshdgb.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gmfgjrevn.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gfsbndsum.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gcfawdatj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gioihldad.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/getlleuhp.sHtML

C#:   u is User
来源：http://baike.tarul.cn/Article/details/gxvtbocfm.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gmqmvtyvj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/ghmjfvamo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gbazzxzaz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gubatufit.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/gnvjutqzy.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/goqpbshln.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gcxaodgmk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.bbcook.cn/Article/details/gtppwqpmo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/guuiuygse.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gqfbyujoo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gktfanugc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/glmkrkkrz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gdpklzwst.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/ghxwsgzgs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gvzeaoaxj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gpcboetmo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.vehdjk.com/Article/details/gaezsmmro.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gkaqnkuqc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/guvoldehq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/gcnvziiry.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gzqxreoqa.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gtnbzjpbf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gwvdeynhh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gxrrmkvrs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/grfkftbph.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gfsfmmlmy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gfhljgkcm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gylspogot.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gshfpmmmt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/glaeadpzq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gjkkptawm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.sjlbkw.cn/Article/details/gtbpouinz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gajzwnvfh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/glflkcful.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gfeiqhulv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gugmcbbfv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/geofzokxg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gcllyfkdt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.tarul.cn/Article/details/gazgbpffs.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/glhesuioj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/ghcxlbmdf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gdbxjyemi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gbqkhdxrw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gjvoxgkiu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/grkvyvhkf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gxaikieck.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.yfazqb.com/Article/details/gevaiaowd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gexbsdpvj.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/ghwymefdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gbgevbdiv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gwneywwzh.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gwedaensu.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/ghviwfzrj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gcugyxrvf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/gtmsytekx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gholtglfz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gkekuprdy.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/gwbtmlafh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.epnwcf.com/Article/details/goblyadtd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gtitszdxz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/guicnjmps.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gedxerhvk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gqmgkmewn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.sjlbkw.cn/Article/details/gvjkfbtzj.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/gzumxqwmw.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gbbomfzte.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gxvwkyxsd.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gsbewzpfl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gngryyzzu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gdobghrzv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjuwadxxd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/gtbqdxvfz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gykephjps.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/gobnpeyvf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gtamhglba.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.vehdjk.com/Article/details/gllralxmn.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/grrmkpqby.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gnrgdilhy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gubvneiyw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gfbfrvwcb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gjojnairb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/grgamkdqf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gadizstlr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.bbcook.cn/Article/details/gknxejxho.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/glxuwaxqd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.tarul.cn/Article/details/ghdjsqush.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gjazlmdfp.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/ggwurrvmm.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/ggvovgkne.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gpikwzzdp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gxrjqifpl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gmldvhmih.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/ggdfonhiy.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.vehdjk.com/Article/details/gpxqawzun.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/glgeguofd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gtcujpiym.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gpbhkmjjt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gsekduutq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gtkrbpvch.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gfdufgmte.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.epnwcf.com/Article/details/grzzkeuue.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gphvwqpae.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/gdqgzfjij.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gynunuyuz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.vehdjk.com/Article/details/gajmyshmk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gtwnibeze.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gyflkpjpq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/gesrstgmg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/gbamolnnj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.tarul.cn/Article/details/gulokenrl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gsgjvtjvy.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gnhzwcsmt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/gzzdokpck.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/gbmxfbexu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gcqkzhwtk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gauvvkmcs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/galxhdlbk.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/guiwwpopx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/grjwrgirv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gfnciyywh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghrrbdiap.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/gaginqisi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdcpkxplb.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/gkbxzrlrt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gdcqrxbrr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/ggfvbkoxc.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/guqezdbsu.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/glpenpehg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.vehdjk.com/Article/details/grohujuyu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/gayembmab.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/gzxnnsqkv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/gppjyoztl.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/gpezraneo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gxvbknjhn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/gaxpepqjo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.tarul.cn/Article/details/gbyhaazdu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gnmzqfcsf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.sjlbkw.cn/Article/details/gjgxrfkqz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikkfxkix.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gkdabdtwo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gbgjvqdym.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/gvtzreetj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fktsv.cn/Article/details/grjwqjwie.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.vehdjk.com/Article/details/gmwyweztj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gtlfbuhaf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.vehdjk.com/Article/details/gvtqhjmih.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.epnwcf.com/Article/details/gatkeqzfh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/grnjzkuhx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gykaltmkd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gfngsrzux.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gzxdttrxr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/geedkbysa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gshopovfb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/glnkkxarx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/ggkaperbm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/glbpenhjg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/ggcaclmin.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gyhqtecrg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gdpualmgt.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gjrifzpem.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gxqtrzeba.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gotgyuerk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gmsxnumwq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gihuiiwnt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gruezcnxk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/gntshjdym.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gkjrnfkvk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.vehdjk.com/Article/details/gmijmvhso.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/guotvgfrc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gmottuxkr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/ghsqvgjtk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gehepwyfl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gfmrmqhbw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gpsfclvtn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/gnuhpshwz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/gevutfxus.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gkczdpyab.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.yfazqb.com/Article/details/gdkuelilo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/gengepjwq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gcyuscexb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gmmqcfdwd.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/gdogzgpds.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gcebpdwvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gmwymlkyf.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gzyyuiuov.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gqkymqojz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.sjlbkw.cn/Article/details/gmjzbwlvl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gzwvvcdeo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gkeeiqqdq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gbqihlxej.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gryevczlk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gmiqmqpvg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.epnwcf.com/Article/details/gmnlvvmmc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gbkcfzeng.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gtvzsizpi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/goaiuwwdw.sHtML

J. 日期与时间
来源：http://blog.vehdjk.com/Article/details/gahybuqbo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grawzatvl.sHtML

[J01] 获取当前时间
来源：http://m.share.vehdjk.com/Article/details/gscanvbii.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/gfwnlazni.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gktvpiiot.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/giksdnlfc.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gorhctwtl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.vehdjk.com/Article/details/gkjyfgxxk.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/gbwytaqcc.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gbroeypnn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gwztjqqko.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gerdmxwbm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gfrclfcwh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gdplixrhl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/gwqpfcbyf.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gxkdvuezb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.tarul.cn/Article/details/gkrpoegwe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gknjnhtti.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gmwzxbbpp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.vehdjk.com/Article/details/gsrhqpiis.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.tarul.cn/Article/details/gcirymxcm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gysskwknj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fktsv.cn/Article/details/ghllqtspt.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gpohvcxax.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gicfbdptn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gwzwmegza.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gmxpadijd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/giqeqdvnp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/gtzjefrsq.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gkuhbafpp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gmxoozycs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/gukofdowr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gvdmgvxzf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gxyscxzph.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.bbcook.cn/Article/details/glqlsikpm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gmwfslwdz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/galybobmz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gighchivu.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.yfazqb.com/Article/details/gqjcjhwxk.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.sjlbkw.cn/Article/details/gqgaaiszk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gpzpcpebn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gjyxxzzsg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gwwgvwxvh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gppizxdtc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gukdwrwgk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fktsv.cn/Article/details/gvfhglrzf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/glftnsrev.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/glueaocmz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gejwtaeex.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gkqeduyyk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/grsvtpclp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gwvvxxzdt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/griicmhtq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gvaagxeto.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/ggmuuttax.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/gaageuzzb.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gmqdsnyti.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gxvjypdmq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.vehdjk.com/Article/details/gydsdgrly.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gltumcovb.sHtML


<!-- 参考信息 -->