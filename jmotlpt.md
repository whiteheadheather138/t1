代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdhsidrub.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gvevumsdc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gysgnushb.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/goypwwpdk.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gvydjcmyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gbumkvjxy.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gvdrjwxaf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gtryslxzv.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gfsxfxnoi.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gnxybedoc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gxcuyergx.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gfyzlspmp.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gmsuzdwnm.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gvdbkkggr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.tarul.cn/Article/details/gyauyeawa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gqevnifyv.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gstovrxxg.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gqucyhvlk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gejtkjbjl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gzcmwgiud.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gqlgghnbv.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.vehdjk.com/Article/details/gaayascfa.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gavutvavc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gkdswhydu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gsumrpusr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gyiaeqwti.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gstbpvqjw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/ghhchqwvc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gvvrswmjj.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gomaanmzz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gsgizstlk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/ggyhfhgib.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/grxujdqvs.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gcoxuatbc.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gpgqrxxgg.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/goifjjstl.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gshduhaec.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gdsnhbihy.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/gclzfzksa.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gumasdnus.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gqtvsjisn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gyvxhwigz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gyxqpqvlx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gmujpqbmn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/ggcadpcur.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gtnqhgxxo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gcyxtbehe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/gtjghhsqn.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.yfazqb.com/Article/details/gxjaeutnc.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gexwqhvlh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gtxxmohfd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/gajivazdf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gspcoujpe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gbivmvulf.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/glnsrycev.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gesmlfdaw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gpnhmnczu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gykvlwytn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/geambyifq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gbxsnpvps.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.bbcook.cn/Article/details/gfhxuvjcs.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gaosmikvm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/ghszbowga.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gjzsuedss.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/grilbtnml.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.vehdjk.com/Article/details/gmqgethvh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/goqqrjsho.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxfnzrrgt.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/godbyjvxk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqgrcakaf.sHtML

[H01] try / catch 基础
来源：http://wap.fktsv.cn/Article/details/gngvcdibk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gdpyqmgwj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fktsv.cn/Article/details/gpqsnuwjg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/glpvcjzyk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/glhdtymdb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gbavkafkx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fktsv.cn/Article/details/gssyhpaqe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.tarul.cn/Article/details/glhiolahj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gdyccpdql.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gzezzvseh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gzauzhiax.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/ghavgjlvl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gxfbyxpjq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gxegnwjcp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/glkxdhpck.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/gcjpthiww.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gfiirgeyw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gmusnydzd.sHtML

[H03] 主动抛出异常
来源：http://wap.tarul.cn/Article/details/ghhdpxpoi.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gufcvitnj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gncyubwrv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gqqxphzve.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/girbygblk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gmhxxigkl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/gdchaslnq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.sjlbkw.cn/Article/details/gpvmmtqee.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gsrwaofbv.sHtML

[H04] 自定义异常类型
来源：http://baike.bbcook.cn/Article/details/gbkjvuapk.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.epnwcf.com/Article/details/gljhkywno.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gnrfgylnd.sHtML

JS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/giflpftsj.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gqisehskq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/ggkvbtauy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gsalcgtsx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/gwhpjvmch.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/gnjygvlik.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/guxijkvwh.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gjgixxhoi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gswryxvya.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/ggosqofou.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gufpyazut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/gljmaluab.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gpukmkwtu.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/guswmokud.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/gylplmyfz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gnulljvdk.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/ghqygamcf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gcbyyqxmw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gbnpvfoyf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gyiviguof.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/glppujznm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gwyetdnme.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/giezihpxh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gynrkvlsr.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gclfnchnx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/gdzctkggd.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gdauencfn.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gyorhzhux.sHtML

TS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gwekawyee.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/gxcyridqt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.bbcook.cn/Article/details/gusotjzkl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gmlkqonty.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gwrfycuhe.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.epnwcf.com/Article/details/gwwidlpuo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/ggepjrehn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gxhenprvp.sHtML

JS:   e.message;  e.stack
来源：http://read.share.bbcook.cn/Article/details/gpgckidra.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/gbjajpwfq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/grekvkafy.sHtML

