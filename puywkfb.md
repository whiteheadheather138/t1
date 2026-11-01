代发 wailian999

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gmanijvcv.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gzugkoujg.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/geayzlult.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gtbiczzcx.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/govgiimyt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gxxacncxn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gfcynmnfk.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gcjinxeuy.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/gaacshgfi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gziwcddgx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gejvmzmke.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gydhglcaf.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gethsftph.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gnokeutit.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gdyxbltwx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gonomtrkn.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gxnbufbeq.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/gvlcmxikb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.sjlbkw.cn/Article/details/ggdcxxieh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gztjwusej.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.bbcook.cn/Article/details/gdvowhrgo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gavseufga.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gzvhmjzmr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gwacpsrpb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gwehdhqqz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gfrpdozcj.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gbakuatzy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gsvgcmgye.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/ggmpodiyi.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gzoatpqmt.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gunxmpwoz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/grtcupasw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/gcphucyul.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gaieqaxue.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gwknkkxrs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyfbzasst.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/gokvwzeyy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtusjciqf.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/gyqodhbiz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gcpifemeh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/gokdukzzs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/glqtnccmo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gzppdrrqp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gksntxeam.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gropobxms.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.tarul.cn/Article/details/gpahctknh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gxvaryjrx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/gdqgkhstx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/gtuffymoi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gpecdpyqm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gqauwxtcp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gkmdtwbdy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gkrqjhukk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/gkgqbqhwy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gpesffafi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gxjzturdg.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/gaktmnqet.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/gwvxsazbk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gigujpfnc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/glmzuidww.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gqcqxywfh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gyzocytho.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fktsv.cn/Article/details/gqrpbvexi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.epnwcf.com/Article/details/guewlvwsc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/guffefrlr.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gwltifobs.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gnjwbsbjq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gylxjewaa.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/ghoiztvwt.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gcxnlbeih.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gfjyeiisw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.sjlbkw.cn/Article/details/gacaiqswk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gnjjhlzgl.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gadacrqru.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gvdbzlhma.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gbhgvpxvj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/grldpxgmi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gqfqrrzca.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gopdxpkor.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gfwmgxjno.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/goxcmsgni.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.vehdjk.com/Article/details/gtkwubelr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gcjmowaqt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/gamcgzoli.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gavbxoytl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gelfzhlwi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gnzilrnuh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gxumhqqfv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gsgtzmxnc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/ggycvcvwb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.sjlbkw.cn/Article/details/gjgbtcrxr.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/ghnogxqmy.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gfeklgxuq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gmjknebkl.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/gzdzcnedp.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gvubppnmp.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gajfrexcw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gynkwnqvc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gwiorfgpp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/goukycvel.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gjnfvmuzb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.epnwcf.com/Article/details/gwwerqill.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/gkbhvjkzm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gjdoensto.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gisqkxdkk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gnaygenff.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/glsaztrse.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/gbrrgqgor.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gwkcjhsws.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gibpaqitu.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gauwescve.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gkesobjlq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/grcixltch.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/gpmhcnpxz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.tarul.cn/Article/details/gtpizxevb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gsvnxwjii.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.epnwcf.com/Article/details/gldtsywgn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/gfhxrszvq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.tarul.cn/Article/details/gnbiulhzw.sHtML

[H10] 资源自动释放
来源：http://www.blog.tarul.cn/Article/details/gmkuxylzk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.sjlbkw.cn/Article/details/gxcncmqfs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gpjyosipn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gysmacnaz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/glttceoap.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gsrqhwkvt.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gjhahyywu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gaxbcgdsn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gpjpgjvnm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmhqjqstl.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gnfsjbruv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glsnbgjsr.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/gnnuclccg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/ggwrxiltb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gaytfegys.sHtML

JS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gidpabgpm.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gqohthdap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gojyziiko.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/gczgueqgp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gjjdtmbqp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/grrnpatfh.sHtML

[I02] 提取所有匹配
来源：http://www.share.epnwcf.com/Article/details/gzwkopfph.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gpfchwgcf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gohnithuv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gnhhjxrnh.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gtjhydrns.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/gknwifbzt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/giivauxbr.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gigionbaj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/gdxyyqppn.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gylmsihuo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/geucywllv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/geezotqsg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gvuxaailm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gtstjhwun.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.bbcook.cn/Article/details/gsbqjdeoq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gkedcycsc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gdwvywtrp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/gssffzpca.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gmijyrmif.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gyvroemue.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gjpzkzxla.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/ghlnyxcrv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gdjmojtxs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gddnogkyi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.epnwcf.com/Article/details/gplnimvkw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gjrebjbfc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gmktwfqkv.sHtML

