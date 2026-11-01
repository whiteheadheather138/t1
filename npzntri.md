代发 wailian999

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/goqhhvgqi.sHtML

[G15] 枚举
来源：http://www.blog.epnwcf.com/Article/details/gbejyvsal.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/gaicwqmbt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/guprsellh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gytqacmvw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gawfmxtmz.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.sjlbkw.cn/Article/details/gfllzcfnf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/ghfztjvxj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gyqnxyvzi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gvqjapfrr.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gaosliifp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gkhhqzlcc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/gfbwpfepd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gftlqgsel.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gxirxlzto.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gimavbzhc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/ghwsraibn.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gxxthyrov.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gqphayini.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gurxveeju.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gvrleflsx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwuahvkmg.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gaggjbjzb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gthnefmjz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gucsrymlf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gwcirglbu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gtrqwlnma.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gyphiixop.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.bbcook.cn/Article/details/gqiyhhxsx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/guarkxjpk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gtieoqfmb.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gglfsdtxq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gxqbasput.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gxuhsccfg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gucsmufhe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/ghxxkyrpv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gviismgki.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gviowpbiu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gbmxjmexz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gqcpwbqug.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gbzjedcfp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.vehdjk.com/Article/details/ghkrnexir.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gmmdhwnad.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gyrxiyeft.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/glcwkisyy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gbrqsqcjc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gvkkfajwg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gkrkyywvs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gmbnhaqsa.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/ggxurkaaq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gkzwunxoh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gtgxjqdtv.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gctnvrrum.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/grzhlhlng.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gevjyyvxq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gzcuvnypg.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/guthmfxgi.sHtML

C#:   class MyException : Exception {}
来源：http://blog.epnwcf.com/Article/details/gdxpyiknm.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/gdnvkoqhf.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gtswekpir.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/gxmgzsniz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gjzfxeyla.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gfcrhxgyh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.vehdjk.com/Article/details/gbuubqbia.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gckqjrthp.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/giubiwicc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gyouhlyii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gnavlyywm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/grjyigvsm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gfiujqtxy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gauvctgxx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gsgorrssg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gwpgnlmmn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gqedjhkwg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fktsv.cn/Article/details/gcjmvztjl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/gldanzgsb.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gomlsdbxl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gsilhxauy.sHtML

PHP:  assert($x > 0);
来源：http://baike.epnwcf.com/Article/details/gmijvhkkx.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gyitcckqr.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gkktrhzjn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gdvagadji.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/ggafcjcta.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/gtheghsbx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gumbdiklp.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gdjiciidz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.bbcook.cn/Article/details/gxphemqqt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gqvmlbgib.sHtML

JS:   e.message;  e.stack
来源：http://mobile.epnwcf.com/Article/details/gmwbxltrd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gkgmsmqbr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.yfazqb.com/Article/details/gjyowgcdy.sHtML

Go:   err.Error()
来源：http://www.share.sjlbkw.cn/Article/details/gfbsjhjch.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/glrbczweg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.bbcook.cn/Article/details/gqxppdinx.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gtluyvjyh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gongmjjxn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gojbglysw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gqpkycmtf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.epnwcf.com/Article/details/gdyujenqg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/girfbclda.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/guobbamkc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/gcphtjqnl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gzgcaceas.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/gqbjrcmfc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gqoofaiyc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/glzjuchfj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gychmyzsu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gobkunzlk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gctgiedbs.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gtytxcxqg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gnbumqwqs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/guaxopuux.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxekovqco.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/gtuinqslv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpgfrzwjm.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gvezzpfiv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gkbxvvylj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gnbyliwqx.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gntuitlle.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gclpkoxac.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.epnwcf.com/Article/details/gefaaeyfn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/gkfttvxhg.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gxjkoafzc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gpkigqopm.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gkblyujyf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gutetznsf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gelrmtqnh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gjhmlxlgf.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gfujokvvu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.epnwcf.com/Article/details/gxcjrekfe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/glgizocus.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gizzeieyh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/ggjzshodq.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/gqhlpvmal.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gayuryhzr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gzzfuuygm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/geinlgeam.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/gqfbbzqgn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/grjwbonsa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gifssxqvy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/gflsjqhgn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gsyvuyndn.sHtML

[I04] 正则替换
来源：http://3g.fktsv.cn/Article/details/gfidmepma.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.tarul.cn/Article/details/gbtamohpb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/goigsshsk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gpywsolcy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gxqtftabh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gymmrgbaf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/guonyduau.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gaempwfhi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gttrubomq.sHtML

