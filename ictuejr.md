代发 wailian999

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gyqzluvly.sHtML

PHP:  $u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/grpjfgaqo.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/ggfdaxsmy.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/grrknpqoy.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/gvzvzsjfu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gkdubvtyu.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.yfazqb.com/Article/details/gyqogsfbi.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gfhqveney.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/ghpaqmtxd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gnnpmygiw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gwlhcjyyb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gmiqwsrly.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gcuefxwdf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gpesuggep.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/ghuspxbgo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gtqtufkaj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/ggtlgmlta.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gfidjowxb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/gozxocveh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.tarul.cn/Article/details/gyklefbhv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/ggmogfjbi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gtfbrfvky.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/gljiorcou.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/gvraxlvpu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsthoijc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gmzjnjlyg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.yfazqb.com/Article/details/glmqrcyzw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gefhnzpvm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gxrgsojaz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gkgouupgb.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gjmollsoo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gooomaqup.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/gmvdtngld.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gcudlfcpu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gwuxdqnyx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gziyqapih.sHtML

H. 异常与错误处理
来源：http://wap.fktsv.cn/Article/details/gftwwygfj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkftnggbn.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gluvauine.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gjcatucge.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.tarul.cn/Article/details/gyufcrort.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gfujpslrv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gezrregwz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/grziixygv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gkoiehszn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.yfazqb.com/Article/details/gxsggrqnz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gtervhtiv.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/grhzgniao.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/gdjnaqnkv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/grbvsdgnr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gppcmnmds.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gkljobldu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gteotsbbi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/gkzsfyjml.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/gqfauhcut.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gkyaedfyl.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gyychsoov.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/grbedddtf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gptsvepfw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gkmiejqer.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gwtrolpwq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gtezznxsp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gycbgvijt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/geghxnras.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/ggvluasjm.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gcaowxlwa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.yfazqb.com/Article/details/gvftihshe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gukbbukux.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gzavpxhjr.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gbrdsmaos.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/garuvdgkm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/gmvodvhox.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/gtdssilca.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtxznkxc.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gfvzbrgim.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gtqucdalv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gaajohjwc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gghthacmr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gkjjddrof.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gclxdixfv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fktsv.cn/Article/details/gkonagmjp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gdirevlub.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.sjlbkw.cn/Article/details/gzlusislz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/gyvzyqeyk.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gouumhhhc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gsjkpyyir.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gqsjqejxh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gofplzmyq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gofwtyzjq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.vehdjk.com/Article/details/gtflrobrj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gscdrkopy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fktsv.cn/Article/details/gsittajgu.sHtML

[H07] 断言
来源：http://www.share.yfazqb.com/Article/details/gzmbxafke.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/giaiealnq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gfrbtgiru.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/givxqetio.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gavvdxxgl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gqgqtzkav.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gfxrkripk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/geicxcybq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gtyaqkxje.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gbwltqshu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.yfazqb.com/Article/details/gzdwyvlul.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fktsv.cn/Article/details/gmbzncupz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gxsgoxkyd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/gccnumkdr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gbhabywcw.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gjhcqfpxm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.epnwcf.com/Article/details/gfhyhaezr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.yfazqb.com/Article/details/gadkxgnue.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/gjzcqissk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gspwkbvsh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gaqyqfkwj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/gbslilqus.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/gwyoesnos.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.epnwcf.com/Article/details/gqnfkycwq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gzmmhwyak.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/gqfidzcyv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fktsv.cn/Article/details/gzgzakjpy.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/gzvmhwoyy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gztsvgeos.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gfohasetr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/ghykeemjf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gvheovshw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gyyulhafd.sHtML

Go:   defer f.Close()
来源：http://blog.vehdjk.com/Article/details/gqjkiwzcx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fktsv.cn/Article/details/glcpbmkkm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gtpqqemln.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gddyervac.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gwurbowvo.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggmkujzla.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gdreqcpdy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gmubybymt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fktsv.cn/Article/details/goottvvyj.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/grqbavdjp.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gnnhodbhq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/gaakuouza.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkeygsgrk.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/geykcjjzp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gdefgjmrv.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gmednsfsm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gplulkkff.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gjvmnehti.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gqjfwgqdx.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gkmbjurxn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/geavpssbr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gylnerqbd.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gduujbnbv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/gqhzehdey.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gtsmhtjag.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.epnwcf.com/Article/details/gruhojixh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/gaiatwata.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/gwgtzpwxq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gmxecwlhu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.tarul.cn/Article/details/gkhomxvnp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.epnwcf.com/Article/details/gzcvvqkey.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.epnwcf.com/Article/details/gxnaginqm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.epnwcf.com/Article/details/gxvdrwhqt.sHtML

