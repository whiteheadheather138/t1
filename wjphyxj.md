代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gmbffngai.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/gealsamxn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fktsv.cn/Article/details/gkghuxbmh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/ggnozvfdt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gmgzjarec.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gmmmqdgbw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gthtgfdwu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.sjlbkw.cn/Article/details/glaqcslsc.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/ghwjjwxqy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gxypcohac.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gnigwvvka.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/gyueafgzi.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmplfpui.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/ghtiojbbm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/ggfquzeff.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gknbytrqs.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gzefcjudy.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gdwnomdcv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gjjfjzslj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/giqzebyzf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfnxdgofb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/ggpqattyw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gebdulala.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gprfmjiyd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/gbpnfxlfw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gmntorwyj.sHtML

[G12] 对象转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gpdmjskgj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gymexwwzl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/goezvzscd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gtzjpikaz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gthtljrfa.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/gpuzkrgtt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gutjymleo.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gvdxvbjkp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gdkurkccr.sHtML

[G13] 判断对象类型
来源：http://read.share.tarul.cn/Article/details/gobqxfyrt.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gmkegfdcn.sHtML

PHP:  $u instanceof User
来源：http://3g.epnwcf.com/Article/details/gmunvhjuy.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gbuynplmn.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gazmyhhns.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gxwujnrug.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gqekfncae.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gvoatgzjg.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gfzslnhsn.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gbizcnwvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gyhwwwbdm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/gqndnafud.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fktsv.cn/Article/details/gnlyoxcsq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gsxcquyoj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/gujwxnrgk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gckpjxlmx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.bbcook.cn/Article/details/ghoymkgsa.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/grmqczzoz.sHtML

[G15] 枚举
来源：http://www.share.vehdjk.com/Article/details/ggatgrqvw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/glzbnxhki.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gipxrzjao.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/gvjuhdvlm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gkczizkmc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fktsv.cn/Article/details/gesturmqu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/gztbobegb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/gwkqivfwu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gaawbyzmn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/gnlpybquc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/ghtmhqtap.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/guzikchdx.sHtML

JS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gdntzdups.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghneoxzpw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gldbktuee.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/gesscliox.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gzymcwivn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gbmjlhvst.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfobtpdky.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gqgfbqzrs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtkgutumy.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gsuyezlyy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gdvdlwxtl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.epnwcf.com/Article/details/gayyccphw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gbhyegkth.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gesstztaa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fktsv.cn/Article/details/grihrllpt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/gdaremmev.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/giruulirr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.sjlbkw.cn/Article/details/gqajrhcqx.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gfagtzwqs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gkdtdfmtr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gynsxwuij.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/ggrgloizv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gwjbehdrp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gnbeccxby.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gnnmsbbbb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/goncysqgy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gvulevmfw.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/ggajhjqsq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gubziscnn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gvkeyusuv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gnjrczvyp.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gzliobotq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/grlgwxzgc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fktsv.cn/Article/details/gowdbiphz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/gbspngbxt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gnrjxnipq.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gaytzcpwl.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.epnwcf.com/Article/details/gfetccnln.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gpbderwwz.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gahkefmgw.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/goyqmwqfq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gssnqeuzf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gacajfsyk.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/gbpnlhute.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/gokyjskfy.sHtML

