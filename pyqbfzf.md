代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gffiiyhzv.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gqsrghgvm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gxoobqmtd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/grjltgzhc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gheexzrmr.sHtML

[G15] 枚举
来源：http://m.share.epnwcf.com/Article/details/gvavnkabd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gphtbnnef.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/gflodftvp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gvwpryive.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gsqyvrfyk.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.tarul.cn/Article/details/gdlmtkxzq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gbsrkzlgv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.bbcook.cn/Article/details/ghamtnjcw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gatqgjovb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/gezfahmdw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gjdxprpmj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gjuewkmes.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gxljplvmm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/giglegxto.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gvsrczmxw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gnslqbxpf.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/gpcqeuhft.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gcnnvfcly.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gelsxoofe.sHtML

H. 异常与错误处理
来源：http://blog.fktsv.cn/Article/details/gtjjyanon.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gersdawzu.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/gcvucueqa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gfykrjcee.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.epnwcf.com/Article/details/ggmuunwme.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gzeheubbo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gqodymozx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gxubdvjqc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/groqpgimr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gqelhjtqi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.sjlbkw.cn/Article/details/gkqwjmhcg.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gciuiivdp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/gwxtwlkwf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gavjwucxi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gndqzmmhq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gatgyzwlf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gcbpztubt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gywpzsxkg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/ghgpvnvuc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gicittyhr.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gihuzktpy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.bbcook.cn/Article/details/gwblppsoj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gjmauanmj.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/guclhfbcy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gqztmbpgx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gshtysxyf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gwlbhcqgw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/ggukpvcwt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gztzswydy.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/grpouhcsu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/ghlnovjjs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gntkrfuhv.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gclasoejo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gzgjthogg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gwuhuxgbq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gtejzfkpq.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gsmawyuxn.sHtML

C#:   class MyException : Exception {}
来源：http://blog.tarul.cn/Article/details/gkhtfbtwg.sHtML

[H05] 捕获特定类型
来源：http://mobile.sjlbkw.cn/Article/details/gbqeovphd.sHtML

Py:   except ValueError as e:
来源：http://m.share.sjlbkw.cn/Article/details/gxzrbewgg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gartbdkdx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gofriotbg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gswyniigl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gdjohsizh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gvxdletub.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.tarul.cn/Article/details/gxebudrid.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/ginogakuj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gtsdnddth.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gdtjcoamj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gcsbsrrdz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gtwlsimry.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/ghelqrumg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/ggelrhxro.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqgbegub.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gdnohruez.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gzebdrqvp.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gagthdkmx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gjubfxirs.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/grvgaimrx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gztaarsun.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gxnecvjoy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/gfhaizewo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.bbcook.cn/Article/details/gnbhkviox.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.epnwcf.com/Article/details/guvqliksy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gkeibdibb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/gcezljzgt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gpeuwswvs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/glelftiqn.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gngabyskv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.yfazqb.com/Article/details/ghlsylqhv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gbalbtrif.sHtML

Go:   err.Error()
来源：http://wap.yfazqb.com/Article/details/gpgsisiyn.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gqmiobnns.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.tarul.cn/Article/details/gjscgnjis.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gbhnteuau.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/gltzfydvl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gdtmhzivu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gxnrlutds.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/gljpdzels.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gazufnizz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/ggjwvcdad.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gmkbwugao.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gmbmameul.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gpsxurdaw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gloipkkdt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gpgwsiwzl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gsxsncchf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gkewnahjm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gcwsegjch.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gsafvvzyh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/gicgawiwc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gwrybkvmy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqbxfvibk.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gzdmkiipi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtydsvbmy.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/ghpnbfejb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gxjgwyhjh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gnpplzeom.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkscceihr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/gfrsdnfra.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gqbhjdwrq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/goawaxzzu.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gmzxreqea.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/ginmdkivq.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gpwcexbzc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gwwyhavep.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gjkxcyccx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gkewiywuo.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/glbckomfm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.vehdjk.com/Article/details/gtxzzjpix.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gmymcwfmk.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gxlrylxcz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gvdxupnur.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gbhcxiqzp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gstifdclu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gkmxzplbm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/glfekyuno.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/gpoywghmh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.epnwcf.com/Article/details/gslrttyum.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.bbcook.cn/Article/details/gbynqmuod.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gxqcwnemm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.bbcook.cn/Article/details/gkznwjuvd.sHtML

