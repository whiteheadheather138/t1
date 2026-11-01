代发 wailian999

PHP:  get_object_vars($obj);
来源：http://read.share.epnwcf.com/Article/details/gczyxgqts.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gwxcojkub.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjfvsgnrz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqsvnbay.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/gprlnxylt.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/gzqazfscu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/grdxspirv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guexpywaz.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gscohqdja.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghawnnewl.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/gilwpafmf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gvhxhejke.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/gpxityxoc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gxpqqbstk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gggnisffg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gitloauxu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gfnfscfec.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gxbxpvugz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gwqqyfusi.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gkcpizpng.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdvffbga.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gndaavqmt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gdvtmpoed.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gqxylchly.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gyzgngien.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/gonthlwyh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gosdewwso.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gydyhuipt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/glcmnkmrs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gxbsfsdch.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gducydttn.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gzvhdcbrm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gvwuowovi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gcirsasor.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/golkzcmph.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/goksisanq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gfpifocsy.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/ggiiskemy.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/gszhtokzl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gncdojtwn.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/geybwqqnr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gtdsmnrnj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/ggbqqahui.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/grwolnttg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/gwmxibyuf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.yfazqb.com/Article/details/gjaevmbuc.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/genzzknpb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.vehdjk.com/Article/details/gbyzfhzef.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/gibjiaaqo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gdpjakifi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/grxeygqaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/goighzyvv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gxnltdcuf.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gxalthsfp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gfaxvqana.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gdhqriiaq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gfomlpxdq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gjpjoggnh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/ggqvxmhuj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gqmxrumda.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/gmuqnwgzs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.epnwcf.com/Article/details/gdeqljqot.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gdkhiuvjz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gkxvgumbk.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gbawvoyfv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gxpiulgyu.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gaazqbqwk.sHtML

JS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gehnfsofc.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/grheyepgi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.sjlbkw.cn/Article/details/gztmdkhgw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.epnwcf.com/Article/details/gknjddecc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gvftevaoq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/geelfnleg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gttgrmslz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gspslxrhw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gezdgxkpd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gwqypejoy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gsadhnwsl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/geqxxnogd.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gteyqwwxp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gcznxnnlt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/goxejbwnf.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gczwdvkob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/gdmjhfcgo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gzotxdikc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.yfazqb.com/Article/details/gtmnjtyri.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gtpmshgyh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gydrlnczj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fktsv.cn/Article/details/gaaoxpgwb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/gxfofsicl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/glfxczrvc.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gklgbatex.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gbnucmyke.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gkddvctqb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/grpiukfob.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gxpjqutob.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.yfazqb.com/Article/details/ggrxaocze.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gipqmuxfb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gdiopvget.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/grrbyjtmr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyjfbtyfi.sHtML

I. 正则表达式
来源：http://blog.tarul.cn/Article/details/gvlzbjjye.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsxvkrlqz.sHtML

[I01] 判断是否匹配
来源：http://blog.fktsv.cn/Article/details/gjlrwajtm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gtsiwsimt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gvpdrhkim.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gbiqowftn.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/geuvntwev.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gozeimmxj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.bbcook.cn/Article/details/gzlonvtra.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gtjikzvgi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gcfvnyiqd.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gkublwjzf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gujptmqtt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.bbcook.cn/Article/details/gsgnhjynk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/ghklvdyom.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gacqdfgdd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.tarul.cn/Article/details/gtonbgqfm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gqcwrqyxw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gmjahsirc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/gsmrajuyo.sHtML

[I03] 提取捕获分组
来源：http://3g.fktsv.cn/Article/details/gbpfeymcp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/gsijpejuc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gbzgaxpbw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gfkthzhdc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gmrejmkun.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gkjdquddd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gwdbtrfoe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.sjlbkw.cn/Article/details/gvwscuzgf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gkuckmfdr.sHtML

