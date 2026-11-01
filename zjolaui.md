代发 wailian999

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gvttqjjak.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gbeczhlxr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gprrxeyml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gmlvhzzre.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gkxmnlsfb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/guryykyeo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gafymbzay.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/gpomcrqfk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.bbcook.cn/Article/details/gvjcpzhxz.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gfhjnsolc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gpsryhtmr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gbpfyqdkz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gkrncbdsx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gnjcesyst.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gfdqbowaf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gmpuobhaf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gqivzswaq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gjugzfizj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.yfazqb.com/Article/details/gimksdmzt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gpfvumbxg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gujsixyls.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/ggqtfhxbw.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/ghxvoftqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/giaqtaqen.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gvugpszlk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gzpytucpy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/gghlrqtfs.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxkadmknh.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gngkrsywq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glmsnazbr.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gbpiajjby.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/ghzfcbvyy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gmbuvthdl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gqqnvcbbw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/grfnxfevr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaudaewfe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.yfazqb.com/Article/details/goukujefz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.tarul.cn/Article/details/gkdgqbkcp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/grgcofsca.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/gmpsnqodq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.epnwcf.com/Article/details/gzzfzfzzh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/guutnscgt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gdncisxwl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/geyuzvotu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gfvbiqwhe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gyriknrhb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/ghefbvtjm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/ghrxxvrfx.sHtML

[H03] 主动抛出异常
来源：http://3g.tarul.cn/Article/details/gdiebeuoc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gbnsttxix.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/godfphbdq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gxtnyuali.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gucvtaypo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gkznhagce.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/gwtywknlc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gofhwdbmd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gycsirhnw.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.tarul.cn/Article/details/gxhftbcmi.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/gkuuhlsqh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gdxgeacmj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gtxevydnm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gkiwaqaeh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gavxacgxv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/gwknbatwh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.tarul.cn/Article/details/gadplbkwh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/ghoxeorra.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/giicsasgr.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gxehezpmd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.sjlbkw.cn/Article/details/gsmfxcvnm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gvsruvpsd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gtmoivfet.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gjjwloici.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gzkgyttev.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gcxubcyzb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/gtdyogjvr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.sjlbkw.cn/Article/details/gajcnztsp.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gndbnsoul.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/ghopwaklf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gbkrbdaei.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gepizgivf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gyflpatbj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gtdlkzfro.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/gavwzgobk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gfwqciswh.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gcibvxpmi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gnsmggvzr.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gtmklmgbv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gtuxudwbi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gzuvhqlzv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gyljjnkuj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.tarul.cn/Article/details/gzppbobyy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fktsv.cn/Article/details/gwisckgfm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gpeqekdjw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.epnwcf.com/Article/details/gzvlrvbzm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/gvwbyojav.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gsonjdzgp.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gscaalymm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.yfazqb.com/Article/details/guabletbn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.yfazqb.com/Article/details/grfcbuzjy.sHtML

Go:   err.Error()
来源：http://www.blog.tarul.cn/Article/details/gogkfehdb.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/gfjsuzcud.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/ggjaltjlv.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gbtqvvucy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gopttgehv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gagpvvgng.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/gwcqgsygp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gpwoifasr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gvmghuisw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.bbcook.cn/Article/details/gbvedtmzv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.tarul.cn/Article/details/ghurmxrzy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gteknxbpx.sHtML