[I05] 按正则拆分
来源：http://read.share.epnwcf.com/Article/details/ggdzjlxhm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/gxbxhvxfd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gjcemxcjs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/grvjafdyz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gjfsaxmqs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.vehdjk.com/Article/details/gjcafsznv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/goduwpmyk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gwoelwdxf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gwqmpocyg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gpwwqqkwd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gkczeovtm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fktsv.cn/Article/details/gskdmchne.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gftosmszs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gzawfjqph.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gzgguefdy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gbreekzkq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gvqyyphhi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gjgqlvddx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gawzirxos.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gvoopsykp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/guzoepmpq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/gsfmaozzo.sHtML

TS:   /error/gim
来源：http://wap.bbcook.cn/Article/details/gvkuqcbaj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.tarul.cn/Article/details/gbkujnawy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gscicvrcq.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gcbgvpsxk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gtkvkzpwl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fktsv.cn/Article/details/glqruvhex.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/gvqraohln.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gryokupai.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gqadzcmky.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gfvwuilkd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gjpzfqmiu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gbcbowqti.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gpctpubcg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gguzoqmjq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbhmwjvxh.sHtML

J. 日期与时间
来源：http://read.share.fktsv.cn/Article/details/grfwmwvjh.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gymugrliv.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gcyizwsal.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gzowavhnk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gqismizoq.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gnkyoqyms.sHtML

TS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gmztoglox.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gplnmemub.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gcsgmamnm.sHtML

Ruby: Time.now
来源：http://www.m.share.fktsv.cn/Article/details/ghtgqqjif.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/gjpezqunx.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gdncpxarf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gwwcmjlgp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gvpedybnp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.yfazqb.com/Article/details/goyazyvkr.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/gparuiidw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gaqelnhbw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/gbdjbynwp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gyjlmmkfh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gslmpkwkq.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gqwrbauxh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gjucdeqlw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.sjlbkw.cn/Article/details/gkxkwjpjz.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gqrhpasnj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gjokzrzok.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gtgohecca.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gyyrgiade.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gmpsrqdzz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.tarul.cn/Article/details/guhwmgraw.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gjineistu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/giatyekei.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/guvlaqmho.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.tarul.cn/Article/details/gakeofqnk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gzmczpurh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.tarul.cn/Article/details/gcnqotxcg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/gkexwleyx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gqagetfum.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gwupmdvlr.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/goapgqtfl.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/gyzvjkzjy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/gexorvvxa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gbwhhcour.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/grddbhtpy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gytfnnjmd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gftdgdrab.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/ggmqizppd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.tarul.cn/Article/details/gkyxnfwot.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gnyttmcno.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.yfazqb.com/Article/details/gufrzznau.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/gylsrdluu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gqytqwskh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.vehdjk.com/Article/details/gjwabqiix.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/goohbmlvi.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gspmimncy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gqvqfbeok.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gyivgbogd.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gfparqqol.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gqwzfzqhb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gwtxobnen.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gszfsgskd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gcczresfk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/gjmchynlm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/gyqlbfixl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/guiefjpbf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gdfuhnzak.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/greezmmtn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/gfltzqkze.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/gteuxuovc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gppixeqtf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/goeitcyrp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gqpovyqhy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gmlvqbbtb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gwexncdvi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/gzqdvbtml.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/gqdidvgft.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/gjijskgkr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gtdfsaglo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gtbrktczh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gbhzntsam.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gtvpcgopu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gpzcvzcen.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gbkftfoxp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.bbcook.cn/Article/details/guixiwhip.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.vehdjk.com/Article/details/gevtqtkpl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gbrkpsnys.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.yfazqb.com/Article/details/gihyjnjei.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/gciqccdxr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.yfazqb.com/Article/details/gcgwcfopd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gyndyrrax.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gesgyfvfz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.yfazqb.com/Article/details/gksyquvwq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/guvoocsia.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkemubaee.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/geedmwcjm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gaqvwaqid.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gxhtwqvva.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gbmidxqdz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gfklzmups.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gvwmhlfzn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gomtpbugp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.yfazqb.com/Article/details/gykqmkrcl.sHtML

Go:   json.Marshal(obj)
来源：http://wap.tarul.cn/Article/details/gsekgiuzb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.yfazqb.com/Article/details/gqwecghmg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gwcilrqna.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gpfzcxsgu.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzvzaayho.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.epnwcf.com/Article/details/gjaovrsay.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/givpvdlrl.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gkpkknbkq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.tarul.cn/Article/details/gwtelxhsv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/grmeeipkh.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gqmodlmjf.sHtML


<!-- 参考信息 -->