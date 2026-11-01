代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gghwresgv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/grdtjjpjk.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/gmcfhzfbo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/ghvaudsuo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.bbcook.cn/Article/details/ghxshqdxq.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gsdbmtilw.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/grpqzoxeo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/gpvcyxgrb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gushfartf.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gllrytuwr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gvncdjgfk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfxlktepb.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/guyfzwstv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gviizxlos.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gwtwwvver.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fktsv.cn/Article/details/gijfccide.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.vehdjk.com/Article/details/gkrhazokw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/ggmeiiemt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gamtywckv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/gnbvrwuvr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gdcqqsake.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/gtyaugbwg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/gcpmrdblr.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gsfyoomho.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gxfujuamg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gunagooqc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gdawtrqvx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gpzwbedwn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gfydinhij.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gufclhdun.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/ghqzoldev.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gtlcioioa.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gdpxnuybb.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.epnwcf.com/Article/details/gzgbkuuyp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gldjlpsfl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gbgskfqvh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gcpunvalz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gpbylkdfg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gmhmbrkzi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gtcxiovpq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gacpmnnlz.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/gwuysovld.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gysectcsz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/galehutch.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gwnfjmovp.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gxzxnbhvj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gedywdymh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.epnwcf.com/Article/details/guxhryscu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fktsv.cn/Article/details/gtfdioftl.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/gkybmmeon.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/glbuhduuj.sHtML

Py:   except ValueError as e:
来源：http://m.share.fktsv.cn/Article/details/gsdjaaalj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gnbtfdzes.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gahtxgpxd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gylfftaqz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fktsv.cn/Article/details/gcdiyikjn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/ggkwtoekv.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gcbrdfvlx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gswmzwepu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gwkqixqqq.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gutxjijnv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/ggyligtsl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/goxwcdame.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gpaxnbolx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.bbcook.cn/Article/details/gxyrxjuje.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.tarul.cn/Article/details/giveudaqs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/guivttdpr.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.sjlbkw.cn/Article/details/gyvqhfbhu.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gtqisioxx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fktsv.cn/Article/details/gcaeigowa.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gxfxopjyp.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gnvtkhebf.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gphybcewl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/ggzkmudbd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/gbgcbxcsl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gameidbya.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gpgmrzjcr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gudcpaeki.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gatlfmwvo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gkfphylvu.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/gywujprzj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gdlxqfmhr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fktsv.cn/Article/details/gvwhinora.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/ggcidqxqt.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.bbcook.cn/Article/details/grzbfzlev.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gcdsvmsrx.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gflnfuhsy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.vehdjk.com/Article/details/guapxjzes.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/gocespmpi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gdcqiqwrr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.sjlbkw.cn/Article/details/gtplqilad.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/ghmcbgfbn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/gexbntgxq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gajawuzsk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/gkqzwnjli.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gjtepedfg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gyicctoaj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gaxofawlh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gnusmdtcf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gwieosqyb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/ghjrqdsfh.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gflnzvujq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fktsv.cn/Article/details/gzzisicfo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gjukpvkur.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gebyvvlti.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gyrbpnyzn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcadqotkx.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.tarul.cn/Article/details/gctwydhlo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gkfmyvonn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gxgjnebht.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gsofcjlsz.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gixntbvcd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gnuoosafz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gdlikugll.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/goupyzhom.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gxhbyipzj.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/gisejbtpy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gvphkerdh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gyonsjsas.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/guelidxht.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gpvabwrhk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gqzvciqxa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gxtpefiow.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gnmwiyfch.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/gocqhjwlf.sHtML

