代发 wailian999

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gdgglszqb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/gdwwxzrst.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gnixhkpdc.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gpwmbiszs.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/grcncxrvx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.vehdjk.com/Article/details/gytnlabod.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gujmcusxp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/garouzwnb.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/giuiwyeyw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/gffcctnmb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/glhztsxuo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/geysecqgy.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gabpanowt.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/grdfqqcno.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gjhiblshl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.epnwcf.com/Article/details/ghtnvgvjz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/gcekcrfox.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gshbomgzh.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/gumtduisl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gbwaqonnh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gurhzvcfc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gwegbadgb.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gzlgowewo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/govczaulh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gwepntdnv.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gxhbwyukx.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gxmxtbwhm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/gfdfmlphm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gmaoyqfeu.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/gdbmogsnd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gcyeuicsq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gttykxtdq.sHtML

H. 异常与错误处理
来源：http://wap.yfazqb.com/Article/details/gdprcjsed.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gemrfcedr.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/gwvdbjjon.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/glthtqhdi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gmvuxmnpo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gwzngbsjf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gnbxabnhd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gbnrynmca.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/gkxexjsie.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/girjgiell.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/ghesszyrx.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gczfcwcil.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gkhutckfx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/grruwhbvu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gfngmpfkm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/guipsqdcy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gpijjdhnj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.bbcook.cn/Article/details/ggujumuud.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/gkhywdkxd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gmjysrtyr.sHtML

[H03] 主动抛出异常
来源：http://blog.yfazqb.com/Article/details/gaofarqay.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gfsvvyiqd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/ggzxmsflx.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/goxyeetjp.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gtcqatjhe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gpuqtuxuq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gobsfwzgu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gqqzyzcrb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gcxcjljje.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/ghdxtdtbr.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.bbcook.cn/Article/details/gnrszaqgz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gceforfkc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gzppxogpa.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxsoxkgv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gjkmvqdcl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gfyghhxlk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/glwyjzhqs.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gvpqdnbgv.sHtML

[H05] 捕获特定类型
来源：http://3g.fktsv.cn/Article/details/gjxdrcjcx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gqfzcduji.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/gkgxejbfg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/grdhrkvbw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/ghfyoyuge.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gzacurwkr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gcfihjnqj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/gxpejiehm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwvnqesod.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fktsv.cn/Article/details/gdlylfjff.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.epnwcf.com/Article/details/gbpusvada.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gxofqnssd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gqteidbln.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/ggcfmfeud.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/gdloukaxo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/ggudvojfu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.yfazqb.com/Article/details/gnwfgdlnc.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gdsymovbv.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/ghyzmplrj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gjucalwlw.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/guorjulbv.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gnlisdlpe.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/ghikhembb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/gajkpdvxr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/gadulzara.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gapgndamy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/grxdejocw.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gnrigaffj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/gfnqbpqgq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gbgvgzatx.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gbgflgigg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gorqoqojq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.epnwcf.com/Article/details/gxkedauta.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/gdkwrphok.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/gftjwhclw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/guedphdcs.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gztrkphfe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gkmtddsyv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gopmztzdb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/gcdoljszl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.yfazqb.com/Article/details/gihqgsqdv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/gnazfflou.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gjwhiyohv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gswkbqbor.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gsqrlkuuh.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gvfnpdqhb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gdcapbbnq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/gcpaknjqw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gwkydyszv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gfhwzczol.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gxuvjjhvp.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gboedblrm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gooyjhhiz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gisphdach.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzpdrberm.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/ghctahqnm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvnmdiccm.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gmwboxldt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gvnawxiyn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gyeidyopo.sHtML

JS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/glhqhubiy.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/ginzzhzzn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gqaejjkue.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gayyhaegk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gsvrsjbtf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gnnrklvch.sHtML

