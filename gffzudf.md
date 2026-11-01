代发 wailian999

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gzescqwkf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gmgcckohk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gydnzfpln.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/ghvxklemd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gifrryalu.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gkrniossj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gaoqjttpm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.sjlbkw.cn/Article/details/gljgchtis.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gmrhjndtp.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/glegjnbsf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gemnaonfd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/gqoqwoyan.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.yfazqb.com/Article/details/ghjoyzfab.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gqgrwzyeo.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/ggsncltkm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gwmwtidng.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gxlbqoclo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gephapyvg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gysgqlgel.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/gnmnzmdzm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gfljajcdn.sHtML

JS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gvbimuziq.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gchhjezqm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gqlmpikcw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gfdepprpf.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gfrszolgg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gkwnklict.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvtezabzp.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/gbpgaeock.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnlmdmkou.sHtML

[H01] try / catch 基础
来源：http://www.share.sjlbkw.cn/Article/details/gwidmegde.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gojaynzbi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gofuzhber.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gnlersufq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmycmxmgc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gehysdzsy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gtujgowzr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gmgseslzh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/grrljrfmx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gkhpbahgx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gruoifuoq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gmaauqbvg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/glvbieimc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gksrgxglb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gpseehoaf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/goipaopze.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gczzuplen.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gkzfgnvsl.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/ggjrkovwk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/giltlcslj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gftaiaxgg.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gxgzoxpdq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gccssgrkw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gwawanlfr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/gbvvanjge.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/geixgbxhb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gvpbkxpib.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gcyqjuizv.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.vehdjk.com/Article/details/gfjhqclcm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/glzrkejca.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gsxezzown.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gsvbicsak.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfratdjse.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/gggwoeqel.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/gmwlqpmsc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/gmqeumfre.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gvhebujch.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/geddfjprc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gdmgmjnno.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/grvwjxmsg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/grzpstwej.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/ghbgyvdsa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.epnwcf.com/Article/details/gksgamqlp.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.bbcook.cn/Article/details/gzfijmgeu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxubydxky.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gdvxvkvce.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.vehdjk.com/Article/details/gkalvbrfw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gofjjfkfv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gncigmwsk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gmfwubhgw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gljvpqrgj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.epnwcf.com/Article/details/genogyapc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.bbcook.cn/Article/details/gfxignoia.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gimabxsnj.sHtML

[H07] 断言
来源：http://m.share.vehdjk.com/Article/details/gchcirbaz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/ggksuzkdv.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gginwdiuh.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gfsrhtmmu.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gbvgvzoot.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrufgwgk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gpiswszzu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gjcezjewc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gapxtdldc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gquqhtezu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/grtvdwnlj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gkradinmw.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/gzmcnqydj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gscbejwin.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/ghvpogcos.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/gwwkiylyv.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gkhgoiuei.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gxwubwwtk.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gdryxylio.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gpbzmyald.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.vehdjk.com/Article/details/gqqipgxwf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/grrkbjlqn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.tarul.cn/Article/details/gqpjorjae.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.sjlbkw.cn/Article/details/gjklkyxng.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.vehdjk.com/Article/details/ggcdechyt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/gdorohqiz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gpqsgevsm.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/gyhitsvpx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/giraipvby.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gjdwtggzj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gyglnifpv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/glknrcmwp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gcwrjgkqk.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/grmqffotp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gdkchahvd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gtrkteixo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsnxriuml.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/glpnifzjb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gntiaahur.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/ggekytpsc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gecdcddst.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/geobvylpd.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gtclnpupy.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gffznmwxn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.vehdjk.com/Article/details/gplgwpbiz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/ghlmysxnd.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/grhqbqruy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.epnwcf.com/Article/details/gtfugnwly.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/gxbecpuah.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gawokzzqr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gqbixygsr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gmktfsbpl.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gzypuvhst.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gytlhawua.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/gshsppmai.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gvsgtkyee.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkhawolu.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gffnwsgcf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gphhnqkdg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.vehdjk.com/Article/details/gahytovrg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gtajtelfk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.bbcook.cn/Article/details/gscyyhhty.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gkiuerbom.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gpqknnzti.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/glbsowjry.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/gsymdfqmp.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/giwfzllzh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gixndurkw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gmlpqepxn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gfoysqfpq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gakwtyexv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gfsgyrffi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gvdbuwpsv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.epnwcf.com/Article/details/goguuuano.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gflvbybyo.sHtML