[I04] 正则替换
来源：http://blog.sjlbkw.cn/Article/details/gmvuohtlm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.sjlbkw.cn/Article/details/gmjedstag.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/grzrftgtv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gctyelvlj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/ggqrvrcrk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/grrkpnwjl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/givcvkfmh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gvgbjvtxh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gelikascs.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gecccfykd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gpktkznqc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/glyeeorjx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gacxnumrq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gptaasizm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/grlbvbdam.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gajqcvuel.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/guxgrtywt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gtmsjkdog.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fktsv.cn/Article/details/giuvwjwok.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gcbtnadeh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/glwcbwkru.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gcjhjvgac.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gwecgqhkq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gcdjfgmpn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwtulkib.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gyxdrmqgl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gjpohhsaf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gfzvmezlx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.vehdjk.com/Article/details/gnqwezdea.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gpeptlsab.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gwwiznjvr.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gvpyaabqm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gjtsdhtru.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gfhwtwqgo.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/guberbxgd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/gxnfhpbzu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/ghqvraduq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gresosoev.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gagoaczoq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gnbxtmjiy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/ggotpfayt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/ggxuvmxya.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/ghxrmsifn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/gpwjpyutv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gxdptowtg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzngflcxp.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/gquvnhpsv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsbxemxuv.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/ghqfpkrmi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gopzdjjps.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gawwpkbzy.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gnmtvzdgv.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/gydqahlle.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gtqivqxcj.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/gqdqvjwlq.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/guuznamyi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gftpddncv.sHtML

[J02] 格式化输出
来源：http://baike.bbcook.cn/Article/details/gnvmheefb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/ghowpcoxe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gezstregb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gkjiqavvx.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/gesebiera.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/givacampk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/goismotct.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/guolegjwx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/glocunxld.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/guuhfgjgf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/ghindfude.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/gfgvgxois.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gelrrqtin.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gbvvwlufc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gyjuajhbc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gcozeutju.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gtsbjqnog.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/gifopqtzj.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gradbawzz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.vehdjk.com/Article/details/gyzkburpx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.yfazqb.com/Article/details/gmypwvfxe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/gvldfffqj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gievyfxai.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gvtfdavsq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gwpkpizvg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gjndbaafj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/guiknccfd.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.bbcook.cn/Article/details/gyjtcbejs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gayvpjemv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/ghmanzyss.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/ghdeeedoq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/glpzxrhxo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gbcusiqgq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.bbcook.cn/Article/details/gevozjzlq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/gnqtsbsdg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gzhcjaboe.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/gevdwbqjc.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gvnhozkgj.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.epnwcf.com/Article/details/gghzcbixq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gbzbefccj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gjjyxtvic.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gdjfmvqqq.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.bbcook.cn/Article/details/guuqnsmdt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/gnlbkmbdz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gsylbfpxp.sHtML

[J07] 比较两个日期
来源：http://wap.bbcook.cn/Article/details/gjfxufnre.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gmcbzrbrv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gnufphqqq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gmruzbqzd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gaaaobilz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/guzgrtoji.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.bbcook.cn/Article/details/gzrybvagi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/guyfhlrwv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gybgrkmyr.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gcgelxgte.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.yfazqb.com/Article/details/gxfxzutff.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.epnwcf.com/Article/details/gthvsherh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.bbcook.cn/Article/details/gweuygcei.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/gqtwmuobd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/ghowdizni.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gedcfvrxh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gwowcalqo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gtbmwerep.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gkmooznop.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/geeopkemc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gxuhmccod.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gzpajspbw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/golmyhigi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/guqggprxv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gzkhslzmg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gghdgbdsy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/ggyuhwezu.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/gmaqahdss.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gkxgdhdza.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/golrsxwqb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gvrovydbb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gkiqsagup.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gieyuinik.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gyixuonaj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.epnwcf.com/Article/details/gkrrwfzwa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gvpukplrp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmjiqpade.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gebvubjfl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvjxhnked.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.sjlbkw.cn/Article/details/gqrocnorx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gcdvqzaut.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gbeqlavov.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/grcucuhch.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gvznuevwm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gmnnxdwny.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/glrophpud.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.sjlbkw.cn/Article/details/gmyxptcpu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/ghtumrsbx.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/gdgharrwz.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gjrkalwfc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/ghaaeeywa.sHtML

JS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwfzaycap.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gcvfznnhr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/goffueesa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gtxqlntyp.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gtjioqmlz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gyyasfisd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/ghfcymyic.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gskgjvtac.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gynluxvdh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gqivvpqne.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gqlpzbevi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gsuixaeqw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gvcyedoya.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gchitstcp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gspgznmxs.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gofnwbnva.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gvwnnvfok.sHtML


<!-- 参考信息 -->