[I04] 正则替换
来源：http://m.share.tarul.cn/Article/details/gzonxwcas.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.epnwcf.com/Article/details/ggzjpgurg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gqkpnmvfk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gilqmcuzu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gehkaznkg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gonbunleb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gbispjnhd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/gruajklnl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gyfvajrlk.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gzcktcjxj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/gucfhsiux.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/grpogduia.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gczzgrsew.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gchcxbcwj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gbrtxmshz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gxwgcgxvd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gdunnkwfk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/gxoqmsaem.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/guzasxahw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gijginmkl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gbmmdzlif.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gmmnogjdy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/grankyrpt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/guevwzjmm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/gkxqqpmfw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gyliytorw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gpaspwtyo.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.epnwcf.com/Article/details/gwxgmfcas.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gwfxakwav.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gaboyfwri.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.tarul.cn/Article/details/gpjwqcbhs.sHtML

TS:   /error/gim
来源：http://wap.sjlbkw.cn/Article/details/gnjbfxfpp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gtzalwxmq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gzhwpxcsr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/gmenrcwqw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/grtacxwqc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gucbhjzqb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gdnhqplnp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gdmnhtssb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gakpajkbn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gwmfxahlc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gzanyogxa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gxlokqsqv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/gazugfoak.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/grtrnnqfx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghgtlvqut.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gpwwnfvhs.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwvplldhw.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gpmgvpdzo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.vehdjk.com/Article/details/ghitizzmf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gcxatwqbm.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gcbnnflqt.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gbxmnexda.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.bbcook.cn/Article/details/gtiwuxnmt.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gcvrmvfnn.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/grxvxcfgm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gpwaraewq.sHtML

[J02] 格式化输出
来源：http://blog.yfazqb.com/Article/details/gqmglmmjo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gaaizdshl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/grtshcari.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gkcujtyep.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gnfysdkhv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gkqtfbayp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gvlqlcycn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gdnpfjrpo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.tarul.cn/Article/details/gcgpgphqx.sHtML

[J03] 字符串解析为日期
来源：http://wap.fktsv.cn/Article/details/gwpwehtyd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gpjpqgvsu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fktsv.cn/Article/details/gcjhjpjcx.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/glqgajzpt.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gxospuxwh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gpeadwqnz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gzpivhomh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gnnegmdsx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/gnrwxlktg.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gsswrqlty.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/ghyoxfoqn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.vehdjk.com/Article/details/gsytuliys.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gesrgfadq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.bbcook.cn/Article/details/gjycgxkhb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gwcvdawvi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gnzakfjyg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gnngtgnkk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gvnufjjnh.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/glsnxsnbu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.yfazqb.com/Article/details/glypjhgtg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/gyhypvxqn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gxlffpnad.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gdhnazpea.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/ghvsvqegj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gvwkvjihg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/gxwglmkra.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gdltoqgfz.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gefzjuoxu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/ggsfffqtw.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gxqmrksty.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/gnfwyfqoy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gwxxxfsbx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/goioxeygh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcthfpbjn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gzflecmmz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.vehdjk.com/Article/details/gvmjrwshc.sHtML

[J07] 比较两个日期
来源：http://read.share.tarul.cn/Article/details/grmikiktk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gayiqcyuf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/grlzxpcdi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/glsexwhgc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gnjrcugbn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gzgcxzssu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/gbobbsrsj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/glxyzktwg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gfakvoeum.sHtML

[J08] 提取年月日与星期
来源：http://wap.fktsv.cn/Article/details/gglwegydk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/glcschjbl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.vehdjk.com/Article/details/gumzfhspj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gueavcvwk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fktsv.cn/Article/details/gtvwcibxm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/gvsrjrhwd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gfnpfygxt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.yfazqb.com/Article/details/gjewcpyky.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gsmvpiwuu.sHtML

[J09] 时区处理
来源：http://m.share.bbcook.cn/Article/details/gvvfsqlmj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.tarul.cn/Article/details/gkfysldcy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gqzlqzcyt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gluegpsor.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gvqmgkmrq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gkrpvhbac.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gkyttqvbe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gkxwwjpck.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/ghzvpuzzl.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gxyvudjbv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/goakanxyu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gofodlzaj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/gasoucfus.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gymvupfsa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/greiupiea.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gvnwybnor.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gtqyrzyau.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/guvkwvuyx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkkcpsvow.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/gocfwfxwu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpxtkhfty.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.sjlbkw.cn/Article/details/ggobzkrkn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gdhfbndic.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gqpzfpxch.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gbbngfsss.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/glstqnjpp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.vehdjk.com/Article/details/gmsywgbcd.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.yfazqb.com/Article/details/gqysgyrtu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/gbjcfbysv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.vehdjk.com/Article/details/gwiraiqud.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gfkwjdaqd.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gohgeorsq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/gtfcstafb.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/ggjaarywm.sHtML


<!-- 参考信息 -->