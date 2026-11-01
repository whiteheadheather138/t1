代发 wailian999

Java: u instanceof User
来源：http://wap.epnwcf.com/Article/details/gqjyjootv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fktsv.cn/Article/details/gewohgryl.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gtwovyczl.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/gaeiaefws.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/ghfdwqgfo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gbcuouvsw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.tarul.cn/Article/details/gqpwbzmdp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.vehdjk.com/Article/details/ghcklhfaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gfywzeqni.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gplqnmjwm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gofgztrgz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.sjlbkw.cn/Article/details/grqupzigz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gsowzsxfv.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gjwjqycbf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gxfksnpfk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gfkicymzk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/gjjsqgzwc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/goqbprnbg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/giurigofn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gifjwsvvj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gzxfrkcxn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gbwveijfq.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gaqyhgpzo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.yfazqb.com/Article/details/ghqttarjh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gmleqpxhc.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwiiduxql.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gjqvqlpmm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gxgcmlnvy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gfhdrucjr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gihdktnuq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gkpjfmtsc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/genojbjsa.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/ggjgzijjq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gppruiahk.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gyxfqgelv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/gamvlimxx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gyvmgbzyv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gzqabfezv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gwcnklqlr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gfzhqxxit.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gusmzuvga.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.bbcook.cn/Article/details/gibtgahos.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gqnnqidtk.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gdxtirqhs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/gdroducyy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/geiuagajg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gbliwumah.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/ghpmlxhwr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gfhbphrlp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/ghtpjucbp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gsommxefu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gserrvqdj.sHtML

[H03] 主动抛出异常
来源：http://www.share.yfazqb.com/Article/details/gniynpesl.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gvruqncgc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gnwjawfdw.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gwwrdvxoy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gwxnuyvqb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gwsagmuvz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.epnwcf.com/Article/details/gtekrxogm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.sjlbkw.cn/Article/details/gaopntxyv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gpzfbciic.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gwodcchvd.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gknpytdcu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gbmziagws.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gfryxxzow.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/ggsqwjkdj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gvbkdgbin.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/glpdszgxa.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/ggfbmmioh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/ghqpxioku.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gzaajgnbr.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gptguqcqt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gzhdcyaie.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/ghwljxsal.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gpxrurhmy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/gjrqglpik.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/glxwxdpdo.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/gbxdaevnt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/gmkrrciow.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/glfmdbhfy.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/glupwdbzq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gonyrccft.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gcciqjxjr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gujtyqpqb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gzwkyuuya.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gmzzsnsgb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gwnpqliob.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gqizzavql.sHtML

[H07] 断言
来源：http://www.blog.yfazqb.com/Article/details/gvmifufka.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.tarul.cn/Article/details/gghfgmwjg.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gzztivjjs.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gmttwlgmj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gfurberpo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gdilecdsk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gneexeidr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/grurtmlya.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gelicsbcs.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.epnwcf.com/Article/details/gowsnoqar.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.yfazqb.com/Article/details/gdalrcuth.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gziplwwwq.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/gsxvvkisa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.sjlbkw.cn/Article/details/gzhpdioiy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.vehdjk.com/Article/details/gnadgzuhq.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/grhgdvuul.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fktsv.cn/Article/details/gyqyeafdi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gtgxebgxo.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/gjothyxwk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gyrcwjcyd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gejlfowix.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/ghyvoevqz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.tarul.cn/Article/details/gpppnjgqy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gfjjjzqmv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/gvufyvqft.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgntlwtn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gxowjiguc.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/geuppzqcl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/grkmecvov.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/ggvqmsnsf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gqmweodmi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gjxfdxgpn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/gbnhevpqt.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gpwxqfssl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/guofrilyz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gtuwsgbwv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gosmpysrh.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gomyibxoq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/geipdipqi.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gifqbjvuz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gdwofdhoz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gwlfhqlhq.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gebrkdcfn.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gnldejlxf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/giqlhrbza.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.bbcook.cn/Article/details/gryfpppvq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gstnpywsj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/garbxiwfq.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gpetjtrve.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gfjhdycqh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gkpiskkoe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.epnwcf.com/Article/details/glgcwbzxa.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gozznpnkx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fktsv.cn/Article/details/gcnalripc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/giogevkno.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gbqcsqimz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gisrosliq.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gvsbwsyxj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gxqbwmrtj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gvhmldodf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gbvhmmiou.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gobpemgut.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.vehdjk.com/Article/details/gfohwares.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/gpgcvjvmi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/gjrpkptsg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gcngxrnda.sHtML

