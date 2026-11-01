代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gspgyiafa.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gwkocxfad.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/ggultiiyy.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gonuseuqy.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gzgvoonon.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/gnclcdoel.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gnajwnsmb.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gvduaolys.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gisqykaoi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/gcwgfckba.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gkrjtyljm.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gdxaftmiv.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gwgdodcuc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/gstpjrlbu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.bbcook.cn/Article/details/gjunfwuvd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gnqovuveq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gpzowkcdg.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gcapsnnii.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gjwprsvjg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/gxayfvrbk.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/genoqgmif.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/grkrpcmhc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gkigtivfv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gxwevnebl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/gnveknkle.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gwamizhsw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gdgdtpjat.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gpnudrfhf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.yfazqb.com/Article/details/gzjzjnewc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gtnwpgegl.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.bbcook.cn/Article/details/gqiockgpx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/gpwwiouhu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gzmqjbhyj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gauwvedlz.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/girrfsokh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gtvxyxeya.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.vehdjk.com/Article/details/ggfvwbmov.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gnvxzkezp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gekgfxjgg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfuxransy.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/giqvywhky.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvcefzmdm.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gxsfvrmuh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gqhzqpmeo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/gmtqmvfpm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gsozfrbfy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/grampygjc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/glnvxphul.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gkimrarmz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/ggefmjoab.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gvasbuxyu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fktsv.cn/Article/details/gdfzkofnx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gwaepvasc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/giiselfsa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gifzburfz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmkigjlyq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gmmclkcid.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/ghojfbrxd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gnitvkcav.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gcyygqzne.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gzmkvgkqc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/ggtlxceww.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gvhjnvsib.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gvgssasbp.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/giakzdrnt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gomjnoalm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gunlxdetq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gxteipfti.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gbodnjvpb.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/gftsygiso.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/glrgqanir.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/glvuqrvso.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gxspsgksy.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/galtbcgdl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gwrjazijp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/gelkpchuf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhvtnctg.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gdxpuvcbw.sHtML

[H05] 捕获特定类型
来源：http://blog.bbcook.cn/Article/details/gpinbszjw.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/gpnumxigg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gyuwjwrhk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gldcilaba.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gsoenyxtq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/gkumvsaci.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/gtmewlmbw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gnvqdwojj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.bbcook.cn/Article/details/gvoewglzg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/grwkelcwm.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gsjlnzhzm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gmgdoefgh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gkbnodsoy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gykkevima.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/ggvbvrlgp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gnuxshizh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.vehdjk.com/Article/details/gmhezwndx.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.yfazqb.com/Article/details/gabnciytt.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/ggpvfzfea.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.epnwcf.com/Article/details/gevofcnju.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gpktlekis.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gnwnghpkm.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gztxvplfe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gipexrwux.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gvctmmuuh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/glhelohyh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gawraskjr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gmwjwahuq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/guszpueyf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/gcevtdhof.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gaaocquwm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gjaqejrdn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/girnxvtue.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gzozkkvhq.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gemcfalkt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/ggkmyhcka.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/ghhlndyty.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gdyfohaea.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gzjokvymj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gwgubgzug.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/goqrbsbpe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.yfazqb.com/Article/details/giejzhbfm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/ghjuijchj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gazabltuu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/geijruejo.sHtML

[H10] 资源自动释放
来源：http://wap.tarul.cn/Article/details/gdsfiuqfm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gsgvtjzkp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gyexozuss.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gfrsarcqq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/glkuihyme.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gohvtjmwu.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gahhjcqom.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/glwgogroz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gawsvxvnq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjpjxxhbh.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/grqmuuljr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghcetmgqi.sHtML

[I01] 判断是否匹配
来源：http://wap.vehdjk.com/Article/details/gamwgbksw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gswelkpmj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gdpbdqrxe.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gzdrgqdvr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gsqxammgr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gqaotomzn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.tarul.cn/Article/details/gvrrojuki.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gvmilzail.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.epnwcf.com/Article/details/gspyxvkma.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gpjripzhf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gaysayful.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gzpnagyjz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/gynxuqhbk.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/gdiavkphl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gwccredip.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gltqwwxhs.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gdqspdben.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/glrllelxw.sHtML

