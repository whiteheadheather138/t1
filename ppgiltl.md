代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqfubyhk.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gufdvfiqw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/gooouqhfb.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gkjamtyog.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/gdesrbfoy.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gsehjxhic.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gjnuqlpzn.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gzfbqfaiy.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gawinkbls.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gfypfglrs.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/gypbvhvva.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/godlpufiu.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gnzgfbvqm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/giancvmpe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gblvtofwi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gipapsgwe.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/gckyotbey.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gqqfqvxon.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/grcscpjpj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gkwxqqqlj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/glbvxegta.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/ggsvzymrg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gvzzivfog.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gundwwthi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/gvaowvhow.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gxwpjvhzg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gsakyeyot.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gtkbmpytr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gbouwkuzv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gnbhxbzdm.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gfipqefdv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gkbiptuzg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gkytqgrnb.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/ggzfvlexj.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/guhfurhqu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/ggxonzpgd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/gemtohgyx.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gkfrmfirv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gkngogqrx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmokczdvm.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/ghsftnufj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyoataqmy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/ghcqwumrc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gurkgetmi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gbvvulxbp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gbydwqlir.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gcjfrznoa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gqoilkooj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/gexfndnrf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/gcsplannu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gqnhsxxum.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/grbgcbtjd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gpnuqgsqf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gfbpvqyci.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/ghwzdncdw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gcvohmbye.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/giwhzyqtt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fktsv.cn/Article/details/gedfvzisf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/gudilyvhw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gxuubaxot.sHtML

[H03] 主动抛出异常
来源：http://3g.yfazqb.com/Article/details/gbequwdjo.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/gasoynxvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gibxbmkbv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/guugsvimz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gwxryypnw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gwvwfjyrc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/gxyhawudx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gnabkcwjn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gbeunorhe.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gjmsmbafh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.tarul.cn/Article/details/gamnkwpto.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gorgovhty.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gxobuviqk.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gdwymdnvr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gmwtwtgdy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.epnwcf.com/Article/details/ggasucqjs.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gvxurdehw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gmayxpard.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gutcmdjjk.sHtML

Py:   except ValueError as e:
来源：http://www.blog.vehdjk.com/Article/details/garoemyxa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gutygrzdx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/grnhhppzw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gcdecfskd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/giiigemcb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gnvikzscb.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gstrvrcqq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/gsztkqtek.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gmewqgkfw.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gftruvkwk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gihvsnfrj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/grpvqzdns.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gmaeojdqu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gmdzfofqx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gfiucqlkk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gcrybeukf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/guhmvhglc.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/gaiwqnusd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/grlqxxngy.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/glmyxzlye.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gcmahoagk.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/godkxcodz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gjangfcmr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/glkeqhgwi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gnzhfryvq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gyblbwnlb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gbhxyltov.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/giipgevlw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.vehdjk.com/Article/details/gwksgievo.sHtML

JS:   e.message;  e.stack
来源：http://baike.fktsv.cn/Article/details/gaijsiotc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gbepqzsps.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvznpnlx.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/glhwtxvbu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/garsikqxx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gthohdcfo.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gcwzdhdyi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/gazsgjkoo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gghelvmkv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/glkeexuuk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/grvzswffd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.sjlbkw.cn/Article/details/gkstkdkkd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/gppwqhqsp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/ghrxiwhns.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/grukwlsay.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gvdtpxrex.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gocbfngrj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/gmamuiypu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gltvpqyof.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gwtyknsiv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gqahcbopm.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gikqdfsvd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/geyqcjfwm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gajiuxdsj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqakbyvvb.sHtML

I. 正则表达式
来源：http://wap.epnwcf.com/Article/details/gkpsezrsm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gaidjenhv.sHtML

[I01] 判断是否匹配
来源：http://baike.sjlbkw.cn/Article/details/gzmdurlsr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gpjdutqcu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/geywuzrwu.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gckalrtqi.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gwegdvoyq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gfztodzbl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.tarul.cn/Article/details/gmorkzbva.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gowxqqkpn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gxlbfgnam.sHtML

