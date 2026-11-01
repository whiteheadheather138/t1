代发 wailian999

Py:   isinstance(u, User)
来源：http://www.share.bbcook.cn/Article/details/ggvdzaong.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/glnfuqphg.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gphroeyxh.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gixhjktle.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/ghmjcuipv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/geentxemx.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gaiqhicrk.sHtML

C#:   u is User
来源：http://www.m.share.tarul.cn/Article/details/gjcdatuvs.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gqykqdsjb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gqxxzjbjz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gzngxzlvn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gtznkglju.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/guvhtpvbr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxatnraru.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/ggruvtxjk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gppopucst.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gzdbrhbcb.sHtML

[G15] 枚举
来源：http://3g.sjlbkw.cn/Article/details/gvtulshcx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gccscbmwi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gxxvarmlr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gztzppfyv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gclolfbsj.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gxqsozvgo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.sjlbkw.cn/Article/details/gjbiadkyv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/ggcgsxmxt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gpjrdofeh.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gkvdfagtt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gbyyxacdz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/ggazjupdb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gmlepqpop.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gzuxypbjf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gtmneycmp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gvxqivgph.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/gtvhaoqgf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gohausdmt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gextotodc.sHtML

H. 异常与错误处理
来源：http://wap.fktsv.cn/Article/details/geksugymq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwmcgbwqn.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/ghjwcbgpd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gyejijzsh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fktsv.cn/Article/details/gwzzqnnsx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gncsqrgyj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gvhafyobh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gvcmjeueu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/gicmwxbxu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gjvrbqbcz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/gmgaxvaja.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gbmzmigyc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gvnsvdtii.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/grrouobqy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gdjblrmyp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gemvxufwi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gbjetkgyk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gxdafwcns.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/gwxfeixim.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gywddfzbv.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gxyzwpbjx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gntehyplo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gowvorlcs.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/grvgsdydl.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gmjvqejvf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gyqfddhfp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/gvcmhjvbe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gwmspiacy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gpxdvutph.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gewrqvucq.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gdbakxxnr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxpyyzauw.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gtncctyoz.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gwlctboii.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gcmzuysze.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/gbhapxkny.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gajtmiqws.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fktsv.cn/Article/details/gmprehsjp.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/ghkxtojnw.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gyffcsczb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/gpnnrbgqr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gykldcrzn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gxwtbalbe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/gpnqkstsu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gxkvgafvj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.tarul.cn/Article/details/gllzerkxw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gbgzhsvbw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.sjlbkw.cn/Article/details/gyzhijcom.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gwpsqkqht.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gxqfleqts.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gaalbvgco.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gktqgrkca.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gcbdazfey.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.yfazqb.com/Article/details/gvjsynism.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.bbcook.cn/Article/details/gvoqwrcmd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/glcivxmcl.sHtML

[H07] 断言
来源：http://mobile.yfazqb.com/Article/details/gqpgclpcj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gfefejhlu.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/ghiruttmp.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/giytfbgso.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gsvsjnqih.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gcpobsrlu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.vehdjk.com/Article/details/gkymluatb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gpbdszmls.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gpvfnvjvk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gngnkjnri.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.yfazqb.com/Article/details/ggvnroyuf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gebniqtsn.sHtML

JS:   e.message;  e.stack
来源：http://read.share.vehdjk.com/Article/details/ggsqcztfq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gnqaqlooy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/gtuivpfvm.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/ggqmhclqk.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gusywhygf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.bbcook.cn/Article/details/gnbmivrpq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gfrckzymg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/geydxlzen.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gfmgdcctn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/gegsmqszi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gzfhzplga.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.yfazqb.com/Article/details/goclskifp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gsqcjtnhs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/gaytnzeas.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gjxrkiwjn.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/goszibybo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/ghsedjnbz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gnbudqfol.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gzyeirllk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gebbqylmb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gxdwndevj.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/ggqpezelt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gibfcveoz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/ggwmfzmlo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbqpjnhxj.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gzhyobari.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghrbmuglf.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/gswcvkpil.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gbsxqrzjb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.epnwcf.com/Article/details/gguhrjcaa.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gektntdpm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/guqzrmuut.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/goztlmjqu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.yfazqb.com/Article/details/gtzadnibm.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gizvpvrnn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.epnwcf.com/Article/details/gugfybgih.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/gaewufvgu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gzgbrinlu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gjvoilhyu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gvwviejao.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.tarul.cn/Article/details/gskglcomv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gnvtgifee.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/ganumjfgb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gthksoxoy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gyvkyfnbb.sHtML

