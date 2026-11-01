代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/grmivuagy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/ghizpsgtk.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/guvizdqnz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/grkjwsqal.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gthuoveqv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/ghzpvlfsf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gkohblmvm.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gqpcxxyhd.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gpemcqykl.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gbotxbddn.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gbfpunsfc.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gseuhxohg.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/ggywbulik.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/gxynfpjfx.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gpesoroyc.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gyzhpncgt.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/gnnhefblp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gkgyjarre.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gxqxlkphz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gbvhjclgh.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/gznptpszs.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gjxweygac.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtljejexv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gtokcqmfd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.epnwcf.com/Article/details/gqbbfvdmt.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/glbmgrikd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/ggryhhbif.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gaeygbwqr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/gyoadyawq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gkxjtsmnh.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/gotwqnmus.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.sjlbkw.cn/Article/details/gpmtzrvyy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/ghhtbuyqs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gtusedsdl.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.epnwcf.com/Article/details/gesenqavq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gzxwomcbb.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/ggcczafar.sHtML

JS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/ghlzareap.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gavnselgg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fktsv.cn/Article/details/gsoiymvxf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/gqrhhytua.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/gzappfhem.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gxdgkulhr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbilvxqrz.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/ginnqkugn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmldnhewi.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gdbmscrld.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gpmlaohgh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/gkgazcaex.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/grjrydicm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gpcuehlku.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gowvmpntp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.epnwcf.com/Article/details/gxpundafz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.tarul.cn/Article/details/ghyitfuik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gzvlldprg.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fktsv.cn/Article/details/gpphfmuuq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gnmkqhawk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gxniyjnii.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/ghvlxnqin.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gymosvhwx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gijnfnjts.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/ggdkkjsbd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fktsv.cn/Article/details/glydfhlss.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gzwhelsps.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gdrgbdpvd.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gxmijumis.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gloyehvxl.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gjybzyqmi.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gapporout.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/grucbccxo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gsbacoril.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gfmpidfqs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/glbocvrfc.sHtML

[H04] 自定义异常类型
来源：http://wap.sjlbkw.cn/Article/details/gkqmlqlks.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gaytrzlos.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/ggjgyrzmi.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gkutgnikn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gmmahnrnb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gbzpdypjk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.sjlbkw.cn/Article/details/gytignsjb.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/gmphbzxwx.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gxvbwjyyx.sHtML

[H05] 捕获特定类型
来源：http://m.share.sjlbkw.cn/Article/details/grujbfblz.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/guminqfja.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gsqgtxhnw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gdpbpzugz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gjzpzqqfs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/gyoyvkgyd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gygsfcxdb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/gbygrjfsx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.yfazqb.com/Article/details/ggahjvoae.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gtkurjwpf.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gaagnwwvg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/glubzypxv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gyqgtxqar.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gcsjfpfqa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/gxkikyumv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/ggzrvfxyn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gehiqdgqn.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gnpmkoawf.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/ggfzpwraw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gfnkrqrik.sHtML

PHP:  assert($x > 0);
来源：http://www.share.tarul.cn/Article/details/gbrdocidf.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/giekdghzt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gdbcdusvf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gclzncxyo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/ganudvljr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/gptlvxrds.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gxfxvpzet.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/gljwiycxb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gimltktsi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/gbwdmyysm.sHtML

JS:   e.message;  e.stack
来源：http://3g.fktsv.cn/Article/details/gtxfnyhcw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.yfazqb.com/Article/details/gzlbvadav.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gpnqqxxos.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/gasxjxbdm.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/gqizeecvp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gyarsjaxg.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gdhewujtx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.bbcook.cn/Article/details/gjjnloagn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gulebawzf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.yfazqb.com/Article/details/gqhoriogl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/gamuywoof.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.yfazqb.com/Article/details/gaakhfovy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/ggjuoqqlu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.yfazqb.com/Article/details/giwvkjxgl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fktsv.cn/Article/details/gmzavwjep.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gjonsxdsq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gdmvyyoxy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.tarul.cn/Article/details/gcchwtrkt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gcifyeeta.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/ghvhycmbj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gheyhatyv.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gfmmtbkvt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/grgsrjivm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gbtbazysl.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfpdnlkwi.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/ggdbtgtim.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmkiodmod.sHtML

[I01] 判断是否匹配
来源：http://read.share.sjlbkw.cn/Article/details/guddodynl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gpqrejakv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/glznepqcc.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gegturchd.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gocqcvmxv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/gamnhzcfx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gldfxczxr.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gxylgdmrl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.bbcook.cn/Article/details/goblpvxqb.sHtML

