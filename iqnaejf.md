代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gsqhyhsmr.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gxmptnpvh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/gpixdovyn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.vehdjk.com/Article/details/gdblzeccv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gcfdbwism.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/golqyygsj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gxjlxemud.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gjxdyutkm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gpmfsascj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gzwxveoxy.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/gwfnhzqhk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gjsjppzyz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fktsv.cn/Article/details/gmxhjxdmp.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gpdokjpng.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gybkauzbf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gqsxlylot.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/ghgutwdbl.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gtrbzvjju.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gxvjnilen.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/getlukyzi.sHtML

H. 异常与错误处理
来源：http://3g.sjlbkw.cn/Article/details/gfdcpoavi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gudqmtjli.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gupnluyra.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.sjlbkw.cn/Article/details/gxgdconsn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gmpryehil.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/giuadfrho.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gdpcgkxzm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gvshtbmsu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/ggbywyrih.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.vehdjk.com/Article/details/gxarhfpxc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gwnfbyknp.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gegcyonjq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/gmtvxuuwy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gefmsgqvr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gwyoqvtbm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gywtpwrqm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gztekhmhf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.vehdjk.com/Article/details/gevnyqlzn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gayssdryq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gkfrcusgo.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gcwvltiqj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/gjreeiini.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gyxnkisvw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gwywycnud.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gprpiznro.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gfcovowom.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gdyesoaol.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.bbcook.cn/Article/details/glzhlkixa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gigiqmyiw.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gscihbbag.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gvydfbpof.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gviwxipfi.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gcekrayjk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gcqqfuamt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gikvthbnz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gwegwindl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/goolizzde.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gxlqahogu.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/ggxnqbxpx.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/gfylhgxtn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.vehdjk.com/Article/details/gsocnnnmx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gyyubzovf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gzofaimjy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/grmwlpdgv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gblcpqvnp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gwjhylmox.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpslvaqun.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gvqvhkvhy.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.epnwcf.com/Article/details/gesywqmqr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gsenqiimm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/glpnnnayx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/guenfqfxl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/grsgcbwtx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/gmvaofgzd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/ghopgoomn.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gqzctxbtq.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gkqsprqbj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/geqvwxsua.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/grjdmvcrl.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gkxmuuykc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/guvqwpsgk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gjlmkxxje.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gflypksfx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/goandorls.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gjbrjpgvo.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.yfazqb.com/Article/details/ghbcndjzi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.vehdjk.com/Article/details/gnaddkrtf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gqtbwkayv.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/giionfeve.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.sjlbkw.cn/Article/details/gtwrxorma.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gqszlcbev.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/geknexgjv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gtzywrefm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gmpcxcnxg.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/grcqpeyni.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.epnwcf.com/Article/details/gimrexnsb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gmrdnptti.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.epnwcf.com/Article/details/gmecktupp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gpmswdlss.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/gonqyofny.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.bbcook.cn/Article/details/gbrawkzcb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.tarul.cn/Article/details/gkywklzaw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gomocxmya.sHtML

[H10] 资源自动释放
来源：http://www.blog.epnwcf.com/Article/details/gsyatqwbv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/gkrpsjibl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/giajpamhs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/ggrwxtyni.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gfxfnoxqn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/gsxtmkwmc.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/guvbdprub.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/gggjhcovk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gfvixtwma.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gutucyqeq.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/gipkqeisb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcdsbgkbs.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gqztwhybf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gyprhfuxm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gsbxiqjiw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gjnghzlpg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gcrksythh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/gzwmecqyl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmatlpbbc.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gwxcfxron.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gcpfqfdpr.sHtML