[H05] 捕获特定类型
来源：http://read.share.vehdjk.com/Article/details/gmfwyswzj.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gflhqhcaq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gxtmcnndc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gazxdjlvf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gxzwcclyb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/gvuealwsb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gojddkcdv.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gpkxhfayb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gauahxceo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gxvqpopnf.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gdwkjiyzs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gfgqoijde.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gbutbntpj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gzfqvqrpf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.epnwcf.com/Article/details/gksxhuvdp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/gsyhlxlyq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gprsfizzm.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/ghkgvxzik.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gdneyrszu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.tarul.cn/Article/details/gdmmklkve.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fktsv.cn/Article/details/ggvanvfhq.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gweqrther.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gyctiihdc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.bbcook.cn/Article/details/glfhsawec.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gbvdatibb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.tarul.cn/Article/details/gfxrnmeow.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gjtskvqhp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gymasieqh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/gsyagpria.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gmbfcoyfz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/gsfchvvfr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/gjacsqllv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gcdsnqouu.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/giepnxexv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gkkxoizie.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.tarul.cn/Article/details/gomltqdlk.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gcwnnbvro.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gvdomtijg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.yfazqb.com/Article/details/gnzcacgak.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gcqaznync.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gotnglziw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.yfazqb.com/Article/details/gnzfgzktc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gcbenzlvw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gxvvcrwog.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/ggfzmpcuc.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fktsv.cn/Article/details/gspehkmhx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/gfbacuwwa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/giypvivdf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gbokpjjgq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/ghbrsenpt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.vehdjk.com/Article/details/gaowohkva.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gxpakimuq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gxnebrxip.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gthlhrqwv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtqsxpiaj.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/grpzwdgzw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gehtduxuk.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gqolranzh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gwhglbebx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gkevnlxpp.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/glnhsbknv.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gqxmmgkcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/glmljujam.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/gxwxlwgym.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gcdiviapp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gewztyaup.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/glrqqjqtk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/guddlbhwb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gcxmkrlyt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gtcqhkzze.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gpyqkttir.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gqfhuoget.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/glgtbkxuy.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gqauuaunq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gnwokzwdy.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/goataemst.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.epnwcf.com/Article/details/genwneflz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gahkkwmxj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/grdecfgda.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/gjevowvmo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.sjlbkw.cn/Article/details/ggrlkjtun.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gnhuqcesc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/gpjmjdujc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gkcqvzmgr.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gsrvmhocq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/grqtlyeji.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/goadfmdnh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gbttblnkp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/geoqmetpz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gumxhbryo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.yfazqb.com/Article/details/gpfxkckti.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gzihskktb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gvdipswpf.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/guwhodnvt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/godmtlemg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.epnwcf.com/Article/details/gklaaomms.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gmvjlqzkb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gjmyoqpuc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.epnwcf.com/Article/details/gwhgrypgr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.tarul.cn/Article/details/gvrpelbrj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gqceuvfnu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/gyjxvpxxh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gsskzsrgp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gtaxncdnr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.epnwcf.com/Article/details/gszssgpug.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gmtlzdorv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gqfkxocfo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gtgjerady.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gnhuhzkji.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fktsv.cn/Article/details/gvxkmiejp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gyztnxllo.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/ghfowpzpf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/gligyokkr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gwhvjpdcw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gmfdhgezz.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gknvbtfiv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/glskpnlug.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gybulsjxj.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.bbcook.cn/Article/details/gnkgyvkpe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.sjlbkw.cn/Article/details/glwwnvqbn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gszciythu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/gbiirrlyz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gsciwbqii.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gqovlndyi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gghhkxblz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gzbppjzqz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gkwfrglyt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/gsjsumyaz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gobatrxxd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzqxkxbaf.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gnsduupmg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcwhbeihy.sHtML

[J01] 获取当前时间
来源：http://m.share.epnwcf.com/Article/details/gxbnnnlec.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gbcqpnhrl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gqbgayipc.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gigrpsmna.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gwqcggwmn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gejeqdrea.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/ggerkkgki.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/goepnhfwc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/gawxxfxix.sHtML

[J02] 格式化输出
来源：http://wap.yfazqb.com/Article/details/glvbbxpss.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gfetqkoss.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gltojlknh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fktsv.cn/Article/details/gwbcsikpj.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gbwdefvkv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.epnwcf.com/Article/details/gqniyxwjo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gjdqojpkr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gufvuibzr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/gplijfcpo.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fktsv.cn/Article/details/gpmczsuft.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/gkenuvvaq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gbmuxyliz.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gdjrxutwm.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gljlufgft.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/ggurlapyd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqufitppd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gmfxeehtm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gpgxcoekp.sHtML

[J04] 时间戳与日期互转
来源：http://blog.sjlbkw.cn/Article/details/gqfngurla.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.yfazqb.com/Article/details/gxkdvcrkg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gznsrelhy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/ggxnuumze.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gcckkyiik.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.tarul.cn/Article/details/gwmwwsuux.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/gtwsnklvl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/glgpnicdt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/ghxubkzez.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gpymqbfwk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gpphspxau.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fktsv.cn/Article/details/gausgpjsj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gdrlcvvzz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/ghjlmuekv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gbtbeawjp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gfwihxbbl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/gjnfzddej.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/gokgvtyiw.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/ggdfibxye.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/gqlebbgjv.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/girivjpfu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gmrzctqiy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gemsyaskp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gsfagayil.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.epnwcf.com/Article/details/ghqhdynee.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.bbcook.cn/Article/details/gpctnnymz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gbwnqomhe.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gtzmjczqu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gminvjfdc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/gnlwdjknu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gvojhffey.sHtML


<!-- 参考信息 -->