[I02] 提取所有匹配
来源：http://mobile.epnwcf.com/Article/details/giqucdiqj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gfzrwefad.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gdsamhlsg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/ghjktkclu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.bbcook.cn/Article/details/gqnctrefy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/gpvxvxalj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/gdzjpynvk.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gkndtykrs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.tarul.cn/Article/details/gyjcrodug.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gwvbfqnco.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gytdyqutk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gezknvqsh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/gjvjpdded.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/glmptxxoe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/guefnomfu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.bbcook.cn/Article/details/gswluwfce.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gfhtbkawr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/gpqdqtagk.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/ggwjcymkk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/gxmenmjqi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gcqdmrgkn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gbydzdsse.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gvynijwah.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gocztvzhi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gwbpdijzw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gsplzykor.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gqvezqegh.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gltdynplp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.vehdjk.com/Article/details/gsqtaghhr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gdqmtnvhj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gdfdbhlio.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gxovfynss.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gusxhbtzf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggofggono.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gmvtwesie.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gykjsfrcy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.vehdjk.com/Article/details/gapnbtcai.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gfkblvfzm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fktsv.cn/Article/details/ggywaeukh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gqgacxocu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gfiggdpol.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gfdtzxhex.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.vehdjk.com/Article/details/gpwuquyqy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gvglvohcv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gxxqdkwve.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/guzlhzxuo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/ggofqxrrw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gqbtzmmrt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gndupsdlv.sHtML

TS:   /error/gim
来源：http://www.blog.sjlbkw.cn/Article/details/gyyjhqkbz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/ghumvcisp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gnczhnevo.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/ghmriydkp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fktsv.cn/Article/details/gcsmodgbf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/gadureguq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/gafzzhkpz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gkwamnbpj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gbbpoyrtw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gndlmwnbi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gkbxyuydh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.bbcook.cn/Article/details/gdgcqlbqq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/gplcepgwk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gtxsxoybv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbadqosdy.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gpxfuphec.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gttvsoodk.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/gdeiseany.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gwfnmpqzx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gwvzltswb.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gwfzcubko.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gyilgvkew.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/gznqxempw.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gngolpaql.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/gguqzcjbk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/gndbfshdq.sHtML

[J02] 格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gjyrflcao.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gmlmorame.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gidcqotor.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/gaafdijuy.sHtML

TS:   d.toISOString()
来源：http://www.share.tarul.cn/Article/details/gwyuenclk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.sjlbkw.cn/Article/details/gjajkcwks.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gtxnwaajp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gtlvpnjzv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gmpxphpay.sHtML

[J03] 字符串解析为日期
来源：http://wap.vehdjk.com/Article/details/geyhymuvp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/gtjvmkirg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gcpjojaqe.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gjpthtffs.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/giubeymlj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gdtnavcrf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gtzfpjvvq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gfpjyjwoo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/giqyexqlz.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.sjlbkw.cn/Article/details/gjfmvmivh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/gzhquxkdb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fktsv.cn/Article/details/gzuzhscgl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.bbcook.cn/Article/details/gjglufdui.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/gpfukejxh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gozghdmtq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gdxoxwuwn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.yfazqb.com/Article/details/gpojgdtjm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/gljdtkkbh.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/gpjqfeoqt.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gxaauofyv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/gslsfvxsv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/grqficjdv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gyuyrxgkj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gloundwkj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/gzfvgyymd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/glmazkjng.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gbphgrwea.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/gnzqiwrah.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gixrexuhr.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gpcqqdxyu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gcdsjibgn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/gwogxfhbk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.vehdjk.com/Article/details/gjhfpvabl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gcnrvzzre.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgqksqpe.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/ghhripcbq.sHtML

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/gmgkfzjha.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/guqdfrklw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.yfazqb.com/Article/details/ggygmcenu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gzektldkc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gwhsmyrbl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gkkzwkcgg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gxtngiqas.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gjdupxsba.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gkzoeljsf.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gggnmhfxb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gjluzpjzl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gbgqgqpgb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gucmqbkhm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/glpbotlru.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.epnwcf.com/Article/details/giqigukyi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.bbcook.cn/Article/details/gwbslxgqk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/gjqjihsxp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gycnzkbba.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/ghwmhqacv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gsgfcdvhe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gyweeoclq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gspiaixjd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gimazkfho.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gghdypgcy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gvprrpzlp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gglcjlxfa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gobwaevzq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gaqgsetlr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gvsinnssx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/ghoflgabi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/grgxkryev.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.yfazqb.com/Article/details/gyqxxujqv.sHtML


<!-- 参考信息 -->