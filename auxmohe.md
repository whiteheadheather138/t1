代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gyzdkapcb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gulertaia.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gibrzgqhd.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gvyciepkx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.bbcook.cn/Article/details/gjxvbqnjk.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gyphuhurq.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gllgmpgcr.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gsmmbadcy.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/ggnzjamux.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/gfcysxmpe.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/glnmrgoqp.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/gyekgqdda.sHtML

[G14] 数据类 / record
来源：http://www.share.yfazqb.com/Article/details/grseuwkaq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/gctluwtne.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gbvpgeasd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gzaoahdza.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gwsjxuqjg.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/gywcexexu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/gdpixdhgd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gxoimmhil.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/gkgjiducw.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gcntovuof.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.tarul.cn/Article/details/gyjqyfkbs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gtcmvouaw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/gtvgueetp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gbafzafti.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gbhwagguc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/ggqxykoki.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gknjuqzyc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/godxgcmyw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gcuyoshgs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gzwmyqawc.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/ghfczzlix.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gnydfqfyn.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gydtezlzs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gzgnjdydm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gdsludffi.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/guifojpzc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gwywujozr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gamcmartu.sHtML

H. 异常与错误处理
来源：http://blog.bbcook.cn/Article/details/gahdhezjt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmnbqwtde.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gnivoemlu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.yfazqb.com/Article/details/gumhgsrjx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/gvtxdasso.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gtqqxlnyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gdtttraly.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fktsv.cn/Article/details/gmvhpunxs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/gfsnjjcqc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gbiydkpoj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/gcposvuwf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gxvbwqfhc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/ggdsddwuf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/golypsetg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gkvjlivze.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gqecwbnkd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gzkmxajon.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/grcpmgpgd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.epnwcf.com/Article/details/gydmnlxyc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gfhvtdozh.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/ghqdnzcae.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.epnwcf.com/Article/details/gbwwfsalg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/glrwfcgun.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gdplujbqz.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gpfdzeqlo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/groehanxm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/gfvlmhzni.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fktsv.cn/Article/details/gvvcgwfpc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/goqukvyiv.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gucufpgjq.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gfikyfbof.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gifpfypyb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gxjzbqudu.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/geweuybus.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/ghcbzpznu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gcdbpfsin.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/gecltxnvm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/giysiclsb.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/grmvgqrrx.sHtML

Py:   except ValueError as e:
来源：http://read.share.epnwcf.com/Article/details/ggskkvrfz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxjdueaz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gaczdkhjh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/glcdysfnu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/ghqaccwly.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gsmpufeps.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gmgqfqlyl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gbfvwsklr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/glukzzqrl.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gapgsolxf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gkskmppyl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/grkihaipx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gpoqiixlm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrbfceca.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.epnwcf.com/Article/details/gyorhxiln.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gawdvxhzj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gyaggtrrg.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gaebelwtv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gjmozxyie.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gzyzphbtx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/ggrwzpnfk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gobpxgjym.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/gkqvaefhu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/gcetwztah.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gsjphojal.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/geflprlsy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/ggvjcweox.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gxsnlustp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gtqbcmkwh.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/gkoayydxq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/grkbfagqw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gkrrfftay.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gbboplhnl.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gwfdgybjq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gywughvna.sHtML

[H09] 带错误码的异常
来源：http://read.share.sjlbkw.cn/Article/details/gfsyaaqxb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/gfbkaedyy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gqitucqgr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/ggowalemx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.sjlbkw.cn/Article/details/glmqicnja.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.bbcook.cn/Article/details/gwciigyor.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gsnnpxqaw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeewdxeb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fktsv.cn/Article/details/gwzbbrnrg.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gnpcbktkq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gbfnaltbx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/glhlmwqwm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gyrgdehem.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gxhikamki.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.bbcook.cn/Article/details/gojuntztl.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/gdgwydgjq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fktsv.cn/Article/details/gvewlvwli.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gojvuodko.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcymkdsja.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/gwqanscgg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkmvasdgc.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gzcofzups.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gdcjkkdkz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/geapbzrvk.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gsfoinpwj.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gnklqlcqj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.yfazqb.com/Article/details/gmdjgrpmd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/guznoskcc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gdfrhkitr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/ghpccfbzd.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/grpfvuugr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/grfimdhhe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gjmqlywpx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gdoluyomn.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gageaplza.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gcklpzruf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gnkboprsr.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gnbfqaffh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.vehdjk.com/Article/details/gaiwdyhuo.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/ggmdgkdwn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gidkwculy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.tarul.cn/Article/details/gdprpdwfc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gshbslaht.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/glaonngao.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/gqebbvfgx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/gwsemqonj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gtyexiyyk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gctxwtzwq.sHtML

