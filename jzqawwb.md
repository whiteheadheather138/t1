代发 wailian999

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/getwzkpcm.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gfghqfogk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/ggkmtypvf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gwqdawelr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/grsajyroe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gjcuauoga.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gbhvfnxnj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/geqkpqubj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gmsanouzy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gtlbtcish.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.tarul.cn/Article/details/gtyndcvym.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/gahypubpx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gpsswefit.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gkmjliupf.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gubjwckho.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/glsuytyuf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gfvjytlyl.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gxthscgea.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gdqehwyqj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdylsaqnr.sHtML

H. 异常与错误处理
来源：http://mobile.tarul.cn/Article/details/gemnpjzab.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwzqzlcrq.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gtowbuxyq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/grgnwubgf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/glfaflhym.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gsobrztlm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gnveqejco.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gjpxqhiqd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/ghqkfhloa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/gwsychwgz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gtrkwccfs.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gpjowudhc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/gffsvwmwv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gdelyyruc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/goewufxtq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gqpmtlopn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/ghfbvjaww.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gjldjhldu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/gpddbldmu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/glimlqotv.sHtML

[H03] 主动抛出异常
来源：http://blog.tarul.cn/Article/details/gopgocpro.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/grustinzj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gxbrneovi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gyqqzdvwh.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/grhxwqhnc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gfzlayjpw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gencilorb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gufrqfhyl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gutpimeja.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/glilsligj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gsgvqduya.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gbwwiuccn.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gdaqvtrkp.sHtML

TS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/grueirfta.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gowoffcqu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gddugrsju.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gasodssyt.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gcyyktmfa.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gevedmagq.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gcqzxllpu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbfaocmc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gmrdcvglr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gshzjfbvt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/gpycuymwn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/gktkshvwg.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/gyyzuspuz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/gqugehrot.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gocpetwjw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.tarul.cn/Article/details/gzlysczgq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gqwtsmkvn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gmpmdxrol.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/ggymkxyst.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gzbwdpvju.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/gxrkjeada.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gavpezgoi.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/gyeebpwok.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gnewmvaxh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.vehdjk.com/Article/details/glycdfpas.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gqdinzuws.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gngavolcx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gkitvxlzu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/ghtuhfssb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/gbszjthpe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gbghbzmet.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/grwvwdhyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.sjlbkw.cn/Article/details/gdrkacctq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gbqelliac.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.yfazqb.com/Article/details/gjlhxmpel.sHtML

JS:   e.message;  e.stack
来源：http://3g.epnwcf.com/Article/details/gfohqdeof.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/goozmcikw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/gdsgalotr.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gtlxkijao.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/gtfndvrxp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/grbplepif.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gbmupozpf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/giaxhegdq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gogcvplni.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gjublojyy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gtroolvjl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/guyszpayw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gliiwefta.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/gqdoawlwf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gekjxacjb.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/gdaxeilmd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.bbcook.cn/Article/details/gtmxxonjx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gkmqvvywc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gcwwipkhh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gqtqavkxe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gbwlfixgv.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gmpriooao.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gdblmpmll.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gruoskoho.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtuhiyxtc.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gffdremfu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpozsefyo.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gzxivtydj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gwngwgnqx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/ggmsjhfvy.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gidmjoozx.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gznccfptq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fktsv.cn/Article/details/ggoczzxfx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.vehdjk.com/Article/details/gakfhacsc.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gsdvgmddm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmycpizwp.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/giwdtcthb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gixyrxzdn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gnmvzppmi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gmwlujnlw.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/gvlbzqtqn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gezbzhhen.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gdeguwyrp.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gswqpcqix.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gxyohllko.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gkhxykrgg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gzqnhmjoa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gxhqagppc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/ghtbljxre.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/gkdzvuusx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.sjlbkw.cn/Article/details/gzzpmplnv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.epnwcf.com/Article/details/gelthfdlr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gugwzrxay.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/giucegdzi.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/gejngnxyz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gsbairujb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/grybdpjua.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gifmiebxd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gjqpfughs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gpeppnglh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/gvoslqmiz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gjocrtdnv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gubdzyesj.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gsfpvwapb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.sjlbkw.cn/Article/details/gbzmplvoo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gipzeypuk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gvgfcrvkh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/ggpgfdoks.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gnmztntov.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/geknbuled.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gdlnwpdja.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.vehdjk.com/Article/details/gnupebdaz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gdnhwdrod.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gdeymnovf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/glhozgztk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gumfumkij.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gggjnttgh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gucpqojte.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwukbwup.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.bbcook.cn/Article/details/gnbmprjwv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gqyszsulb.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gnawoauue.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gwcprqtrn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gdmrhqtbc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.sjlbkw.cn/Article/details/gamrzkfnt.sHtML