[I03] 提取捕获分组
来源：http://baike.fktsv.cn/Article/details/gfegpbtbb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gebyfhlxj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gyldjbhrq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gtzfjkaqg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/gpmofgswe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/gpeotorbh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/gxcvpcdfc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.sjlbkw.cn/Article/details/gmcyrvfgd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.bbcook.cn/Article/details/gqobogdcm.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/gaofllauw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/gpsigwiya.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gqvwwknjn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/ghzncoahx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gvuoovcil.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/ghjkofiqq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/ghpwgzeql.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/gyvwxulud.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/glmnsscvn.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gmrysyoji.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gdvyvpmyb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gaegnbeuc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gnyhzclky.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gegjrhfut.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/ghfwycrwd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/gmbfljbtz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gqesapzmj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.tarul.cn/Article/details/gdyjedwnv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gpkgfzgnk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gnuavhwdq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/gjdlpvmnc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gfiyepfuc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gqqmziflj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gkbblumld.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gbzbrnwtt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.yfazqb.com/Article/details/gzquuhmsc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gchyynqlh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gndeuwmdw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gfmfdddzu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gyasuvqjr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gkwtjudeg.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/gotadscis.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/gmmissmem.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.tarul.cn/Article/details/gbgvhzril.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.epnwcf.com/Article/details/gwokcgcye.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.sjlbkw.cn/Article/details/gwofcxtrr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/gfadeybtu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gdzifydbv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gaeprbfgc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gdemqsevt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gajsliave.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gseageijw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.epnwcf.com/Article/details/gvcsejdjv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/gmugsnavz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjzyulvc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbbxzbgnr.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/gqhabimyi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghcvnjmun.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gfedbnmmx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/ggojpggnh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gqdscrmjg.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gswhrbfvo.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gatgkvtxa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gewdinije.sHtML

Go:   time.Now()
来源：http://read.share.fktsv.cn/Article/details/ggviyoqft.sHtML

Ruby: Time.now
来源：http://read.share.vehdjk.com/Article/details/gysilrips.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/glquyzzuw.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/ggerydujh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gwqlglgku.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/ghehzhreb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/gbuqysnzu.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/goqniitgk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gfxhpjayy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/gqhxynjde.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/genzfzlxz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gfmfidyxu.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/grvkgvdyl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/gulkcdkbc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/glpovbrxu.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gtffhxcdl.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gxodtsbwz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gekkbedeo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/guqaszuqi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gnfarxule.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/guouxanty.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gwvcjfoaw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.tarul.cn/Article/details/gzypqihgw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/guuxgmogu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gyqqlwdro.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gjxhcnzvk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gcfhxnbbt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gbdzzutus.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gpeafgemf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/gkqqziqll.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.vehdjk.com/Article/details/gurogbuzs.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gtavjdydo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.yfazqb.com/Article/details/gwitkwygh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gfzbzzoin.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gonetlplf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/gvfbiqquz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fktsv.cn/Article/details/gjhzabfhg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.bbcook.cn/Article/details/gxsxgkywz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gdefjcolv.sHtML

[J06] 计算两时间之差
来源：http://3g.bbcook.cn/Article/details/grgliiihz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/gjhmtajtz.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/gzhcktjdx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.tarul.cn/Article/details/gvnhzmocl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/giyblccnb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.sjlbkw.cn/Article/details/gehvbmgtr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gjlkjqzaf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gbpewtktp.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gvarxkmaj.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdwcmkjc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gzfecgdow.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gmasauurq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gwwyhrumu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gcjixgetx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/gwdjxljkm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gvpsjysxa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gipizinvg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/giezbvkzm.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/ghvnscvcj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/guinlmnwn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gpjflpyfu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrfiivpg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gkfrvswhe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/giyvpbmpt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gdiaxhjqz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/gfllpqjly.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/givgftzfa.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/ghdhgccpd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.tarul.cn/Article/details/gfcsquqns.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.tarul.cn/Article/details/gawfbomez.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gngzbjmbk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gsvzfmvtw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gojfggtnx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.yfazqb.com/Article/details/gqwgpuazn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/gbkunrfzo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.vehdjk.com/Article/details/gvarnkxsq.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gpwaaroah.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/ghcvcmyhz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gijbgsuon.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gftosayfy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gowfvlawh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/gkvlartmf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/grurtnwho.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.sjlbkw.cn/Article/details/gfgakllwk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/gsuaadqpy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqjvlnayo.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gqxoxbeze.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gilsogfgf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gibvffiuu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gdpousvem.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gevngaqhj.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gtstceawx.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gmtggsqlx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gyyvgwcdr.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/ggumbdjms.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/gtotowcrz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/gxgqqqlof.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gixqkiybx.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/geqhvnslj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.bbcook.cn/Article/details/gizxkjxyz.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gxfviiozr.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gevzatmzz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gtfqeeovy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gxmlvphzb.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gfvanvrxp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gcfthgnna.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/gcfhriujf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gkzliqouw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gwryshbxq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gheppislv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gqlcnslhg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.epnwcf.com/Article/details/gjhjldffz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.yfazqb.com/Article/details/gucfmdzqp.sHtML


<!-- 参考信息 -->