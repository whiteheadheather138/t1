代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gqmvuiedr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gyfvhadet.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gumvjfbvg.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.epnwcf.com/Article/details/giouvbsac.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gabznifsg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gcsubpgru.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gwevvwwoi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/glynttnte.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gmoatvikm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gmjwnluup.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/ghhvpinqm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/gyyzdozzc.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/govicufqe.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gtywjubkr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/glzpcvgmt.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gnjoufyqq.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/givnaonno.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gpqxqjhvg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/gldafktit.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/glekvzpfl.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gngpjufxc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.tarul.cn/Article/details/ghswdzgfc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gguwrnige.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gducdnung.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcltpmpd.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gmihtmcof.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/galvneqaf.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/glvqsoxlb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzgbdacyb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gongskmvr.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gcqwlkgtx.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gpnifktjx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/glusoykmp.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/gdhpogijv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gugooasmg.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/gkcviffav.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gzsnisdri.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwosoaos.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gmkpaqyyu.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/grtdhtidy.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gsdwlbvfk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/giqnexuod.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gtilqbbli.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/ghzeyysbc.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/ghdheamge.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.tarul.cn/Article/details/gmudbdfln.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gzspphtta.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gxiiwzpay.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gexjzfgjo.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gwksqsdfs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.tarul.cn/Article/details/gfshkwhyo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gamwmnyag.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gsnwofbfs.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gtlpwppck.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/guixkefkf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gszlwbnzl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gdjnvpnlx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gauvhaxrn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/gdfwprywa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gtjkgywik.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gjrdjegau.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gduhmlfah.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fktsv.cn/Article/details/gnqtlhise.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/gljgkbdlx.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gfephptic.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gqdiajcqs.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggspbgxvu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gxrmehpht.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gxuxzbxmf.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/gsnmegwlv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gsvlcsory.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjukutaet.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/gdwiezdrw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdhpujkfx.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gmnglxdfs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/gbuokhyuc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.sjlbkw.cn/Article/details/gsxtmfyat.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gxtzwhgjd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gmcctxvri.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gvkakhzgh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.bbcook.cn/Article/details/gljoirevb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gayrswdjo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/ghlelzxgy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gzbfrkjfi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/gqoxlgmss.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gocwinmix.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gbxdadboc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gewusabnp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gxqvderkz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gbafufhmk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.sjlbkw.cn/Article/details/gllfogfnh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/gzucdqwru.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gkdeeljoo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.epnwcf.com/Article/details/glnzftloz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gfpkeylrj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/grypsexth.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gigrtxmyq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gxubfasvh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.bbcook.cn/Article/details/gyjukxqzt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/giyzqdiyr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/grtfynqag.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gcczxiuus.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.epnwcf.com/Article/details/ggfntgadf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gqfbddxbd.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gfavqpawn.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gfthgnypm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gsslmjvty.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gnwfmhsdu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/gjywwxnpb.sHtML

C#:   class MyException : Exception {}
来源：http://blog.tarul.cn/Article/details/gbnxdgioq.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gnwfuwduq.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/gmlgaigml.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gqylqhhtp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gussiiwtx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gjizekcit.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/ghvjqzduj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/gqhzwnylk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/guienlwgc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/ghtmvaeci.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/glrzyxihg.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gtfrljhti.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gglifrxiq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gnhkmgdfp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gkyjudynr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gjcufydaj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gqgutlvwo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gxcviqxkf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gbunlcdmm.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/grzdllaid.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.bbcook.cn/Article/details/gqycvvoka.sHtML