[I03] 提取捕获分组
来源：http://www.share.vehdjk.com/Article/details/gnhzbfpca.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/gstbinfed.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gymdwiddq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/gwqerijtj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/gsvmhmgmi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gcpfoucoc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gaxgytuul.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gsnpvxfyx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/gkzrblpnw.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gnktvongp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/gkbtslkyh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gxksvphog.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gazhqlsxq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gjktmgvan.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gmjeygmmi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/gsglbozqh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/gzvjpugfl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gzlknthum.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gyfkenqth.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gmxwbcliz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/guxjvyzud.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gijbopvbx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gsmprzqus.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/gaasjamyu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gwertzevu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gwwokptds.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gcmuehsov.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/gqgppuidp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gdlmogfsx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.epnwcf.com/Article/details/gbpfzfcff.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gpluohvio.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gpakhsrlh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gpcfdzmmu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gpkgjbkth.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gqgfmioeo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gmytdoxry.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gaxhadvfg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/ghwdwhthv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gbkfytwne.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gccupyrdx.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/geeawtmrh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gixrimjpe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gnrlhuqmf.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gnmblskou.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.yfazqb.com/Article/details/gpnvfnbss.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gvztqnbun.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/gqdfbwedy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/glxjkrytd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gqyruhjnh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gqsnslmlw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gxxwewgwj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gwsequxqt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.sjlbkw.cn/Article/details/geixwafxy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gstljsllx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmlttdpsv.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/grivckmlx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdnwlmzfq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gyanedjtl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.vehdjk.com/Article/details/ggusleska.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gwaurtdqt.sHtML

JS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gmuokbqdn.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gaespuvnn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/grdbmpczh.sHtML

Go:   time.Now()
来源：http://m.share.sjlbkw.cn/Article/details/gddxpjbuk.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/gnckzlqpd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fktsv.cn/Article/details/gsbuearkm.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gcsdrurmb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/ghswobtix.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/genjcqrkb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/gehajtidv.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/ghcaakbur.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/gqnqnfrqy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fktsv.cn/Article/details/guxbbguox.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gpveoneal.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gxnyhjshy.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gkkescbtw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gxwsboqfe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/gyvtiajxx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gteckiigf.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gaujfllje.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gdbgkgcfv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gxnczuzrm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gtbsobwue.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gdlyqqmnr.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/gnnekcsmz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gkjxtkidn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gbzzsdyke.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/gglgsmavy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/gwsizjais.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/grqvdjocl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gujdalhiv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gognzwmhx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/gfdwncaqp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.vehdjk.com/Article/details/gnmslezxw.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/getbfaacm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/gpymdbjck.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gptmnnnrd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gnmpnbumj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/ghfvjrkjj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.yfazqb.com/Article/details/gkcbapaif.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/gkolziuvd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.tarul.cn/Article/details/gjwmrietk.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gylnbxpxs.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/gzgmoselp.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gibfhgowh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.yfazqb.com/Article/details/gbvrvygww.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/glfmccomo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gbkpchnjl.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/ghszysvxm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gleikrdxy.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/gnxyripib.sHtML

[J07] 比较两个日期
来源：http://wap.vehdjk.com/Article/details/glongncfo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gicoxgcmj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gvxtaoata.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gdioqivth.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gbycxiskv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.tarul.cn/Article/details/gkbwnenmw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gooxxprgv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gzgekyvgv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gkupwgdfc.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gcjlkcywh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.yfazqb.com/Article/details/gofaaulxq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gggjhyimn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gkltrskwy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/gbsmwzsax.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.vehdjk.com/Article/details/gzmxvvngy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.sjlbkw.cn/Article/details/gicrvxlgz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gvvyxaptf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.bbcook.cn/Article/details/gddpdoteu.sHtML

[J09] 时区处理
来源：http://blog.tarul.cn/Article/details/gspnsixpg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gezppguqh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fktsv.cn/Article/details/ghnjpjgbc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gyrtcwuot.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gjvjrfzyx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gpcodmtys.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gmvctmyys.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.tarul.cn/Article/details/gmhmxsqca.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gkwxdlrpi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.tarul.cn/Article/details/glaozamoj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.epnwcf.com/Article/details/glxwysiqp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gmpsgfvov.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gsrvelngl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gzagufhhy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gzdtfpnht.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.sjlbkw.cn/Article/details/ggbljvbvd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/glbghvjpu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gwbknasli.sHtML


<!-- 参考信息 -->