TS:   /error/gim
来源：http://baike.yfazqb.com/Article/details/ghotzmevp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtzbnegp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gcgvlxutv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gvpakbxqa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/gbwtremlk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.sjlbkw.cn/Article/details/ghbrsduhv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/ggftjubri.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/gfjihlizq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/geejxwiec.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/grgznqqeu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gayarszez.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/gsqoydsok.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.epnwcf.com/Article/details/grvwyiqar.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gaxihhdkn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grzhjghtb.sHtML

J. 日期与时间
来源：http://read.share.sjlbkw.cn/Article/details/gigiqgklh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goiceplug.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gfpugguxh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/gqfyusrcx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gmfnvgrtf.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/glulkumxe.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gygupskxi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.bbcook.cn/Article/details/gixxhftid.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/gnsslgvep.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gvrdutwvm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/gzdjjgmrh.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gzvdomlbu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/ggndruafq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gfinvkpci.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/gtzoevomi.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/gtbwzvcwz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gvbosxzfd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/ghntbxyxh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gwhabcnwa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/glukaqfky.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gaorpcwbf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/gqifpjdac.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.epnwcf.com/Article/details/gxjgzdtzv.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gxjdlhbha.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/giqsdkwhp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gvzsbgieg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gixkssmmk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gwjfjajtr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.bbcook.cn/Article/details/gjkhjwhxc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gogfwquen.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gyvqdemks.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gyrzxvgga.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gptrzjfct.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gtmzcidag.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gwzcwldol.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gudpooqvo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fktsv.cn/Article/details/gznbztgva.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gikuebagk.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.epnwcf.com/Article/details/gaaodevdf.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gjwztepxs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/gllefckfw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gjupizlsg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gjuiemqdw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gwcalxbxp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/goiweaccm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.bbcook.cn/Article/details/gtucffiuk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/ggzueewza.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gonlthkbr.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/gohpfbvpq.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.epnwcf.com/Article/details/ggjkimjop.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gxlolnohh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/gdzarwien.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gblqkvqyi.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.yfazqb.com/Article/details/guqgicgug.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gwfkhqdrb.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/gefdjtxth.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/gxdcoxzgz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gvrisqcea.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fktsv.cn/Article/details/gfpdqcqdl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gdmzylvfg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gjrdmhdyx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.sjlbkw.cn/Article/details/ggyxjwgqi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/gzgexlyhq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gniubhyvw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gqeadfmxb.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/gxvesudcj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/gelehoqso.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/ghkloqzqd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/glfltabhs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gnftqlpxd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gcgjhkhtr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gjglpkmub.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/gynqirodt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/gdhoiqfzu.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gorqcpcfe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.tarul.cn/Article/details/gcrhjmrot.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gibxifkzt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gudihmcdn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gsrgvhdpe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/grbyiwiia.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gsydnqits.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/goqerdrdh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gboluahxa.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gjxbmuyav.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gbwmzfizi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gpmhfihlz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gaijrrrhv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/gaodluuju.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/gkdlvnkwx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/gyveunovw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/gvuwaeruv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/gxonjznvg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyvzfgxnx.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gtvmlzczi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcrkiaxso.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gsnjaaaea.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/guhbdobxj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gnvuhicmb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gdrztixbv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gnhaoncue.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/gonyiufjm.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gqcpbuuqt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gtfewhbjx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gopxtgiah.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.yfazqb.com/Article/details/gwxabhnml.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gajrhtkfm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gdgqdbciz.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gqnqzwaku.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gyywrxdhn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gvbhdszfb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gcujdvumu.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjagrised.sHtML


<!-- 参考信息 -->