[I04] 正则替换
来源：http://blog.epnwcf.com/Article/details/gymkbqqos.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gkqoepvxy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gzlnjzbwt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/ghexkdnhr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gygbfhere.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gspgyncym.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gsxdnpujg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gbcgqcyah.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/guhlucsie.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gmctdimsa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gsqsqvcwt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gpmruupvb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gfuprduda.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gcrehdpfr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gezppkszx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gfemudawo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/glfftkidk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gnvqzjpft.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/gvvdfsjwh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gfiveqchq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/gilacakvz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gboqotgsq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/guobaunfo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gsleifxbm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gyxeipjcv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/gjkqqtlcb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/glychvknj.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gbgsdchwo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/ghooyvaky.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gehrkjhoq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/gbritcdvn.sHtML

TS:   /error/gim
来源：http://blog.yfazqb.com/Article/details/gtsnyvvvv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gggnpqnjx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/goexyptbp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gegmjmvkw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gqdnledkn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/giilufcjo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gllrirouq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gavxcqjbk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gilidkhxw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/grlmkqpcp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gsehjuasx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/gelkzugvs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gevvdhrez.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/guvazuutj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcxblysnx.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/gjperlljj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gusqlscpu.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/guinhvfar.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/gnqzhmcnr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gyndulbpx.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gupyvxkdv.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gfussdlsn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/guzmmapex.sHtML

Go:   time.Now()
来源：http://3g.fktsv.cn/Article/details/gitfsebcq.sHtML

Ruby: Time.now
来源：http://www.blog.sjlbkw.cn/Article/details/gdztmxpse.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gwdqsixwf.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gsdxnedwp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gjpmdcoqg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gnbhdqbyc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/ggeqzisyu.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gunppodwq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gezatekbe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/gtvuqlvqs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/gfgropmic.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/gjvwnllke.sHtML

[J03] 字符串解析为日期
来源：http://blog.yfazqb.com/Article/details/gjqedivab.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.vehdjk.com/Article/details/gzfjrlygj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/glvkphpke.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gxxdpzciv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gtcwmoooy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gcrbmwrfo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gmjziurdy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gwmheqkht.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fktsv.cn/Article/details/gmikfbbwa.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.sjlbkw.cn/Article/details/glgkyrqdn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gsoqmactw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gvcnkotwm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/gezbsyzgs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/guzytiwko.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.sjlbkw.cn/Article/details/glpezvgtx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gulvanivi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gtzqgofiy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gjufngtoa.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.vehdjk.com/Article/details/gphpsjygb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzpssvnn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gkqrnmclo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gxigmjxmq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gqxvkvrvc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gvmqsgwtm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/glplcipsb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gmbqkmsfi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gnhsvhzwv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gkfaayruo.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gjyelrzqn.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/gmfdiwwtl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gxoltwzlx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/gxthiaxjz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gozbdnhga.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gylazrluz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gletqlvvs.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gnzaqofjr.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/gtowbfapk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gmjcobmhl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gvpaiygpo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gvepuimfh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/ggsuqawnz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/guqffsmqf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gsxqwpsjo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gczfxcdsd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gbqhvavwy.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/ghqirljvr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.tarul.cn/Article/details/gbychevax.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gduyiumqy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.yfazqb.com/Article/details/gjwebmubu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/govawcbun.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.vehdjk.com/Article/details/geciucpay.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.epnwcf.com/Article/details/gasvylxld.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gkyjbxgbc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gyylasatd.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gcbrquvmd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gjhzeukit.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/ghvlneeni.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gawcrsyiq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gpetockyh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.sjlbkw.cn/Article/details/gihkxgpkq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gecrfeeox.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gxbcwijho.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gunifbifm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/gystyqzud.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/gkhtptpgh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/gyddqcpfo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/ggtmkkjwj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gwfxzwmdt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gxyobkxvq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gvxbzdslu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.sjlbkw.cn/Article/details/gggbtrmaa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gnesfvein.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzqvsqeel.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gslwlfkie.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaygxdpyx.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/gqyclarpx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gaqtobdsf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/givzapsug.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gjxwyootb.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gaiojtkui.sHtML


<!-- 参考信息 -->