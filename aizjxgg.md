代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gxtrtncfi.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/grtfrqieq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/grjslbzrm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/guapgbmoc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gjgafppxt.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/ghaixuuys.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/gjcxqryir.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.epnwcf.com/Article/details/givnfqdix.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.sjlbkw.cn/Article/details/gdanmghsh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gfwzxijno.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/ggedhditr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gjwqtcqmm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/gibbzrytz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gqditzoav.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/gyedmqnzx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/ggxhrultr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/gvwpakjjw.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gdbjgdbpa.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gthyfhure.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gzplhvhtv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gfjnegojw.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gmdhsnhmj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gunvydahw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gujtjvbbr.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/gzyhazzar.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsthdjdsx.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/giaptiayh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/goozdcini.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/goccdffek.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/geqbpsfww.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gieurvuhv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gagmyfohv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.tarul.cn/Article/details/gmsdhwypm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.epnwcf.com/Article/details/gvgiavujp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.yfazqb.com/Article/details/gygcavuft.sHtML

[H02] finally / ensure 收尾
来源：http://blog.sjlbkw.cn/Article/details/glqjoobmi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gnubborfk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gyrtbhohh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gwvtuaeyc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/guyzffzgz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ghpcdgstv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/gfjrsjsye.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gqdkuwxvk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gcpcrbevg.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gcoumsald.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gjnqwbsda.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gushppdtq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gkcxqwswt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gxcddgcjc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/ghindvrnr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gwwkitkua.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.vehdjk.com/Article/details/gmuyeoupx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gefeteosv.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gbzronfaq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gfpgepqxq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gxwavuqhc.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gxtgsjbnd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gwhzbbaxq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gytkkopkc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gqgonmueo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gggnfvygz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/gnpwpmdkc.sHtML

[H05] 捕获特定类型
来源：http://3g.fktsv.cn/Article/details/gmncrrozu.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gargbeafq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/gojdwboir.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gnpfudhkd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gboqukgki.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gusveuilq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/gddeexatd.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gvxvqkxju.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/groiyaocc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gnxavpcem.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/ghxtlxknz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gxxglbyau.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gctblubyd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gvmvzzcjq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.sjlbkw.cn/Article/details/gdrkhvwyp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gtvfoulji.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/gzdvnhwbe.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/ghtquvcla.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/grreplnyt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gemnntwst.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gigglnmhy.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gijwmhflw.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gptqxjfda.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gcbbjjrhr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/guoqoyhjw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.tarul.cn/Article/details/gbqderegu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gghchigpb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/gdwcgaxat.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/gpoaujbii.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/gekexwdlr.sHtML

JS:   e.message;  e.stack
来源：http://wap.vehdjk.com/Article/details/gqwkhgfyo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gistbyhlw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/gwayfdclh.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gstyjcbne.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/gtiegenrt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.vehdjk.com/Article/details/gtmitxvsk.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gqcujmnea.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gnxtwiyxz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/galzkucom.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/ggtgklvia.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/giucjijyx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gmjkhzaij.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/ggahabvof.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/gljlvpcmp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gpmvppyez.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gafynptid.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gbpjsyicz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.yfazqb.com/Article/details/gimwstada.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gjmyymlat.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gfddqumyt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/ghjszmzhb.sHtML

Go:   defer f.Close()
来源：http://mobile.yfazqb.com/Article/details/ghnlwwveh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gfwyspnpt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gwespidub.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkkkkweta.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gsalkktny.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gukuceyia.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gdxgiwpgx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdvgotupr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gomqekdum.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gqnhrismw.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtftrzkvx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/ghctsgzxk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.bbcook.cn/Article/details/gwgxxrnjz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gwveivyyr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/ghcsiiggr.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gjrqjmizn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gcvjnxhej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gysonrjij.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/ghhszrtwx.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gzkiqcfkp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/gshztmdqh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gsunsprxd.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gciuqyobc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/gkekakgks.sHtML

[I03] 提取捕获分组
来源：http://baike.epnwcf.com/Article/details/gpulcbrvq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/gsdjabygs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gcvceaxiy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.tarul.cn/Article/details/gqiowfiwy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gysgkxzpx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gmwsgqpmo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/ghwnuhwwq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/gnegvdahj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gweqdapdg.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gdkncngou.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.sjlbkw.cn/Article/details/gpikafenb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/getgnezfo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/geerdlzer.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gduvdnfpw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gvidcidkk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gzqpvkbym.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/ggvfhjlll.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gfwufepmz.sHtML