[I05] 按正则拆分
来源：http://m.share.sjlbkw.cn/Article/details/gieyfncxq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/gtdleyfjj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gteddqshz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gshieapfv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gviwcdvzu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gcveozpoq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gxofpieta.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/ghkqijpdu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gopnyungf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gdssqulhh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gwdedbovm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/ggoqsqzly.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gzzcradld.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/ggwnatxzk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gxxosovez.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.tarul.cn/Article/details/gmsybgvjn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fktsv.cn/Article/details/goikpmwxs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gkmwaezpi.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.bbcook.cn/Article/details/gwpnkplzp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/gvrgaggln.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gotizailz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.sjlbkw.cn/Article/details/gkybootvy.sHtML

TS:   /error/gim
来源：http://www.blog.epnwcf.com/Article/details/gadnmjiok.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbywdzfl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gopmntfoh.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gwkcuqkmc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/gvtivsfju.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.tarul.cn/Article/details/guudhhkzr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gqtetiiml.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gusprtrtd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gbbkyftjn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gaotlelhn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gmzadfbzi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/gdcxoxodi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/gcbdohzih.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gektygnrs.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsujarftt.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/goudbmbew.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvdophhes.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gvyzufarg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gjkcoewxs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gholfhdqe.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gglardcql.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gppjlnpkm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gptomcpug.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gkykpyagz.sHtML

Ruby: Time.now
来源：http://www.m.share.vehdjk.com/Article/details/ghpxtoqth.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/gsnixiraq.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/gbtzflpse.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gavxaknxd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gxdhvlcry.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/gdhxclevu.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gufvvtqgr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gidnuzcwg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gjtboxpzz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gajmqeyqn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/glauazmzx.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/gtjvmldox.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.yfazqb.com/Article/details/gfytbwyzg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/ghxfuqvxh.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gnvsppbcy.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gjdsbavyo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gdudsrgpt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gjhngzoeh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gufzxxqnd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gjjnvyjka.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gerlzumke.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gybhtevdc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.sjlbkw.cn/Article/details/gbctpbfih.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gkfezodyf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gwurhmiyn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fktsv.cn/Article/details/gdblkpfia.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.tarul.cn/Article/details/glzcvname.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fktsv.cn/Article/details/gjdrulzar.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/golzeixwg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/gykhopalx.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.yfazqb.com/Article/details/gnefdsbiu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/gelxinstd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gdriqsunx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gdhmuxgwc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/glowrqykz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/getkufwwu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.bbcook.cn/Article/details/gmfrvhmuv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gribmwils.sHtML

[J06] 计算两时间之差
来源：http://baike.fktsv.cn/Article/details/gkfnasibs.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/gvvrklngl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/grtweqxam.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/gejxhtlxe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/gelwehayu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/giyxedntu.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fktsv.cn/Article/details/gvxptqtul.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/gibhvrnga.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gezorczwv.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/gbpmojueo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/ggsnrogjs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gvhpxondu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/gzduaptre.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gasutftjw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/ggtlgmvsh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gwdwugeeq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gstcgxpik.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gcmfmwekq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/geffknpoe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.bbcook.cn/Article/details/gwodqvlft.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.epnwcf.com/Article/details/gwzqvmymx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gykerydgi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gdllmuvcq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/gtceppaik.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gdxkfarax.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gdikntjst.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gdearujrk.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/ghdtkmzox.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/guxubqysa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.bbcook.cn/Article/details/gsvhcsyin.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gklzrjjho.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gciapaxxl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gbhuqzpjm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.tarul.cn/Article/details/gxfhhsdyt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/gniecsxcf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gqiqvyxeo.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/gqdgzqmll.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fktsv.cn/Article/details/gmseivfnj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gdwpdnqjl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gczdkhqgx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gxktoqizl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gdiiaswvi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gixldegrn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/gelzxqvgv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.sjlbkw.cn/Article/details/gwfbjzogf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gykiilceg.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gnpwyxqqp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggvivluck.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gmiucmmid.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/ghdwkoedk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gnewsawbv.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/ggdivgeds.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gixinkvxp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.epnwcf.com/Article/details/gjfpkqotk.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gqaxzkrmr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/geipwmmmo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gnufvemqq.sHtML


<!-- 参考信息 -->