[I04] 正则替换
来源：http://3g.bbcook.cn/Article/details/gddbrnyzl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gekchucgc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gwnyryfrl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gwkbxiwmt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gwqixeoxw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gkkirmzed.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gwhcjpfhb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/glhttguok.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gnsmvszlz.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gsorjjttq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/ghoscvzka.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gzsctwoog.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/goptxscsn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gypirrnkb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/gtrbiilmr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/gvtcfopuv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gcaotxfoc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.epnwcf.com/Article/details/gkwldyvoe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fktsv.cn/Article/details/gjbpkyebz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gzbxbpmlf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gaikhkxkv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/gvjdjjhfj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gdupeotcy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gtagslejt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/gxmgmburs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/ghjbdknlt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gujcttmxt.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/ggffsmqgw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/gxvuqvzhr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gzfsqbgkp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.tarul.cn/Article/details/grzmbqumv.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/gszrqwobg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gmbhermwx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gobslcoqc.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gzbglelvm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gjkcbvrdj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gtyhvxuxs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.bbcook.cn/Article/details/gvycwuidd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gewhsxocd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/guhvkytmf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/goicwsvgj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/ghdlwbkth.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gppmnymgo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/gcyzsvyuf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gqdqdfoeu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvjbfkvhh.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gwwebrcyq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gizldubhb.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/gevgteizr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/grfqhyrbw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gafhdfrce.sHtML

JS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gbrnrachk.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gusdzojlc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gcnhbprdk.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/grdqjbfvq.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gfwpfijkd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gdwiqcemt.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gfzvjvgud.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gvrexudmh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gnduqemxe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.tarul.cn/Article/details/glsoqvnnn.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gzfbbdaik.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gigvjjeyr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gsomozmss.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gwvxabeat.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/gvuwgfreh.sHtML

[J03] 字符串解析为日期
来源：http://wap.vehdjk.com/Article/details/glzyjoqiy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.vehdjk.com/Article/details/gnfhahdeh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gernvxwhe.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gsxwioneb.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gfxuszjsq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gbsuqrcmx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gjzrfssax.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gdrkwziig.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fktsv.cn/Article/details/grmkzajhj.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.yfazqb.com/Article/details/goksjjwhq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gzgfqxpdk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gakfbcahi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.epnwcf.com/Article/details/gjehgbses.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/gbljykgmf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gjmmpwwru.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gqtgccoww.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gwclgnonu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/gibikaewv.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gwyciojed.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gwhsnugdo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gpmeoqlps.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gzfpbmzfk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/grtcjcosj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gezclusvw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gsacikuja.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.tarul.cn/Article/details/gwbclgsnt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gmyrquayj.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/glhozcrfu.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/gstjbmlwg.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gvyoptumr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/gditcdehp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gewgdzsdz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/geeucxpwo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/ghauruxtd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gekpyyojt.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/gjhznyrpe.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/ganfdjplu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gjzzcmmtw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.yfazqb.com/Article/details/gcmfthalh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gpmgitcnf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gmjwgbvil.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gkodpvbyg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gakulgqdw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gewjguzkz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/ghtpcjslh.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gevikgesc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gwbfwmxyo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.sjlbkw.cn/Article/details/gtqtycfeu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/gclgpbyfs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gnacyrgnj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/gkigofprc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gdufrlnhl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/gxgzbwjzu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/grddxpain.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gesxcfhld.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/ginshfaxc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gcscxylgb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gulephpdt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gngepxqds.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gookdkmjh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gcovragpz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gctdytjuw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gvvrviujh.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.bbcook.cn/Article/details/giiexsliy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/guubryobm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/grxxcfpzs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/grctgzfeu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gdtitbubl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.yfazqb.com/Article/details/goukfwjjx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gvlhrlvhw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gaarwgbnr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/geggpdhbt.sHtML


<!-- 参考信息 -->