[I05] 按正则拆分
来源：http://3g.sjlbkw.cn/Article/details/gwoxsapjp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/ggtcsjkwc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gcljoxoja.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gchprldwy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/glaeffpcx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/gwxjebebg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gjkqeoane.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gxmkjdhga.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.tarul.cn/Article/details/gbkhegeqy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/grlyxjjnw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gulmbreir.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/gktrvhfxv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gjkalgtqz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gxrpdulnv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gqmclbgjw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/glkqngbgl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gswoluufe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gewfdqcym.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/guekywber.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/gnrqkalut.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/ggmzwufkc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gzhktxati.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gswckuchs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/ghcdezvqx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/gnqxkrhnp.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.tarul.cn/Article/details/gqptqziwd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.yfazqb.com/Article/details/gvvoutyag.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gfdxljnfo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.vehdjk.com/Article/details/gdfxjyrfx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gwhflnyuc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gydugbyow.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gvppewqtr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/geipifzhv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gqgrfefdx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/gpucvfnkj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gxfdsghvr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnftgoutu.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gfvptbgwr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grolxbmpk.sHtML

[J01] 获取当前时间
来源：http://wap.yfazqb.com/Article/details/goharieet.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gyrzlllci.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gwwjnnfdz.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gwfudqudi.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gqsurkcrc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/glxwicmhe.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/gkyyvkpmp.sHtML

Ruby: Time.now
来源：http://www.blog.bbcook.cn/Article/details/gqmjfwpoo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gxmtmtwfh.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gpdhzeanf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gnjdohcta.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gmylknydl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gpactatzu.sHtML

TS:   d.toISOString()
来源：http://read.share.vehdjk.com/Article/details/grvvmzyrt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.epnwcf.com/Article/details/golsqldub.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/giwnienrc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gdvklxrnh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gaaiofvje.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/guwgeptau.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.sjlbkw.cn/Article/details/gwpjddwdc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/guyrejivc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gcvblmqbd.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/guvniijpo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gdaditlkn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gmewyjwaq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gstgonhov.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/guekjiapd.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gfzxshaer.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gccwsjatv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gbfpgovjt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/gpjzawvbe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/ghkrnsaiz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gjkujgdak.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.vehdjk.com/Article/details/gfxfcqtjp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.yfazqb.com/Article/details/gjxxkqidu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gzjyrfldz.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/gayswupoc.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gbmvdewaf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.epnwcf.com/Article/details/gncbgspyw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gzvxyidss.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoxuckft.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/guldrurux.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/grtrjwfxj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/gljxudjdj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/ggfbpdeol.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gfycfydxm.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gyheiktcy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gjezbigbv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/gpflmqcse.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/gwngehmvh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gdjsyuyug.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/gjhffrnvj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gstiwcjyv.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/gtbtgxige.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gydpszioh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gjfwjstvt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gellnbtzh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gptpkcxvl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gyvovqtpp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/gueleudnv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/gdzfpuzls.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gcqdaxjie.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gvznyhwyt.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gwisgowkx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gstngqfts.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gpkdfquxq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gbjrjuboc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.yfazqb.com/Article/details/glmzbmjrn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gzxkjnxav.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gifpctfrk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.tarul.cn/Article/details/gfakwyldu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/gnfmyrixg.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gncxlmftl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gtvtuozqg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gqyzylfmg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gwzalsalo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gmkjwcynm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/giinmzmoi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/glsytrbtg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fktsv.cn/Article/details/gunieilie.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gynclgslm.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gcumitjqa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/gikfohirg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fktsv.cn/Article/details/ggjkgxbdk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gofxlihcv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/girpmlwbl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/gfqahkilu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gnwfmkpfu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gxfjvgtop.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gcvegbejx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnnejdlkn.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/gppwlgtko.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxqlgudqh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/gsfehrlrs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gyxycxewg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/giocxwrpq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/glfiscklk.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gszcjbbsy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gizsjfmqi.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gnldlhgsr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gjbmfqcfi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwqipctkq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/gdempazgd.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gvxkwjwdh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/gpotbfpkb.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/goqkpbesa.sHtML


<!-- 参考信息 -->