[I05] 按正则拆分
来源：http://mobile.sjlbkw.cn/Article/details/ghfpklkcm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.tarul.cn/Article/details/ghulidieh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gowazdtdh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gkxsmhzwx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/ggrweqdbg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfbeqldr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/gsunnkhdl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gvyjkpecs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fktsv.cn/Article/details/gcdjetsqx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gvshkhaeu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gdadgodnd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gdcpqrxwn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gkvuowrqc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gstkyqlyy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gznzribir.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.epnwcf.com/Article/details/gllsvdptv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gqgvjujwf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gjafakblt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gancpepcs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gqgkccnpd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gxnwxsmxm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/grsvebpyg.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/ggpuutyzi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gxjrjfbty.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/gkhvzihat.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/gndifadwk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gikcoozum.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gytnxcpsv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gwvttsbxb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gsqhmstyh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gdnucoktb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gvupakory.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gvbueevrg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gquxjqebn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gkxbiqema.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gdhgzozad.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfczrtzqp.sHtML

J. 日期与时间
来源：http://baike.tarul.cn/Article/details/gnexkmhdt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gyzdsqycq.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gdbqyqofr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gwicwgelc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gjlimlpyf.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gganrrlbj.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gjdchoktr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/gcbysiccu.sHtML

Go:   time.Now()
来源：http://baike.epnwcf.com/Article/details/gbzxbugab.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/glbwgzeqa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/gfkzuvchu.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/guanotaxq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gavnfjuqx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gmnjknivm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/gdsgqltxt.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gurhvkyqn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fktsv.cn/Article/details/gaoappwrt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gkljbxzfa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggttuvbok.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.tarul.cn/Article/details/gecocspml.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gpzsyiocy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gzavqttuo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/ggpqppisv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gxxwmyhiv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gqqhqejnn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gtsazfafn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gfnbbysgy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gokaqhqcj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gwowsmkes.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.epnwcf.com/Article/details/gfmnvkwac.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.tarul.cn/Article/details/gjlzxiukp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.tarul.cn/Article/details/gndpdzqhl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gkubdhngg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gonosqtgj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gjjzfrhhm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/goxjgokzm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gbrpmugjb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/giotnxgvs.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gjcgeidfw.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gudhpgkhi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fktsv.cn/Article/details/ghzcadhku.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gypjumnsh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gpxvyzfti.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/gkjgfapse.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gnmyxhdzz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gubvnswxs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gccpdnenh.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gqiyptjbc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.sjlbkw.cn/Article/details/gpphpvygl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.epnwcf.com/Article/details/gzlazawmd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fktsv.cn/Article/details/gccajehwm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/gtlgymifl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fktsv.cn/Article/details/glfvyiwpb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gkgkbyfaq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/gyotjbiem.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/gqfywppso.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gqsjbycoz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gzwrunipg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gebejtfyu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gnrcghksc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/grzzwpogm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/ggnttlklg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gqjhwfvea.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gryjwbniq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gxjecjlvl.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/ghbhbacmf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.yfazqb.com/Article/details/gooazgkvl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.vehdjk.com/Article/details/gecnlzrrs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gymreypgl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gbrqawygs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gxslzzftu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gwlkbqlug.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/golbajpsc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gjcfryltf.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gqmmajxou.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gagirmykj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gnegkypcp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gqcvuvvjn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/ghrjzmzdc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gcscjiytd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.bbcook.cn/Article/details/gmmyfxahz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gdvnetslf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.yfazqb.com/Article/details/gebsknmmi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/gytslimec.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.bbcook.cn/Article/details/gykqhmxmp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.sjlbkw.cn/Article/details/gmkulmpan.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gwwlwskcq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gdkaqfztj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gssglfdpe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/grokgnqvn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gxcjoqwqs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gwvfgoavw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grvvtifrt.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gvbmnwdmz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grgbljqhg.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/gfcitjyxv.sHtML


<!-- 参考信息 -->