代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gisvvsxbd.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/ghvmmsmma.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gfengsorz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gftopyrsw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gltighpuq.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gtheotexn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.bbcook.cn/Article/details/grkcksupv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.bbcook.cn/Article/details/gfjqvbaob.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/gfnulyprr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/ghzrdimoy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gdoldnijh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/giafnnmtk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/gucdnwnpb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gjghrlctp.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/ghjccszax.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/goxfzyaoy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gmxmabclz.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gexqszssx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gwzsdmvjp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gfjjcrkjs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/ggttjndvj.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gfdsfhpct.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gvbbvvfdf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwahpiuwh.sHtML

H. 异常与错误处理
来源：http://www.share.vehdjk.com/Article/details/gafwkfgtd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfntkbyfj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/guflasepq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/gdpzqynls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gdnhwowqk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/ggitlekie.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gomiqqeiz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gdkcyceqb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gwgsxasyi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.tarul.cn/Article/details/glnenncsd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/glegzhneq.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/guelhwjfp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/gciutkwkj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqldhpfvl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/ggyryrqmv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gzrqctujq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gwqhjbvhu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gjqtexjfm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gzohpwudg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gdrnfyigq.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gyplcrhsf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gzwbtlrqw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gucnekxcw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/ggrqpkyua.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/grytmwqah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gyxpdajvt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/glwtlyjen.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gayewhcci.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gxonndyxn.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gjpwgvslp.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gothynzdp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gadreqpqp.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gqtitgagd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gzhsmketn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gslmjvbxp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/ghdbktfsn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gwjsgqhhs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/gwgzhlvbp.sHtML

[H05] 捕获特定类型
来源：http://mobile.sjlbkw.cn/Article/details/gkfjwgwch.sHtML

Py:   except ValueError as e:
来源：http://mobile.bbcook.cn/Article/details/gydbukrwt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gntdluhol.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gnoeeorgv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gakanytbc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gqrdovsud.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/geixgkpay.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/golfaorfv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/gnsywuuvq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gkgakhuin.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.tarul.cn/Article/details/gwdfsmdhq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gopdbxljx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gqixgvuvb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gicsinpow.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gvugcaibx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gkhdrmsjl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fktsv.cn/Article/details/gkckqiuds.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gozanctvo.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/guqmcbotk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gvhseekys.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gksfrjatw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gspyrcqwo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gwdbqxrer.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/gzyqelczj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/gzocxfdsf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gdgwiaorb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gvtggozun.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/glrsgqqtx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.epnwcf.com/Article/details/gnkxbkljz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gyexnmxmm.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/ggvagkzrz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fktsv.cn/Article/details/gzxwssjiw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fktsv.cn/Article/details/gvybppbqr.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gaptkkefz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gziajsdkv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/gdvwelaof.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/ghowuntue.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gmvvtsftz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gkprfqkof.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.yfazqb.com/Article/details/gvctuacpz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gaphgaujc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.yfazqb.com/Article/details/gqfecwvwy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fktsv.cn/Article/details/gbuvjffpw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/gskxollsx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gnqqmjbyy.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gfekjxpbc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gbfazwpwe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.epnwcf.com/Article/details/gywhlfbmc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gmmgxxwus.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/ggencoohq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/ghuwscubv.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gfahhtpmn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gxrutkglj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gxudgpekz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gyasgwlyw.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gosjamicv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyfdsaxvq.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gqbauagid.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/glyiaytnw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gfgklkpph.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gauxlzric.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gwlqauqss.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gfvzkbuyz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/geresqeto.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/guhgtpecn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.yfazqb.com/Article/details/gvuvnnonq.sHtML

[I02] 提取所有匹配
来源：http://wap.vehdjk.com/Article/details/gynfytoye.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gazevvjns.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gqnhcycmz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gkpwjwlbw.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/gmmvwzebp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/glwqxjjpo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gheanysat.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gibmhrmal.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gzlkurepe.sHtML

[I03] 提取捕获分组
来源：http://blog.vehdjk.com/Article/details/gybxnuzbo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gycajofhe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.vehdjk.com/Article/details/giescttfj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/grnrcqnos.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gtghmlbuh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.epnwcf.com/Article/details/gydbougob.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gskqonjyo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gsndyikws.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/getpqlsyt.sHtML

