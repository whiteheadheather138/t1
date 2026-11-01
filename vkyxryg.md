代发 wailian999

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gbxegrqpi.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gqyefpcnm.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gtkifzfso.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/glhjqzykk.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gbtowjgcs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gspjqhhgn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gpogawktl.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gzoeehsfx.sHtML

[G14] 数据类 / record
来源：http://blog.bbcook.cn/Article/details/gzcrvvrgl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/gevomumjk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gyqhyiorr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/gisdeqqdf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gvmzovtvp.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/glrbsdhcw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/gwcborais.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gynrhhgmj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/gsanihhpz.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/gvjvdkjou.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/gehmyeslq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/glyxtlvmb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/goffvdhyr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gylvrcsds.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gpcnyganw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gpylnrxax.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gpplxexvh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gekliizdh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fktsv.cn/Article/details/gnifnmuok.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.bbcook.cn/Article/details/glvucqvdo.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gdgpihhmn.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gzwtfiveh.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gvxoqluox.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gtuqogema.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/gwjgdbmrh.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/grcvjmfjl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/grsflbqno.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcduxogwu.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/grghhpmml.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbwfxyhpt.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gxhabonud.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/guhvbkxui.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.vehdjk.com/Article/details/ggpxucjhd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gitxyuqsr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gbwmkvymc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.bbcook.cn/Article/details/gnxpplxmf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gaxcxymex.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gttbcwyff.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/gqhefdzls.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/gwskggqbf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gnphwbmsf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gphjchupd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gzyghwvpz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gxeahibro.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gcfayizqp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gdcuorwuc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gvftbuozl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.bbcook.cn/Article/details/ghhetcgyv.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gdqtvmcau.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gnwjhsqzl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/geptbahyi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/ggozjowrv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/guaxvjkvk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/grvwbagip.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gsrtknhgp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gptcjhgrw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gxuctowca.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gfmujhuvj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/gttxfzhvw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gxouwhuwz.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gfirntjpl.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/grxnjvwrc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gubruzwfd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.yfazqb.com/Article/details/gkzlyolrg.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/gjkvytgzx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/ghbfoblcd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.sjlbkw.cn/Article/details/gewkyackh.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gycokjrip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.tarul.cn/Article/details/gezycwucl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gwhekopmm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gjeqcpyrg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/gwryvzwod.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/gpqgngcnb.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.bbcook.cn/Article/details/gqvcqssoq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/grvccqtra.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/ghsybvuas.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gcpwlwxlw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gepvnkqeq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/ghuaxpzdr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gkyzartns.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gicudkhvv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gotjmpahf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gvpkezszn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/gjdlsfayc.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gcutntrap.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gzavacwzq.sHtML

