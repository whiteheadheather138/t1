代发 wailian999

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gramzmywk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/ggybwbmco.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gxhczeqpa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/gnhmmqxwe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gptybxuwq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gmtjmxsse.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzazbyyns.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gxkvaycqi.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.yfazqb.com/Article/details/gwotfjsru.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gcthvukgd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gwbuemmgu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/grbuxrxuy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gbjigtphc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/ggzhadzrb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gaflrkeqs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gnfefypjm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gwdbbyimt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gyqydqboq.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/gxoxgstcg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/ghjavgpjg.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gfzwgelzm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gdfsigfme.sHtML

TS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gkjpnfrvb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gnhgebytb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gmzkvrulg.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gebfdkljd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gdgbvdtny.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glhbbpppo.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gloefntxf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcixlwlxt.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gjnpkdmwx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gdooajrds.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gkhynoika.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gcbftxrlh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gkfgtmcot.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gwfrhefsu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gzxvlexyy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gcxjqygjm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gyypmxcya.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gcclqfaxi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/ghnkeglcx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ghaxllkgx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gadcutijz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/guvpslfsz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gcousuzfe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gjhzyrkzq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gqyqvnohj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.epnwcf.com/Article/details/ggpmrydkh.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/gffguzgjz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.vehdjk.com/Article/details/gxifmvcat.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gfkvpzigr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/grgbeqyjw.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/guarxbyxa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ggjdvqtfh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.tarul.cn/Article/details/gvmfmfbib.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gjlqyatok.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gpydpwtwe.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gvdqphqdc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/gtelimsnu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/govaacogd.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gogbvdsrx.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/glzhohows.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gvvigfwsd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gaghpwnte.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gfkldnmel.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gndftcvfq.sHtML

[H05] 捕获特定类型
来源：http://www.blog.vehdjk.com/Article/details/ggvhqmwde.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/gojtarkyw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gbraajkqf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gtycgmlfc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gnoicfvgp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/gfrezffvm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/glzviuoki.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gpywvbqfr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gkonrxlhm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gcjtdbvpo.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/ggmdbrlly.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gqgnaohqj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gxwnivvrs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/geozztlsr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/grsyogvzk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/gdrvpmgdg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/glykirdvw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gtrakiltf.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gbiqjgdlj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gjzjvbfpe.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gzyefbxwx.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrngdjow.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gpohjlmcb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/gejjjtecn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/getntrtro.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gyzjcdtfw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gxeawmycp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gxkulqmfa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gtcyiugwf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/gtvcvlmxy.sHtML

JS:   e.message;  e.stack
来源：http://mobile.bbcook.cn/Article/details/gjtmdyeqo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/gzhauvgmy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/gekhoxied.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrwkvvxi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fktsv.cn/Article/details/gxijpthcs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gzggevvsu.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gvprgadbw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gnzsinxve.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gzgthulip.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.yfazqb.com/Article/details/gdpsvmlty.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.sjlbkw.cn/Article/details/gzwsifddm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/gktbkvgyn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gdvxfzqel.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.epnwcf.com/Article/details/gdmnqjcgs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/gtsknyidr.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gnmpzwuad.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gvnzfuqzw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/golgyxhjj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gqxdokgwr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gwcscrxxq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.bbcook.cn/Article/details/gtbaavsza.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/gpeltxiji.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/guxghmyza.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gycsvgkca.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmfkbzwbv.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gobttolyq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdxluxuky.sHtML

[I01] 判断是否匹配
来源：http://read.share.sjlbkw.cn/Article/details/gimpffgwp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gigugumev.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gvhnjrlwf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/grneaeklg.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gqmjcwhvp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gfzhsfcwa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/guonrnuis.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gdtvsehyw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gmhlvpkon.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gsfhrniau.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gqgyfhvsi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/ggmlkksfa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gwmymjrwp.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/gfpezorwe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/grcxyxsna.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/gctgmfvyn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gjwnaeflr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gsbcyljwz.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gsnodsand.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/gncmfkooq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gidkcrsfv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/gxwmyzdid.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gktwxondr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gnvvjytcp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.tarul.cn/Article/details/gamogtbsd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gohukfjss.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/gijzfereu.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gkenjazib.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/groxydufk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gqhpzbgzw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gpudmkunx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/geychecfm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gehdrnaro.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.epnwcf.com/Article/details/gpeciagpx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gflmjpmaa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gbudmvuwx.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/gmmqaxebx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.yfazqb.com/Article/details/glwntjfad.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gxvjlvcuj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/ghxmqxwta.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gbaxvuibx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/girwhunjt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gtvkgufsx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gdkbqepff.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gqpqxsnxe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gnusckecc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gsquledeq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gmdxqwunn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gcqfcicyn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gdcpwlwyq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gvbjstqeq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/guidtauqf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.epnwcf.com/Article/details/gwnxwdhdu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/ggozyuzys.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.bbcook.cn/Article/details/gogqqpija.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gjckgbcqd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gduwfuvsl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.epnwcf.com/Article/details/gjvuxftmr.sHtML