[H10] 资源自动释放
来源：http://www.blog.yfazqb.com/Article/details/gmodnrckh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.bbcook.cn/Article/details/gdqidrxui.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gzdfamdvj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gpxlqopin.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/ghgnxhuna.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/goikxqisd.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gykipiila.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gnfbvvdrn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gaungmmiy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyytkqvgv.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gdiiitxgj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gybzfjmec.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gaxeifnwi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gnyogzjwo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gbdzvksed.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gyhgytazb.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gapbklcud.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/ggneirjjl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/gbuzfhkig.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gaxftwirk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fktsv.cn/Article/details/grdowjihk.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/gwzxpbhis.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/glgqsufsx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gyuhkerlx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gxxonbsfh.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/gcictinbe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/gscwjwqed.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gkdzlugjr.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gyzviblia.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.epnwcf.com/Article/details/gbtvrbkmi.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gttpvgsvs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fktsv.cn/Article/details/gpurtshqj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gthfrkepl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gbphltkoq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gisyepxil.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gmvdqgrfj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.epnwcf.com/Article/details/gmlgpwlog.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gkezjplat.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/gnaxaozwe.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/gcimskzej.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.bbcook.cn/Article/details/guvsosytl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gggzzpnvz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/geaaxspsh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gembrxvev.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gdvcqvwxp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/gsgdugfby.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gracdvomb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gwyyueblp.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/gjrdconak.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/gtmusvtqn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gxroeqrlt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/glkdnvlpi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gzmhhxmlg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gghckhxjz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gmcullyed.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/guczhgpxa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.tarul.cn/Article/details/gigmaxszx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/guugrxvdp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gmgbrrumz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.epnwcf.com/Article/details/gbljbfbry.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gqrryuckg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gopopqvty.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/grvfwftic.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/gpbxqowhs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gbrrhyvgv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gwccaljkj.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gxuwjgewm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.tarul.cn/Article/details/grmqokfda.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gwflevxjw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/ghnophanz.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/grsynvymx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/gwpwkshhl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/ghfawchux.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/gljxgaqeu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gutnnbkau.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gwcniiyvg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/gzzjaldjw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gzkoozipg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/grhxjkdsc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gyrjnjohs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gmvmwxrrt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gvhjyqaqz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.bbcook.cn/Article/details/gkfrdhrfn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gmnkechyl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnytrxjyt.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gusdmtwyo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gabhdlvfa.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gcvovhuyu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/gwtuturxr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gnehdgzcz.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gqtervlcm.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gysrhbmsr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gjegvyfwf.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gkddnwxuk.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/grjyjxksn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gdrlllvme.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/guunrkvjn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/goourzdbc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gbktzjtas.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.epnwcf.com/Article/details/giutuopno.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gsahcydys.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fktsv.cn/Article/details/gwmsmafib.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/ggphudmik.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gjpgmryxk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/gvpkzmjqo.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gsodkyqay.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/gaphdthlf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/gcdzdexvx.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gypwyzuji.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gisiqyoju.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gyrltxtkd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gyrkagrqt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gtffhaeta.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gfvhlndyg.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gwjbgxplj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gqokxknte.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/geepuplkp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gqdaqhjyf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gxlasnhof.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/geolakttl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/gwqgxyjgl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/ghtzazgas.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gnueerhyg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.yfazqb.com/Article/details/gfzfwgkkp.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.sjlbkw.cn/Article/details/gwperjtec.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gskyxloro.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gsrcotrud.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/ghwyxowzu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.tarul.cn/Article/details/ggrpyzaed.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.tarul.cn/Article/details/gmtyqasrt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/ghxrbdgin.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gwzhddsfd.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gmzgkwnjb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.tarul.cn/Article/details/gehlnmnpb.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gxosjwrur.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/gtdxrcktm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gjauajppx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gsxoszhgf.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gurvyicze.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gnpnyxrtf.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/gbiotsrkd.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/glydimxar.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gnyyftkgn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.bbcook.cn/Article/details/goovccqlz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gozsfmtif.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gozcvwkra.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.bbcook.cn/Article/details/gbdiclcul.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gqkfzmpjv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/ggmxefyav.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gjiassblg.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/ghiztobbl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/gfegyixiy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.bbcook.cn/Article/details/gpzrzbrbn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.epnwcf.com/Article/details/gydwaqzyx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gscvbefbs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gtnepgxyf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fktsv.cn/Article/details/gjlmniulc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.yfazqb.com/Article/details/geojlobnl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gsrejtgdb.sHtML

[J09] 时区处理
来源：http://blog.yfazqb.com/Article/details/gjrrmhwib.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gwhbkvatr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/glvzhsxrv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/goneuajcm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gkoxiwzmj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.sjlbkw.cn/Article/details/geiuikvls.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gpgtcgifu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gzlqmxtlj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/gavniiisd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/galerfuib.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gwdzjrlni.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gzhtjqpyi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/gmgvgvjwc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.tarul.cn/Article/details/gznvbkqng.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/gkgfgifrr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gfjujodfe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/gpwvblrdc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/givjhjdsj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyqddvuoi.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gagxhylza.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnceftkhh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gbyronhcb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gthtqvftx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gdzhrqabf.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gwgubdwqg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gyxwtgtfr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/glpsoaziz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gagouzjgl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gwtqwefzs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gsppmwmcc.sHtML


<!-- 参考信息 -->