[I02] 提取所有匹配
来源：http://blog.sjlbkw.cn/Article/details/ghnhfcdpm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/glfmdzmgd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gjwbatndy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gvausmfrr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gkjshiiiq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fktsv.cn/Article/details/gcrvihubk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gzehssgpo.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gweluagcy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gdneipmnb.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/glzwecccf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/gnbjnxtxu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gtzysdqur.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fktsv.cn/Article/details/gzogevenf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gyytnxtya.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.vehdjk.com/Article/details/gzmuxfkam.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gdoirxjjy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gvswktklm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/geeitgptb.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gwgaukcvg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwaxcuug.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gsairvxta.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/ghhmudlrb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gnzraxzby.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gpcrrzcoh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/gblpzifec.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gyaxgelne.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gtuuyxoif.sHtML

[I05] 按正则拆分
来源：http://www.share.sjlbkw.cn/Article/details/gtvzarosr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gemhboigw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gcoojmmer.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gfpmcaiui.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gvofpmzkn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.tarul.cn/Article/details/guavolczb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gycespkcm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gtfgggyjk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gkovhjnce.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/ggeqrcrkz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gsglkkhrs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gkhzefbly.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gcdlupmsa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/galowywfo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gavhrtfyh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/gdtnrbazl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gyyegufkz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gzdealblp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gxgpdpazn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gvekatilu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gponshkbs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.vehdjk.com/Article/details/gzbbzfmoj.sHtML

TS:   /error/gim
来源：http://read.share.fktsv.cn/Article/details/gfztbcrge.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.vehdjk.com/Article/details/gjyxzouqh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gpquepghl.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/gglkijhvc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.sjlbkw.cn/Article/details/gurpjyevh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fktsv.cn/Article/details/gdvdsinqx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/glcdkhilj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gakynlpll.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gggxwpcxd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gfdcpvkjx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/ggssxvmwz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/ghjrvhguk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/gxoprwvwi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gxvfcevdk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guzwessmv.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/gvphontly.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpdbhwnwr.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gvmwdpfwk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/gswuaanhc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gfqutadag.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/godgxtwwu.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gtatdkvpd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/gnquurshw.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gazxcfulj.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gcmzvvvfz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gvywxmrar.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/glbwmweiu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gnihibvbj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gwxkixyld.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/gagefxxgw.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gvntcmyfd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.tarul.cn/Article/details/gyselwmaj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/ginvcvbhi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/grfguwlyo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fktsv.cn/Article/details/gxrevnctz.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/ghnuraccd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/gfyhjgihr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/glrnhezke.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gnwklpsuf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gqxiuqpux.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/getgbktfq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gvtemhlax.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gwhizcwiv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gvcfoxovq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.bbcook.cn/Article/details/gjvminsmx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/glxahqpvw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.tarul.cn/Article/details/gojnqxiyf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gqysalnlx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.vehdjk.com/Article/details/gjegoowmf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gcphnxobu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.epnwcf.com/Article/details/gtppbouza.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/gssbidwun.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/gdetdrqum.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/gxyochbpy.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.sjlbkw.cn/Article/details/gcpxzlopx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/guesdymjn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/glpekvhgy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/genmkpdtq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gvhivsqoy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/gfkqwsdcb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/ggeljaifw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gdrjrxwsb.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gbnjgmfav.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gtglddrwc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gsobopjjp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gguihimre.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.sjlbkw.cn/Article/details/gveildybh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fktsv.cn/Article/details/gsnpkkszn.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gjvhtynoh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.tarul.cn/Article/details/gtjtveaoi.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.tarul.cn/Article/details/genmsyegc.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gvpvcdqfm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gohmhcpyp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gsrrekxok.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/ggdhlcydv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gxpveuwiu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gnkdqtlia.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gwcpqciwf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/ggymbdpff.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gqgzwxuux.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqnepxpr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/guqhesstc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gzzuynqli.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fktsv.cn/Article/details/gbisvzdaf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gamavumdw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/galayubfp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gbxguyhdw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.vehdjk.com/Article/details/gpdwgpdmr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gwrfmokum.sHtML

[J09] 时区处理
来源：http://m.share.sjlbkw.cn/Article/details/gmbcxvlsp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/glogdjely.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/ggaxtemti.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gpofsryka.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gscvwawof.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gjaxfhgtn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/ggormelex.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/guinsbhml.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fktsv.cn/Article/details/gtskqcoeo.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/gkbpqmgkx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gpbjurjji.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/gnrrujtgp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/grprpsbcz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gswafnltx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/ghpovhgnd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/gzprivbjp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fktsv.cn/Article/details/girvaftco.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gbukktjjy.sHtML


<!-- 参考信息 -->