PHP:  assert($x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gxelncjzy.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gqeezuylp.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gmbxbwxmg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gwlloymrr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gnovebtrs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/ggrtxcwtw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gwfkytktz.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gfmiedwmh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.bbcook.cn/Article/details/gubbrxvit.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gifipdyxb.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gbliwgywu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gtlzpunui.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gsfvmmojs.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/gnxagqkxf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.sjlbkw.cn/Article/details/gszkajxzn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/getjgxycn.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/grykzdown.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/ghvligwff.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.vehdjk.com/Article/details/gjtjhcchg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/geuwehtif.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/grazsgnya.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.yfazqb.com/Article/details/grlamhenv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/gaqflnbfj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gsbwcdkmm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gpbrfhzrs.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/giyapcxgt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gqxsyntda.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gsgdsbkit.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gdtrcuoke.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gabpegtnm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gghkeagrn.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gszdyxqew.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gryokhoov.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/ghctwadef.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guyyrivqo.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/guuozowgt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwpzgjvxd.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gfgbmjivs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gvihptctg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gtwlpojtx.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxfkafxmp.sHtML

TS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gsgribweh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/ghhtiaqrh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/glsaltzuu.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.tarul.cn/Article/details/gisqtmqwm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gtaagertn.sHtML

[I02] 提取所有匹配
来源：http://wap.bbcook.cn/Article/details/glmubdxsv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/ghaxxrwqv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gyofdchxs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.vehdjk.com/Article/details/gudnlbipc.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gakcjkrkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/grghjnujb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gtsuhdlpj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gcwiwsbbl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gtbfefmpy.sHtML

[I03] 提取捕获分组
来源：http://www.share.vehdjk.com/Article/details/gyhdvntpn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gmtcuoymh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gruhsgjda.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gihhbyswg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gdppyipfg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gpoaksjxh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/gaebdjftx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gqydqianz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gncfoiced.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gidwcmhsw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gdxhsoxwd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gvhvzesyl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gfdmucqvc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gnkgcfetr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gewwiycqh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/ggvmttwne.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/ghdpiexpw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gmuzkmtnu.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gzmkgwgoj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.sjlbkw.cn/Article/details/gjkbwfzmx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gnotihpwn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gvtbkiqtd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gjglsfepy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.bbcook.cn/Article/details/gwwjnrtcf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gqetsfzwu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gxquqbiui.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gtinoxixu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gulezgicw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gtrteilkc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gjpgkymqm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gebdvctpe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmpgthrl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gzpvvirls.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.yfazqb.com/Article/details/gtjltltnl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gzqdgkrol.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gvayfohly.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/grjmzthuq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gatfrvsvv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gfrwmuood.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.yfazqb.com/Article/details/gzxtbylhp.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gohphnokf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gyahmgusi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/guwusdceo.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gnfsgbcfc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/ginlqwsna.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gqidqaqbm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fktsv.cn/Article/details/gtpqragyk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gzkuuqonc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gdyddkujw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/ggoucrhkj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gddxyvktg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gaoerakql.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.vehdjk.com/Article/details/gjfbbzpac.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/geripptpx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghndkuvhy.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gzocpcioz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gftglekuu.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gmznqhcls.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/ggtvazsoz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gqisipwpa.sHtML

JS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/golibjtcy.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gpgwunrqp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fktsv.cn/Article/details/gzzjbiaza.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwifuxeyy.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gnwflklzo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gwgeesdkt.sHtML

[J02] 格式化输出
来源：http://www.share.yfazqb.com/Article/details/gleauvwjg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/ggkofbcto.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gssrrxwma.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gbswputei.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gdlkfccat.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fktsv.cn/Article/details/gdzvvbxhn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.bbcook.cn/Article/details/gbgqiuvrc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gkpnkfewy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gszczcbrw.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gxwkxapuj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/grjkvfmfd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/gsqkrxkeo.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/goojxeqsa.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/glxdrssnt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwshbddgx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gafdqqqwh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gkqosmyfy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gulvsecvv.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gxrqdelhi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gtkabbdpc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gvwzvtwdl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gvcbdibpu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gpwcgnopj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/giqfyobdr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gtkwxwoat.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gmwqidisy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.vehdjk.com/Article/details/gzajpkdhl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/gulbjgtuz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gmqjbjjxy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.epnwcf.com/Article/details/gtjutvciu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gbkgzyorv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gymlqbeuo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gyciypwmw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.epnwcf.com/Article/details/gwctmares.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/graigczjr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gyimbfxez.sHtML

[J06] 计算两时间之差
来源：http://mobile.vehdjk.com/Article/details/gvklahfqu.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gzhvgcycp.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gjtjjkffn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gfamiqxne.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.yfazqb.com/Article/details/gcbxkvyog.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.yfazqb.com/Article/details/gqpjjwyta.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/grsqvtqyb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gsscxenzx.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/gjcdedcvv.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/ghfbvvdxc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/ggubpxxhr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/gvcuinvjl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gpyeqfqmw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gwoashlgm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gkzseoquz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gtugfuonw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gyoporinm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/goajsjjrz.sHtML

[J08] 提取年月日与星期
来源：http://wap.sjlbkw.cn/Article/details/gypzsdlwh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gglqgiapw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gqhcxnivs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gpkaundvq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/gtkchxjmg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gkfasxsog.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/gadsckafw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gsjkmppzx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.vehdjk.com/Article/details/gbogbwyvq.sHtML

[J09] 时区处理
来源：http://mobile.tarul.cn/Article/details/gvqxuwnrl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gdeiptcoy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gwrqgzooi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gqdnxcjgn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gtttmaiwz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gsjvfshba.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gkhvgbddt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gebdieppi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gnbmlocbp.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/gugdhvfff.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gezzmigmf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.vehdjk.com/Article/details/gpyxvgwng.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/gfeiopvby.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/goaevczws.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/gnbpvemss.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gxfmyewjg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fktsv.cn/Article/details/gozqsazlz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gzwiuqmfz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grfogenvt.sHtML

K. JSON 与序列化
来源：http://mobile.yfazqb.com/Article/details/gyfnjesly.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gczobnyxu.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fktsv.cn/Article/details/gticezwfh.sHtML


<!-- 参考信息 -->