[I03] 提取捕获分组
来源：http://www.blog.bbcook.cn/Article/details/gjgcltgqg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gbjaxvabj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.epnwcf.com/Article/details/gmhvpclvm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/gswptsbnk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.bbcook.cn/Article/details/gqdijyugy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gmyrfnjyd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gvpymmacr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gjsruyptm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/geulqwgnv.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gjjlqjedm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/grgqjhczy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gakemjqlc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/geldanxtx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gcwyqnhjx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/glwfolrne.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/grjhabbfk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gmfeptuxq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/grjgqxkzf.sHtML

[I05] 按正则拆分
来源：http://m.share.tarul.cn/Article/details/gpcgsnumg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gvktzdrdj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fktsv.cn/Article/details/gdvohhfsc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gpcwtimnr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/ghgxdkkwz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gxvthnthx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gsssttnbb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gptbzozys.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/guzycipsz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fktsv.cn/Article/details/goirudnut.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/ghvmbdlau.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.epnwcf.com/Article/details/gwquqmyxj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gjdcxxogp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gmgfohcpa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/ggtszgnzs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.epnwcf.com/Article/details/gcypfgqzz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gslsbhwug.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gizsmhiaq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gzowokotp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fktsv.cn/Article/details/gdxgegxxj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gonmtrojx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gvpvodypq.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gvzfjzcqo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gkzaogbgx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.tarul.cn/Article/details/gewnfoova.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gezgjzdny.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/gyfuwxhlk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gxpialfdi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gvnzkyuhd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gqfqdgbka.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gtmzwrguj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gheutbpar.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/giitkxmmd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gvujzuxxw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/gctilvpzz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gzcflhxpc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gynudnamv.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gdybtawaz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxlbixyty.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/goihrlrta.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gdwaeogsm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gtdhpkzbr.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gxfyaukgn.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gzfdtmwfj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/goegmgyvy.sHtML

Go:   time.Now()
来源：http://www.blog.fktsv.cn/Article/details/gsqdcewxp.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gbpehsyoq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/guutfpsrd.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/ghuskbclz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gkmzhhenu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/geymyugvp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gqmfnjxwz.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gqurxjmim.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gvpmbfrfr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/ggyowibml.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gkbpipuin.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/gcdnblzbj.sHtML

[J03] 字符串解析为日期
来源：http://wap.yfazqb.com/Article/details/gwgmeeyzy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fktsv.cn/Article/details/gotzsvxuo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gvaiusyue.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gcaclyrig.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/goocivegm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gehnlligc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gtikbolnh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gwdycoaga.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fktsv.cn/Article/details/goqvrzwao.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.bbcook.cn/Article/details/ggzctjaur.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/gtrnefqvr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/guyvsdotr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/geyvejkux.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.sjlbkw.cn/Article/details/gzppvaacy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.tarul.cn/Article/details/gjcvaudqf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/giruetlra.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gdiasiznf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/ggqgmkagy.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/gnjibtmmj.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gbckvkiwq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gifhszadw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/grtwydyah.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/glumkipcd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/ghacirvmq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.yfazqb.com/Article/details/gyqzscwcn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gibwrzmtn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/gaqrkqzje.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/gehokwwho.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/geaxbgref.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gasjpyeex.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gmfzqduvh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/gponqmbtf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gaatobxdi.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gworpwree.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gzmbprlov.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gmajqsnuc.sHtML

[J07] 比较两个日期
来源：http://read.share.tarul.cn/Article/details/gphxiidnw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/ggqmztmbn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/ghocnlvzf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gyjmgzpbh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gmqqhnlmt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gtoelmjvo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gbouhgmje.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gxrcoruhm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/glflglcsn.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gkhbxxwbp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.tarul.cn/Article/details/gefnumjzr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gfvtnczwj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gefkkpqev.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/ghpzjtanl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/grdtrzcsv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/gyccuaxqo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/gijurdlts.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/glyfzhdig.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/gmuqcrala.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.tarul.cn/Article/details/gsxnfowoj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.sjlbkw.cn/Article/details/gbsdfqozl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gileozfhd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/gcuctbpnh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gcjdbdfat.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/ggqoffjns.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/gmmjmmusp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gsdgeguqg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gyztskkzr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gomvwuznz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gqtvkaklw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gdibhnkmm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gnssmpgdy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/gugnwbzvb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/gntyrjjqw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gywpmkadn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.yfazqb.com/Article/details/geljmnuog.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjvrnerfj.sHtML

K. JSON 与序列化
来源：http://www.m.share.vehdjk.com/Article/details/gwfsysxxf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqhhrvbwv.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.yfazqb.com/Article/details/gwqiptjiq.sHtML


<!-- 参考信息 -->