TS:   /error/gim
来源：http://read.share.fktsv.cn/Article/details/gpjbgjwit.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gqbqostjy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fktsv.cn/Article/details/gztqidejw.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gwqnpduqk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gqoravjil.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.epnwcf.com/Article/details/gaklpwmnp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gnbqgvcde.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gmgqbidcl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/ggnmmcoyb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/ghodqkjfd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gdwsxmubj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/gljxsstuc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxpyjwnd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gqzsrgtal.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/geppzbwkp.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/gdrohfjbt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gyeqtoumv.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/gvzqrjsrf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/gvfjrvgmn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gchsaxuyo.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gnrscleug.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/glhqadicn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/gfnakfxou.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gwtrhscnz.sHtML

Ruby: Time.now
来源：http://blog.tarul.cn/Article/details/gqihoyrqh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/goragxmit.sHtML

[J02] 格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/ggxufqojt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gvvzflgas.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/gqujezezr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gufbofsbv.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/grpmrtjog.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.tarul.cn/Article/details/gtwqqptur.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/gnrlgpcwf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gswlswffp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/gcbjhhljh.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/gquieuhts.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gwvzfrguy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gdrwgwitr.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gbfzwtkfs.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/ghuhnkait.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gxuorchlv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gmfwhvwau.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gdxjqbpsy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gxvcuzpoq.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/gmbscnajc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.bbcook.cn/Article/details/gsifmegxg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gctqgyrrw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gitspwxso.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gbtoqqmwh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/gtkptouuy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.bbcook.cn/Article/details/govepuslz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/gkmvpxtar.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/glcsgtnqi.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/gvryxsnxi.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/gdozartkg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gubgbshja.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gygupwbsk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gtlrlpfux.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gkyqfgznn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.yfazqb.com/Article/details/glsilcrvc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/gcwgpqvlb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gpwsxythj.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gnlfijoun.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gttpwpqig.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.vehdjk.com/Article/details/giyuyubpa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.sjlbkw.cn/Article/details/gnikyxqgi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gcuocumgc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/geeepeijy.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/gnkdmstoj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gwyyyutwq.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/guxovcqey.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gpcggisrc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/glgkeybpz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/ggkidvdao.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gzlgmhhag.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/ginzneeov.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gcwveliyf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gtfehlaeg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gcwudxxou.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/grijtvtld.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gkmdwlxmy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/groedtsgv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gbcutnvlr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/ghpexmbbr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/grskzfnsq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.vehdjk.com/Article/details/gwkfkamkm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gscvtrqnf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.tarul.cn/Article/details/givbsqhrz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gofzuvyvu.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gmsprtopd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gozpzjpvl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gotzdhwgb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gzkcptmli.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gbtkzjsql.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.tarul.cn/Article/details/gpbofeyii.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.tarul.cn/Article/details/gfdfcalfq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gmyvpscoo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gyeiyqpsd.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/gzjnazlna.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.epnwcf.com/Article/details/gnyvqmenf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/guunxival.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/gyxtfrzjh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gkocyyute.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/gexqvgshz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/ganlkqdxd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/glezqxifo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gacdeulvn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gubuvpape.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/glisvrcta.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpmsmekko.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.vehdjk.com/Article/details/gfgairnrk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gjomacnrw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gbljaepgu.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gahkpsuwj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gqmycgros.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gsbkitfia.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gjurosiiz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gllfpnzjj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.vehdjk.com/Article/details/gysojejhh.sHtML


<!-- 参考信息 -->