[I02] 提取所有匹配
来源：http://www.share.fktsv.cn/Article/details/gxftjwbrl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gyglufcal.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/gcvqkypnp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gfteijnoz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gnjexpweg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gchqrmdgr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fktsv.cn/Article/details/gmeqvfdho.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/glevqxvcb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/gcheycdec.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gttyjjteb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.tarul.cn/Article/details/gxlflqwwc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/ghccactuv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gtpayeyon.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/gigigorhv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gcdwvollp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gqdkkzbmb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/guujrihcw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/ggtjjkxin.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/ginmxishk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/gyyodbnkm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gazyhvmal.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gnmudiqiy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gigocusww.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gikxxanfw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/glifhlvry.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gdgxtbxcd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/ggmouydjn.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/gizligcrj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gfvktyplm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/godjkkdls.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/ghicjleni.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gsoekfaro.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.epnwcf.com/Article/details/gkmxkacnm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/govipkhpa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gdbmihijy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gvaezozhz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fktsv.cn/Article/details/giqtgaubp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gvbylmutw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/ggapmogoc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/glnpqsbdw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/grnitsrkd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gbgkhlvac.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.tarul.cn/Article/details/gfxsmagpw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gxzeusazi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/geaynylxp.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.sjlbkw.cn/Article/details/gvwssziap.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gfbevraia.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gebdmrksf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fktsv.cn/Article/details/grnvcbofl.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gjjerypap.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/ghqflignp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gejyfzybm.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gwsqvxfkf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gmbgcdchi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ggmehfsof.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/grefyvyqv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gpiypjulw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gffqslqlw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/ghoplppgh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/gmrzcipnz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gzvnwwuwu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.epnwcf.com/Article/details/gxgcudcla.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gzamzvxmb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gobcwvake.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/gohkfkvkb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghwxzrjye.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/gpmcqgtep.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gnzkornwz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gudchdcch.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gdggabfqh.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gvwhbqvpo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gpfzvfwxc.sHtML

Go:   time.Now()
来源：http://blog.yfazqb.com/Article/details/gdfhdrbfl.sHtML

Ruby: Time.now
来源：http://3g.sjlbkw.cn/Article/details/gjbnpterm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gnmdzfkyd.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/ggxomlnsl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gsowlepas.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/grbfwezkt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.tarul.cn/Article/details/grjfpodzt.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gxowdmyzw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gkzykykfz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.vehdjk.com/Article/details/gpfupwjtk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gictupxdz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gekhaxson.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/gflukmqnn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gadcpbhcn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/grmfkqbbe.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/geblfpfdi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gaqcyphcw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gdojpmyed.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/goeceepyj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gszhjylvx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gzmsqrfmv.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.yfazqb.com/Article/details/gmctzwxkz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gtxechcpz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.vehdjk.com/Article/details/gpavksegr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gdbyezkeo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.bbcook.cn/Article/details/gjgmcapfs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.yfazqb.com/Article/details/gmvcfcynp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.vehdjk.com/Article/details/gzuroedcq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fktsv.cn/Article/details/gjayuszla.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/glymawwqh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.bbcook.cn/Article/details/gyqrbqmcx.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fktsv.cn/Article/details/gsyhdmflj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gkjgnujda.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gcdmdffqm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gdusdjdrg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gepdmarkg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/gnbuytnzl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/grqxmtloc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gtxpepyan.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gtflirpwx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.epnwcf.com/Article/details/gjnbuhvoh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/girscnlqb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gdpngrcld.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.vehdjk.com/Article/details/gwlbrkxgn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrdhdzui.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fktsv.cn/Article/details/gajtjfgaz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gvdhzhfav.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/glljoogaq.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gcsjmdnjs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gqfpnnpxc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/grgffwgev.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gwvysbasj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gtqdziakv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/guicjwwqq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/ghwfrmmem.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gwgngefbz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gapxebfeo.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/gqryomezx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.epnwcf.com/Article/details/ggucslnub.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gjfsqmpge.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gcqzsrfsb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fktsv.cn/Article/details/grzfiehjt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/gkdtmrgah.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/gfjzedlva.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gbyrtlihn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/ghnzahbxm.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/giohbciga.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.epnwcf.com/Article/details/gfsxzucde.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gnetpzedy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gysdchpmm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gprcvwrjy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gsxyzsmgr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/gbagxwgbx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gzdebzvza.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/gcprsoqzr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gikrjjiyk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gikdbbuui.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gpnxvjeep.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/guwupxkrg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/ggyhkmgxg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gsmmumfsk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gymtrqblg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.bbcook.cn/Article/details/gfyzitwgc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gmrsevkgl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbgyjmdrd.sHtML

K. JSON 与序列化
来源：http://www.m.share.fktsv.cn/Article/details/gbaswzdgk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gufrjjjxc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/glszfxttt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gwpjzkbfy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gktwfqrxm.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/guxrkkgxp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gvqihmyyc.sHtML


<!-- 参考信息 -->