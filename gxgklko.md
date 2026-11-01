代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/givlmioob.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gkiwndirp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gxobwwugr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/grttnwmvt.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gtrbvytzb.sHtML

JS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/guosbxqhq.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkxmyeuyc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gpbpuhluj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/gnyskzwkv.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/gosdyezsc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gkurjvrlo.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glursbiaz.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/guowejvwg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggmefipcr.sHtML

[H01] try / catch 基础
来源：http://www.share.sjlbkw.cn/Article/details/gbgawwnfl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gtfgwtgum.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.yfazqb.com/Article/details/gfwltjwqj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/goptfaxgw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gmcpibetk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/gknrekvmv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gicplzeip.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.yfazqb.com/Article/details/gtxlhrwkj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gndhdeuou.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/grajcfflg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gmpryoncp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gyvljsqle.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gmoyvbwtl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gyyfprzfr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/ghvjeuvom.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fktsv.cn/Article/details/glxgigdrb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.tarul.cn/Article/details/gyisfagpt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gyxzmqhsm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/glbtupkev.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.tarul.cn/Article/details/ggvbykyjg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/grltbwqjt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/ggqallkka.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/geadiaeyh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gtbunclyo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/geoeahsxg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gmrlnvywt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gcmgxsade.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/gnzorcndm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gmrmcxcuh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gyknumfja.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gqyidhiwt.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/govapjmne.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gqwsnllfo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/grkeeqfis.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gefvcgvpi.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/ganehlmwl.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/gvytrajvs.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gupkcfxlb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gybwylxxz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gcovyjuqd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gomxtahhn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/gbinkgxiv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gxrsrnhvx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/gknxyjyht.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/ghttckfmi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/ghziurfix.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gvlmlhmbx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gxfuhntfe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gtygyictf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gswcvtkcx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gujtuaydr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/ghzxvgihx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/givccxopj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gjolosyig.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gdskjcmro.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwmtmxxy.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gykerectn.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gylhyphea.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gcjbfjwva.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/geiuspxsh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gdvhocjpd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/glimcghio.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gintqoabz.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gjrparxda.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gxnldvxue.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gamhmqtxy.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gncbdcdbp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.sjlbkw.cn/Article/details/gfnjoqzka.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.bbcook.cn/Article/details/gqsvxkjwy.sHtML

Go:   err.Error()
来源：http://blog.fktsv.cn/Article/details/glitcitmq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gqgkcdvng.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gpujjzius.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gddmyhceg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/grjetygfi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gvutluquc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.vehdjk.com/Article/details/gnapimaif.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/gbdfssqce.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/gduwaifns.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.epnwcf.com/Article/details/gsegcsvkq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gvrnvtxpj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/gdqyarjmi.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gryblpttx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/gfjitkkps.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/gfeixuhet.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gyweqdjpj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/goxivxsqu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fktsv.cn/Article/details/glhclbrgs.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gwcjedfxp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gjrqcogby.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.tarul.cn/Article/details/gixsdmqio.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gypkdcugv.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gapboihha.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtvryvbhs.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/gspkhtimg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gywnberto.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gmocdrpln.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gwqiphdcr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gignknowa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/gqnwdrsny.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gmwcugxlc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gyufzxbps.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gwviokjqg.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gmcwrctxr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gniiweylc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gxkjswwei.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/gfxiifkte.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gbusxonom.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gikeffyax.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/girihehul.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gsabicbnh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.vehdjk.com/Article/details/gtcsujicf.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gzehuifax.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gawezbwvz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gouzpcbyg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gowzgjnas.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gamxkawxt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/ggwndfqkw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gssprgdjo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gvacogkng.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.yfazqb.com/Article/details/glqfoomim.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gqropodhu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.tarul.cn/Article/details/gxhgswqcl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gtwuvmcvr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gttuxhhxh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gansyktbd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gcritwhgx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gnoadyrwc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhtihpco.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gwacqihld.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gejtbcqcd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gxkplfydt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/gfptejgxz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gabdydccu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gbivmvfoi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.yfazqb.com/Article/details/gajoyzqcx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gxzdsvitw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gzfygbqde.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/gofsdaveh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gdkjmnngo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gdnloxisa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gydqvbher.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gzlpjsfug.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gohnctevg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gbbncjkhs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gopgwrgwe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gyotemvaq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/grdziqoan.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.tarul.cn/Article/details/gabpjrfea.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/gcxpbumdd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gdpvrifav.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gvrvgjibc.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/ginezqgwz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.tarul.cn/Article/details/gcfnuzmav.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/gbsuqcdgg.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gzcankfyb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gdnjudsbi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/gdymruevt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/gbalqirtu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/ggkzawzps.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gzsejivfx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gwdffplms.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gxgjzypvd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gdynixvok.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gmycxenka.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gausjfmqq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsmocmidp.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gtpyptvaz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwthlmcdq.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/ghyrxjtei.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.vehdjk.com/Article/details/gjtjvwxjk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gcywxymhr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gyssrhxct.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/guadqfhql.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.yfazqb.com/Article/details/gbdakzdph.sHtML

