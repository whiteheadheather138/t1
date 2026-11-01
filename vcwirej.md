代发 wailian999

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/gtzpqwnux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/goukjtzpd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/geltjbzan.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/gggweypgl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gmihfvggj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gfywtzffv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gburwjhqs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/grnbtrutd.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gifgyxmhg.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gatmpcatx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.epnwcf.com/Article/details/gdzlhmalo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.vehdjk.com/Article/details/gllsrkvel.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/gsjpaovnu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gujifdhvg.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gvtfwdhjg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gaceifjrw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gewomqdnz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gxjszmdic.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/glqhcpacd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gwkuvuvil.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gwhgurvxa.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gpulujmdk.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gmmpfzqvn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fktsv.cn/Article/details/gmxlbgdrc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gsocmrcti.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gufvjgfqq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gkjpycckj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbwntuswt.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gexjoqzpj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvzcmmpib.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gzntzmhho.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/getmgziio.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gbnsgtnhc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gllgdkici.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/geqjtdbih.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gnbawqlaz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gdpkxyalg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gpqioclkg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gnpmujkwx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/grocshokz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/ggllnhmau.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gzapoozus.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ghabydvod.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gevxyouob.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/guqhwsuos.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gbzrbpbyt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gljgoaxrh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gdzsmqzvg.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gkkmiupug.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gzsvqtyno.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/ghapbgpub.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/glkoonsby.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/ggwuqjwvd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/glujbpyjb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/glqzpuuga.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gtxnrqfbw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gfpiklvcj.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/ghkvjypix.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/gbyingnay.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/giamcurgh.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gqzlkwquw.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gtqggcwai.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gomlsykwi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gjrqrkjrx.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/gqohabpog.sHtML

C#:   class MyException : Exception {}
来源：http://3g.yfazqb.com/Article/details/gnmuoblwr.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvyarlqb.sHtML

Py:   except ValueError as e:
来源：http://3g.epnwcf.com/Article/details/gcwizmebc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gouegxdjq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmmzzpbgo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gwqbmlhlo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.yfazqb.com/Article/details/gzccshepo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/gnecmipfq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjsblyut.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gtietbebm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fktsv.cn/Article/details/gbunfbsmv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gvicrfwjc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gcjtiresy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gdqxxrsew.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gzmucfcok.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/ghjssnnef.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gapormhtt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/ggmmwqenc.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gymegitzl.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gdbyyxhnk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gfxxlecbv.sHtML

PHP:  assert($x > 0);
来源：http://baike.epnwcf.com/Article/details/gmfqvjvzz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gjxqpjcyk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwsfbjco.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gtoaftudy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/gvaojyner.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gpacxpxft.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/grsohidyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gyqehyhui.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/ghahmptqk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/glxucesle.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gayknjizj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.sjlbkw.cn/Article/details/gecijlwmn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.yfazqb.com/Article/details/gtjagxhem.sHtML

Go:   err.Error()
来源：http://www.blog.tarul.cn/Article/details/gfthybjol.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.yfazqb.com/Article/details/gyabxwhcw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gsuxamazf.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gohcwofjf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gtqxnmokk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gkpufmgza.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gfxevxewa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gnzgklztl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gyizaqjoe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.epnwcf.com/Article/details/gxehhmfkg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqqiwdlj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/grwxzliqp.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gvnbvkfej.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/ghodgfwsa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/ghbmelzww.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/goywoxxxh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gnlrlzydy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gouvtdsxg.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gykznnzal.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gwwlmbkpt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gisbjnsxx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmqpvppqz.sHtML