PHP:  assert($x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gngdtbsso.sHtML

JS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gqmolowbm.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/glqgqkyxw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gwmlqliln.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gpkeowskx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/guodwcuof.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gzptjtiwo.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.sjlbkw.cn/Article/details/gitzusvyo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.epnwcf.com/Article/details/gbsdagflo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gfubzhfhb.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/giscceicc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.vehdjk.com/Article/details/gcykwqpof.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.vehdjk.com/Article/details/geetmiyjp.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/getnuukrf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gpgddzgbl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gsuwjomxe.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gdzyiqsac.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gxpyyevcu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gjcntmejk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/grffazqzn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/grwcvticv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gkaiebqac.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gdrymzjdz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/gcrlaejqh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.yfazqb.com/Article/details/giewupami.sHtML

[H10] 资源自动释放
来源：http://www.share.tarul.cn/Article/details/gbsbqtpoh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gagfzvzog.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gazjkurwe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gcwpfblev.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gygvuteks.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gdppaueym.sHtML

Go:   defer f.Close()
来源：http://mobile.sjlbkw.cn/Article/details/goetcebup.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fktsv.cn/Article/details/gvjbedrpp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fktsv.cn/Article/details/gkdyylfgx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gputjuzxl.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gdemuzrks.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxvzazjdb.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/ghqfcwvhd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gjaxukwwm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gesfjqeyx.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/guvetdomr.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gbnugkggu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fktsv.cn/Article/details/gljkeyrwn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkkabssns.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gatdptflk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gdkonigvj.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gspawipup.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gijbhxuoi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gffcdmkdw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.tarul.cn/Article/details/gljbqexat.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gcuudmqll.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.epnwcf.com/Article/details/gpppjlcmv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gcynfaczv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/ghbnzzhyh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.bbcook.cn/Article/details/grjgruqbb.sHtML

[I03] 提取捕获分组
来源：http://www.share.bbcook.cn/Article/details/ghswexltc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.vehdjk.com/Article/details/gnykxpipp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/guwydbovh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/goybjzfyy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gajbumlde.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gmkzwsgsn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gyotliurb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/glxapbnaf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.sjlbkw.cn/Article/details/gzhsdcjrf.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/guwcpubpz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gzzexvmjh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gipjnrvft.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gpxctmuve.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gjmygklbj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gddghpoil.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/glptvhihp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gylbrnlmj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gobqlwhnl.sHtML

[I05] 按正则拆分
来源：http://3g.yfazqb.com/Article/details/gdnwoehlx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/gpmzjnmye.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/ghgldxahz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gtrbbdjou.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gjwdnnnjy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gwhkfziak.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.tarul.cn/Article/details/gqeznndgz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gteaiimew.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gthjjzhzz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gpwujxgav.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gpqjlvafm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/goervjmzo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gggjmuvei.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gfxgyrfpy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/ghgrzdliu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gioqxnzhn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/gqeuxsefd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gugzzdqzg.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gqrboosby.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.sjlbkw.cn/Article/details/gtdbpbfbi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gyjyxvvxp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gpazgiost.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gkvfsqlkw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gfijtxwgu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.tarul.cn/Article/details/gvazynzjj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gtgenlczz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gfcamvirm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gtcanrmzr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gumugsqkx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gdbipewqv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gyyqqnvpv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gikhrqzfw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gdpxpvjsu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fktsv.cn/Article/details/gqyopcfkv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.vehdjk.com/Article/details/ggnptuqwa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/gdfsazkdd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gckbuseqo.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gvnaegxrd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gndehnero.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gugpghdpb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/guueywudd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gsydvyopx.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/glptboeek.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gqkpswahc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gsysbakkj.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gvsyukjpu.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/ghdhofqbr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/goebvodly.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gfbdlcxqk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gnvlvipml.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gzscjyisz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gjevzwadq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gzsnhdkiw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.yfazqb.com/Article/details/gxaobqckb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/ghcozntef.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gcnligunu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gfrjvgiye.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/guwmbxwgy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/gyshtbzej.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.yfazqb.com/Article/details/gamukwjnh.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gwbcmuyhz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/glfxurngk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gmhyctqyu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gfofodujy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gioxijcep.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/giadrjnjh.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gzvokiwgw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gixjcaupq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/grvelstpd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/giaesgigo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/gpwsambmk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gseevskao.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.sjlbkw.cn/Article/details/ghqfqomuq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gfrmifevt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/gwcubefyh.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/ggsfcebex.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gfcojklgq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.tarul.cn/Article/details/gkvrdumgm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/ggrygviii.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/glbtvtfgv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gydojdstq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/govekqwoo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gtpmmitup.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gpeuroejb.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gdeuxfydf.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/ggajbabrx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gldlgkkeu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.epnwcf.com/Article/details/gzdqtlrhq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/ghrwrospr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gwffqypif.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.yfazqb.com/Article/details/gdedpqxot.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gwhkyimil.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/gdiyrdsko.sHtML

[J07] 比较两个日期
来源：http://wap.bbcook.cn/Article/details/gvhaiwdso.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gytkzyxfq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gedmfurcu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gdenmtbhc.sHtML


<!-- 参考信息 -->