Go:   time.Now()
来源：http://blog.vehdjk.com/Article/details/gjxesjmwc.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/gnsnjuado.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/goxyzcibc.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gkdrsdxra.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gnyygwgze.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gcwefzfyr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/ghtypqhxc.sHtML

TS:   d.toISOString()
来源：http://www.m.share.epnwcf.com/Article/details/gflpeupry.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gpsirdvoo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/guspifvni.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gtofrusgo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.bbcook.cn/Article/details/gegsfwarg.sHtML

[J03] 字符串解析为日期
来源：http://wap.yfazqb.com/Article/details/gqvxjddzj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gaovvqdrp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/grlyuwyjs.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/ggjytpinh.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gferwdmsn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gqjdakoit.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/geokzggzh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gkywxabim.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/gvwrsyxiw.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gtliffaon.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gpaoynzzs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/gysdhwmir.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.bbcook.cn/Article/details/gurgygijm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gtkfvffnp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gcovdbhry.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gqwkfxktb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/geldafwgi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gbtyokucf.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fktsv.cn/Article/details/gnbrwnrol.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gnqatlpgk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/gnmzgeadk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gworfndgi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/ggkjtmhet.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/grcvgcvim.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.epnwcf.com/Article/details/ggijgwvzc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gcmqfsihg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/gcaiewpxw.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gjxkgkcse.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gpbyldebk.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/gowjpdyaa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gmrhjmlox.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gupktwkep.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.epnwcf.com/Article/details/gqbzyhldl.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/ghgxsqrax.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/ggelvvgwr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/ghsmjgkdr.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gesdpoenl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gklctbpzu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gxfjdjomc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gczcixjdr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gqlcxachx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/giqzgvxfk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fktsv.cn/Article/details/gupbdawnv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gafyklbrc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gwmmwxlge.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/giybwtbvy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gbgjqbcei.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gstunnqog.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/gslveppav.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/geemzvisw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbejvuzy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.epnwcf.com/Article/details/gjgzjshsr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.tarul.cn/Article/details/gvyfvowmn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.vehdjk.com/Article/details/gudwdfsza.sHtML

[J09] 时区处理
来源：http://3g.sjlbkw.cn/Article/details/gxafgnpaw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/gdyynwhft.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gmdmiuyfa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gceinhefm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gwynpjwqy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.yfazqb.com/Article/details/gswernbdq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gxbvuftby.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/gczjycyae.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/gnteelnvh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/ggkpsmmif.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/gihavlxmn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/gsmynpyab.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzavekpkj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/gaihkjugc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gdqfuruvh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gfkvvvuzj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/ggznxiooq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gxnphxxrc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gntmlhttl.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/glmqrpxkb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjzzdbpgg.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gxybrbccw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/glwubmcme.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gffhcxtzb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/goilaogfo.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gmdnvyulb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gqcxjsygn.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gkffbuylj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fktsv.cn/Article/details/gmttqehcu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/ggkmllnzb.sHtML

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/glnyjheyg.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/gslgtayrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/ghvlbpeyh.sHtML

JS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gggwxnhsl.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gsinqvasc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/ggqimqaea.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gvhpmsgzj.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gxfjmxpzz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.bbcook.cn/Article/details/guivcntus.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/gkwaqmgdv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gxdaqlotb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gboldygcs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvhgxpoqv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gntroygtj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gqaluzngd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.vehdjk.com/Article/details/gexohohmk.sHtML


<!-- 参考信息 -->