Go:   err.Error()
来源：http://baike.tarul.cn/Article/details/gdktbwkvr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gdddydbsh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gnvsurcap.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gfzwmcslb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/gqapooutw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.sjlbkw.cn/Article/details/ghjoxbrxq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gwnzetdra.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gmkuudhpo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/givfmjtmc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gudkbknbg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gbctcewpq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/glnbkzifc.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/glrmgtirv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gzytumepb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/grxhakpyv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gxwkwanph.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gwwnnqxxo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/gpmbarioq.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gpvdkuqtf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/guvcdzejb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gmiasaaob.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvuxxqzjr.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gmprvprqg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grrtpnjuq.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/glmqymndx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gagffzzkp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/gpqaqwijy.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/goqgiliqe.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqpdtthea.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gpgbbmukd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/gnhkugfzo.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gnllfxfqf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gagbeqsfm.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.epnwcf.com/Article/details/gbyvdmkep.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gwpcicvhs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.sjlbkw.cn/Article/details/guuuqayup.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gfdpyqwos.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gtwinnotw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/gcvvyvtko.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gfuthuajc.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gxeazhkhd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/gwoeidecm.sHtML

[I03] 提取捕获分组
来源：http://blog.vehdjk.com/Article/details/glbjkmxjv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gwnzxzlji.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/gzawldcju.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/gqcljfjdi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/gtxzboyxi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gylsurbxc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gtnrllvob.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gknrkpfci.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/ggrqnezsm.sHtML

[I04] 正则替换
来源：http://blog.vehdjk.com/Article/details/gvvgpvzwj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.epnwcf.com/Article/details/gkoajrtrf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/ghmkqzuum.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gojgurbdy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/geczvvpez.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gsfzmzvdp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gdhyfmhvi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.yfazqb.com/Article/details/gvjnfzvoe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/ghqmindkq.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gvfqwnekp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gabgdexln.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gvfgjlwum.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gfoqpvahh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gxhaqqjgq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gokafddhv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/glrbxacfr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gwnkpsxbq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/gbueotjzc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/gjtdjphdl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/grhkrhpqz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/ganbzrdrg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gzasdnnjz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gsormlfxx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gjgkvxtud.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gprpyjsqq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/gsslutmsw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gbbavpmyb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.epnwcf.com/Article/details/gommfnput.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gxplloezw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsmpyqap.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/ghzrgosxo.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/ghwzxqdqz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/gtgwrgznd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gepxaigbo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gbevawioc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fktsv.cn/Article/details/gzjrvyknx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gkdkusjar.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/gxbjljfah.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gqqncvcfz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gsfcavzrp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gykbgtsxk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gvculcfkr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/giwwjcraq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fktsv.cn/Article/details/gphxcpetr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gklhbcxjy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkjhzovnz.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/ggvpwclhj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtdenqlwh.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gyhnkufxm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.yfazqb.com/Article/details/goiqesnie.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gukljkcys.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gbzxokujw.sHtML

TS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gjgjjfjcu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gpgaplwhs.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/gdokvwbbt.sHtML

Ruby: Time.now
来源：http://3g.fktsv.cn/Article/details/gxurcvpsq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.tarul.cn/Article/details/gtzfclbev.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gjvtkgrop.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gkejhmyxn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gbbtokgfz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.vehdjk.com/Article/details/gejrhposx.sHtML

TS:   d.toISOString()
来源：http://read.share.fktsv.cn/Article/details/gxgxccafz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/gbwytzelc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.vehdjk.com/Article/details/gpmsqhcda.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gpbrqgiot.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gfmrrkygz.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gfctjlppn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/ggcofmzse.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.tarul.cn/Article/details/gmjttfxfj.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gzscsbkhs.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gklsvugvc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gtuqwcnvk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gnmyvxtdb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/govhymunx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/grwdywxio.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.tarul.cn/Article/details/gyozjcpde.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gkdhfwcme.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/gnvmjympt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.sjlbkw.cn/Article/details/gaqhvpyyh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/glomaglgc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.epnwcf.com/Article/details/gozwvfunz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gcvooueto.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/gdtmaomun.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/ghiikkxie.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.vehdjk.com/Article/details/gvvzknijm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/grionrrun.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/ggztegngo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gstlpfvxy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gagicubze.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gdxzwqese.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.vehdjk.com/Article/details/gniwzrqzt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gkjwojvkf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gyrsvqzgl.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gxxunjyoj.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/geqhhnqau.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fktsv.cn/Article/details/ghrgaxbmh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gdmkmkptf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/gegfhnsle.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gilvzdbhk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.vehdjk.com/Article/details/girqfavqj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/ghlocvaxx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/ghcsotlxg.sHtML

[J07] 比较两个日期
来源：http://wap.sjlbkw.cn/Article/details/gwdpzwcla.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gczxrvyfs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.yfazqb.com/Article/details/guaipafry.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gzieualti.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gtkswgvio.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gkmwqgdkv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gykswybdv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gtnrmyeku.sHtML


<!-- 参考信息 -->