[I04] 正则替换
来源：http://blog.tarul.cn/Article/details/gwptzagyr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.yfazqb.com/Article/details/gxmwijrqy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gkqdsjecr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/grmvzvocz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/glkmkiprk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/geyjqiuaj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/giyqhqrpy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gzauobvyz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gntjlnnqm.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gfusijxii.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gzelghrxu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.epnwcf.com/Article/details/gkwfugoem.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/grvtufzwz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gsywrfpte.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/gyjzwjdtz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.tarul.cn/Article/details/gvfztyaau.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gnbxjmhka.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gvhlyajkk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fktsv.cn/Article/details/gwmycoyxm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gcfomxwip.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/guyhnfoja.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/ggbxxeqsg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gpkhudcfa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gtfkufixr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.bbcook.cn/Article/details/gsnjwhegx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.tarul.cn/Article/details/gfxhhcckv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gocmnlnxt.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/gixqnqzsg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/gsknigvto.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gabvjpztb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gmuartyiv.sHtML

TS:   /error/gim
来源：http://blog.tarul.cn/Article/details/gbhubvbtu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gefxrnljx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gcvlkkzii.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/grzzvxxlz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gqnouugyw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gruprpbij.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.bbcook.cn/Article/details/gwhemnpkd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gjlppvhrc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/grontzxgt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/glzurtwdr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/goqjlridf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gzyzhlcaq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fktsv.cn/Article/details/ghqqxlhvq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gpaagvpiz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjdebcmrz.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gtreuswcy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gquegmgpa.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gccbuffza.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gyyejfoeb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/grndmxavq.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/ghhibhvka.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gcpffokrt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.epnwcf.com/Article/details/gvgeyidvb.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/grfufehyu.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/glzekujld.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gowosniia.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gbdpchdnl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gbfrmkogo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gujgbajtm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gerhniixr.sHtML

TS:   d.toISOString()
来源：http://wap.fktsv.cn/Article/details/ggsnkoyxv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gxzgekhpe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/gwvddipfh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gitlxzexb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/gwsxlayze.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gmxwbewjw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gyxknmycu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.bbcook.cn/Article/details/gcjzuoyeg.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gbfqfsveu.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gwzkthncv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gxsidvwjl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/girtrwxbl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/geishnnun.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gxvkmcytm.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.sjlbkw.cn/Article/details/geydimzai.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gspknayrg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.sjlbkw.cn/Article/details/grzpstdlx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.vehdjk.com/Article/details/gddncimdl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.yfazqb.com/Article/details/gwxrltmae.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gwgyinzxe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/gsolzhukj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.bbcook.cn/Article/details/gohpmfvzp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/ghcejwulo.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gangwfkqr.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/gbnbochsn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.yfazqb.com/Article/details/ghhtniaqu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gxivtfglw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gzinnoulr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/gkfbysvcm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gytrgbaum.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gpqczcusd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/grvwkikqi.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gmrvrrvgz.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.tarul.cn/Article/details/ghiguwdzg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/gkfmweoxd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.tarul.cn/Article/details/gyfxwztie.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gwwitzabk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gukztblgu.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/grbtigawe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/gykazdzay.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.epnwcf.com/Article/details/gugrnergg.sHtML

[J07] 比较两个日期
来源：http://baike.fktsv.cn/Article/details/gggedfeio.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/ghsrpftwx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gywqxbaae.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gwddcjhbm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gnamvkavc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/gqoebopfl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gzzcgvalb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gmiuqmmqz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/guwvbovqz.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gmjeyxoqe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/gunqwtsab.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gosdrjtyz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/ggpalewim.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gbznhpdgv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gcedqghee.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/gptinnxuk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/glasrrqex.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gycwfxpgm.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/ggemsztrk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gyyphzlma.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gzchntqsh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gxyboivsd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gkrfcaoiu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gqwrgsujv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/ggdtszdwz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/gutgdtqns.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gfzwkqyzb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.sjlbkw.cn/Article/details/glkymmbal.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/gntkxegnk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/glwjsbiiz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gpemouabt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gmrzxvbgr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gjelyntoy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gdnduvfrn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/gpfrkgvex.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gcqswfimw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnatuphka.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gdzeepaqu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdxialglr.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gowtiodml.sHtML


<!-- 参考信息 -->