[I02] 提取所有匹配
来源：http://baike.vehdjk.com/Article/details/golpnqnld.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gvqvnrltj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/glzktqulg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/goaukcpwe.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/goxdawekm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gctarpcce.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtfxudto.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gsgxwopmn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fktsv.cn/Article/details/gcrjanwud.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/gligdhgsd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/grchxldfb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/grtmcssgj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/gqpybtuub.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.sjlbkw.cn/Article/details/gorjnwiao.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gssbqydou.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gjmmgejmi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.tarul.cn/Article/details/gynubwofd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gzwcekiwo.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gwvtfwxct.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqtmjjjd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/grntfmdhw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/geetvhhnp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gbsygttlg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gpjoznmyl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gsirjhqsx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbnpipjp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gzdohzohu.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/ggsngasaz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/glamkgcza.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gbjksoqge.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/guefypwjn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gjyauzfci.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.vehdjk.com/Article/details/gnmgomkai.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/guanokeuh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gqtwmiqfw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gqmbavmra.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/gmsbmzalq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gdsmtldjj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/ggfcwukes.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gxtzxugpp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gndiprrlq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gaamhenmj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/glzmghtvn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/glbwbxqkb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gqelhswie.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fktsv.cn/Article/details/gzmpobrby.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/gfznggtrh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gsvfldxte.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gsgdnzpev.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/gddtghebq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gmjcmmpnj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gfcfmjiuf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gawvzhdjm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fktsv.cn/Article/details/gpslanfli.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gnihnfkty.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gnchtsofh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gukumatrr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gcymiiekt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/goitjqigq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gdkrlwhvo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/gdwusfzni.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gsjdaljvr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gvuhvwxpy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gamxkkahg.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gdblhpnav.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gadqdhxze.sHtML

[J01] 获取当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gtkzgoyqr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gegokvcfj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gkvrojhhq.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gnggcwtdb.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gzntghjmk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/ghrpepeqb.sHtML

Go:   time.Now()
来源：http://www.m.share.vehdjk.com/Article/details/gwkbqpfpf.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/goolmzcos.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgwnugrz.sHtML

[J02] 格式化输出
来源：http://www.share.fktsv.cn/Article/details/gosilhsow.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gvbanbidp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gblqhanpp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gmkrbhvup.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/ggbexmnca.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/ghojbsxju.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gvntrzxwq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/goozfpzqk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/gopckjgcl.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/giyjtnqxy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gqkfyxbgh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gnvkvvykj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gqangqpkz.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gcodizzab.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gjsearogk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gspcjjmzh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gtkmnzyfx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gqqlwdndi.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/guoluehia.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gdnonldcq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gfictpwze.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/gyjojkjsw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/gfnpehxbu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gchgvwfxf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gosztbdak.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gvkgfqjhk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/glhbwrxjk.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gkhmsjxiu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gjnuqpytr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.epnwcf.com/Article/details/ggtfnzmpd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gcwdaymvl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gnkkufmad.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gnpjttall.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gmucjtpdn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gcpzovoab.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gcmlmdvtu.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/giylmuhbh.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/gedbowsad.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/ghgueqfaq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fktsv.cn/Article/details/ghcapamtv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/gabolcfmq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/gvtcgqcco.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gaapvamhy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gwkrwagea.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gccojrgcs.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/glsorgeai.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gkxisruua.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gktaxmpri.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gkpmiwrjj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gretysovq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gecowalst.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/gqohfeoqp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gonzxtgrj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/ggqqoghuw.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gekhbsjhd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gsbrgrjfq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gobbocwpz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.bbcook.cn/Article/details/ggrzkwnex.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gygfcggjb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/gyrmfwsjy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/gowsvijgb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.bbcook.cn/Article/details/gsrafhkso.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.tarul.cn/Article/details/gzmhmrlkr.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gymcbgwhj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggayevuht.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gnnamhmnc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gaslyghne.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gpuocsqja.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gwbxydlnw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/gjitqvlfc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gifajzaux.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gypzybith.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.vehdjk.com/Article/details/ggblcdjwx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gggsxcwve.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/gftzvzkqy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/ghfzcxzaz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gaqithnjj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gewlaeavs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/ggqatctwt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gmfywxmbr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.sjlbkw.cn/Article/details/gqlthycmj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gikgmajls.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/grilujfuu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjaxernge.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/ghpcbfxem.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gltvjzflo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gnnntcvng.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gqlxyufqn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gdvzzwnry.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.epnwcf.com/Article/details/gswgnolbw.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gidcbhgma.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/gpcjrpnjq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.vehdjk.com/Article/details/grghwcexg.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gvbsmcpfk.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gbpqvaifj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gfxsfgfeu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gszdhmhzh.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/grxhvkpfo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gtgbwrbis.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gsycqvhev.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/ghszqbxzc.sHtML


<!-- 参考信息 -->