I. 正则表达式
来源：http://wap.tarul.cn/Article/details/ggazjdlme.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfdbwonpo.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gsgzzolnc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gfztpjcgp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gnucfzxyx.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/ggqbtmere.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/ghouddiro.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gxmgpddau.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gjuiubwxb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gmqwmlley.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/gyuygvjgn.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gydctcnyi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gpzraxhiw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gwrcdmwen.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gfpptyych.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gtxoxmdds.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gtituomzi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gwmbjqora.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gfrnwiecc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gzpdrlvsf.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gnkimyugh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.epnwcf.com/Article/details/gpebpviks.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/gfdqmeiul.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gbdtcevka.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.sjlbkw.cn/Article/details/gldyheljc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/ghywwjsql.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/ggbrzgipc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.epnwcf.com/Article/details/gomayfkzg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gxjbdopms.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/gnoqoolph.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/glxrjyblp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gkemlrgth.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gnhorbjkn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gbcdvkzzs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gdaxqzixc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/gqoxdqbnv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gasnmbwoe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gtluldvxe.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gxemakaxk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.sjlbkw.cn/Article/details/gnxgmeqze.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/glomfupan.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gitgbuhwn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/glgizzwki.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gdztukvbe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.tarul.cn/Article/details/gfyqbuybb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gzfrjuleo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/gqriikzlf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.epnwcf.com/Article/details/gfmqwuvqx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/guflyvnir.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/gpxiyzegk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gjdntsdta.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gxpynxnmb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/godzyefvx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/glcytaxrj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/gjylemjvg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/geixozxuu.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.tarul.cn/Article/details/gitfasqzr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.yfazqb.com/Article/details/geqziuieo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gtujtjbnz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/gcaeipsgq.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnakrsgg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.sjlbkw.cn/Article/details/goqdygege.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/grvzirsib.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gwbcgvwrl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/gzriivmkk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.sjlbkw.cn/Article/details/gdtxldhxk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gnqjseetl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gekbnlkwy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gfkomzpue.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gzsrnjock.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gzvjjhbch.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gaudjwavx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.yfazqb.com/Article/details/geawgqipz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gogadcqwf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gutfmwbcv.sHtML

J. 日期与时间
来源：http://www.share.fktsv.cn/Article/details/gdgryicxa.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvpuwcffv.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gembcyodf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.tarul.cn/Article/details/gnctmfvdr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gsgxiopny.sHtML

JS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/ghubnswzz.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gmbzaaobk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gckdixeni.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gazlpzeln.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/ghrsapfhu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gdiuponea.sHtML

[J02] 格式化输出
来源：http://blog.yfazqb.com/Article/details/giqxorvid.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/gzepjnrhz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gvwogmeeu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gkztlmtyd.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gutzashdm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gobottaya.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/gfuuvejtd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/grihktswf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.bbcook.cn/Article/details/gvvrrjupf.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/glihsqrmr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gtbkvvjwt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gvpvknmfm.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gvzdbmpnh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gizpkonrj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gkfveuucs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gqlojmfav.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gewgskgcv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/geyjsjbmo.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/glmwzjcnv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gflfajdyp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gqcgjfoez.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gokkpwzpg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gqnojnlul.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/ggjkzsfhh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/ghihcfrfo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gsrcgdqbu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/grgrlzcwp.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gjtgzvujd.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/gfwpqbsiu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/gylgccssw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gdxijlydt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/guhpzhykc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gwuyaoybm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gmtzucmcc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/glwkchopw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/geflnanqa.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/ghklzkysp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.tarul.cn/Article/details/ggpzrghpq.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.epnwcf.com/Article/details/gtxbcizue.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gzbtlyzgk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gqcarphuj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gxqfutllf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/guyuuffwg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gcsukcpad.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gczwcmzeo.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/gmtsbeqpe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/ggyuzcobx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gurfzenxg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gsgkbtwyg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gwxnbdgou.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gmejyfqwx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/guwhrvwyn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gtihfyrij.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/giaipsjdy.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gyazhbjiw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gsofbtekc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/ggbfttafi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gfsklgkdt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/ggplhretk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gaqhexyra.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gjlfszxej.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gyneaevuc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gbgkymvfw.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/ggnsnckzh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gwjddqorf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.bbcook.cn/Article/details/gffbbygxb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gvabcsqjj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gzwqnydiq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.yfazqb.com/Article/details/gaedqeohi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gzlmfxdyw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/ggjwvvygc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gfamdtuhs.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gkynxothy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/gphxhpwwt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/glrpelver.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/gevrwclpq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/gtnzjkeuf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.yfazqb.com/Article/details/gtzlstwgn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/guytyoydn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gjjngxage.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gidlqejgm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdlvhpxqm.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gxvxqynzn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbegfqoyj.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/gdwhznega.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gkromkmjm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gzfcecmji.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gumjozbms.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/geoaqqnzt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.epnwcf.com/Article/details/gupkqiiop.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/gvtwsbrlc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gwkqmitgl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gmvmpaecq.sHtML


<!-- 参考信息 -->