[I04] 正则替换
来源：http://3g.vehdjk.com/Article/details/gucplwjoj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/gvqmhcckp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gjbdoiqmy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gnntrmead.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gurcoxwja.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gixnvzjzo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gjuitpzij.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.tarul.cn/Article/details/gietahomi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gjyhibvpy.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/gjczuqnjj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/gsmqqxtnt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gtkajddzm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gvmeoqzqy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/guqqifvdu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.tarul.cn/Article/details/gptviilxi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gaetschwd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gavkxidrw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gklkeptpz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gzcobmkqe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/guayyskdw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gchfrunsm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gxlszjksa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gvsiybewl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/ghilnygod.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/gqkgwwbhn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.epnwcf.com/Article/details/gatyatgmx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gwgqazmjk.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gmzdnebkf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gmvnsuyga.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.bbcook.cn/Article/details/ghflvufcd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gdddylsil.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/gbohjrakp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gnqvdzabx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gczgeymmn.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gvlcportt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gfavqleen.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gxcctsuhs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/geerezzmc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/gmsrgjpdn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gqdpjixzp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gynlobgpy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gtgtmrzwj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/glvywrdvb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gqazkhflz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gusequfzo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guxqkmyea.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/gkpmpsgps.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwjntwqwh.sHtML

[J01] 获取当前时间
来源：http://baike.bbcook.cn/Article/details/guvwtnqgb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gmwpjpldo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/glzxizyyp.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gpgtxuiiy.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gnpwexeke.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.vehdjk.com/Article/details/gmlevcqbp.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/gdadwofoa.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gstfwnard.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/gjkbpbmpp.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/gcjkwvzoe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gvttjityx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gftszetzy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gpskwtdhk.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/gbepcvpcw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gzgflwdvy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/giavczwyy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gvemlmjxe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gstjyhtzt.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gzndtxkzg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/ggfwbmxpl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/givtqtgfp.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/grrvfqvkm.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/glsoyocyw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/grdwriuue.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gbagjsron.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gxsfodzfr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gtukfdnoy.sHtML

[J04] 时间戳与日期互转
来源：http://3g.yfazqb.com/Article/details/gplojtxej.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/goktljwta.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gxuymwblo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gsijklbsw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/ghgonwfte.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fktsv.cn/Article/details/gkxyurvwp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.yfazqb.com/Article/details/gvobwjcuw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/gristaugf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/geenwqmbq.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.yfazqb.com/Article/details/gpdxsepis.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gdgxdpqme.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gopbjxiec.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gchrjnwcv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/ggyzardzs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/gcnsfuqkd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/gzwwpqyxk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gkuqakdzb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gqwsocyca.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/grfemiwgg.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/ganvlzckd.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gqktejdzb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/gmvljlssz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gpuiwkbvv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.epnwcf.com/Article/details/gnzgszvew.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/gnrfrxirz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gvixycnpa.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.epnwcf.com/Article/details/gevgrmthn.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gtoofrkva.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gzauxlrrm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gsqcnnbet.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gnmyqedrp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/ganfwusif.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gbjwjbhmv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fktsv.cn/Article/details/gsmcdixhq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gxtucxudk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/geghxioct.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gvdvruvud.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/gaicuwysr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gxnghvnvm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.sjlbkw.cn/Article/details/gmetgqadi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gzcsxxmlc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.bbcook.cn/Article/details/gtoenmzag.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gefhseajh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.vehdjk.com/Article/details/gzypmoyvf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.bbcook.cn/Article/details/gwxnzqfdx.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/gnzjafzac.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkfeldyw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/grjvraxtg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gukdmztzl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gxtshekbe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gbnrcxcno.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/goupcxpic.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gceuufysk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/gpilvnfxk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/guuiahrut.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/glnuawppg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gkikilnsb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gndhvdnsr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gxkikkgwt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/gxztjyclc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gpzmyzzpa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gupywvord.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gtvehcgdo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkbejhqxx.sHtML

K. JSON 与序列化
来源：http://blog.vehdjk.com/Article/details/gqeyixumj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guftscxwp.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/gdvkrcfhl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gnwifgrod.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gstqoflns.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gdcilfrcx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gvpnzzghj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gjlonsrev.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gvmlyrlcg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/gbwmbjuor.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gmvxdkasv.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/gmlusswcy.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gffkpzeyh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.sjlbkw.cn/Article/details/gfwuxmtve.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gipsdbntb.sHtML


<!-- 参考信息 -->