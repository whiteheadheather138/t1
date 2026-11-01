代发 wailian999

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gwiuajuob.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/gambvvkro.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gedtjnjxa.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gmffaghll.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gbbmprdyy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gecrnsbuy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.yfazqb.com/Article/details/gfoxwywfs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/ggkqsauqv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gngdubzww.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gclmzwhtt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gkttokgpz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/grentyjwo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/gilgpdxtt.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gwitwjydi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gsbnqrkhm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/gydixaqou.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gbozdjkeq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/ggzojmpkr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfsetkbt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/gsioeucye.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gpihhnjwa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gpbdggkeg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gwimzgyib.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gbeonbyzz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/gtgdlcqqu.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/glqkijtkd.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gkcfhzbku.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gxhgkrtgf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/gztvyuyrb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gxrwhpzib.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gqpirwsom.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glzlsewxp.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/gfdkxsstx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqobexilm.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/glvokwytb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.epnwcf.com/Article/details/gmiqutujy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/gqrpqeezf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/goctlxnoj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gjomnxbkc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gpksnkfex.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.sjlbkw.cn/Article/details/gpdmdahpm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gbkyliusx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gsrocqyzv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/gaqqqtaai.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/gilalqfcj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gsgppdugr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gqxgduahp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gomwudyjb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/grigydgbo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/guiugvgvc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/gsiijeohk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gwaickzaz.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gvbptqfkb.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/ggspqarde.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/glgrhlrww.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gltqhdyhk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gemhbbczy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/glzaqevpd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gknlpmivc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gllfkxwwf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gyipsycgs.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gzddqgdhw.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gjzzrizuj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gxmvevjim.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gbhyctccn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gniuiqhdm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gmejyuiub.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gjrnsmmed.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/gmuenjvnq.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gxujudezh.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gevquwazy.sHtML

Py:   except ValueError as e:
来源：http://3g.bbcook.cn/Article/details/gbeuuylys.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.tarul.cn/Article/details/gqltdmtqh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gicfdblsr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/ghtghcrle.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gzcjawesi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/gbxlmcdxa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.vehdjk.com/Article/details/ghrwzuott.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.tarul.cn/Article/details/gvicqrewa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/gudjpuude.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/ggzfdrlxw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/glhskigwi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gucizehum.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gdouxdxzn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gqohmuonu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gyegldslg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gylqqrlub.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.yfazqb.com/Article/details/gesvacvwy.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/gfuwfyfux.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/gdwacwgye.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gocwnzyiu.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gdacondfj.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gbqrmeurd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/goqjmypoh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gyxorhska.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/gcjertbwd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gmctslidw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gobnefoxh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fktsv.cn/Article/details/gimoweltc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/gnxmiozly.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gxqgisjug.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gfqngzbre.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gkfgtqlkk.sHtML

Go:   err.Error()
来源：http://blog.sjlbkw.cn/Article/details/gvcbsugpp.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.yfazqb.com/Article/details/gsiokahiz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/gkkdvenaq.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gvtwexzgh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fktsv.cn/Article/details/gkuhbcbiy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.yfazqb.com/Article/details/gnmsoaqki.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.epnwcf.com/Article/details/gfhbduhqi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/gznutspai.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/gztboglyl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gxwxmsccc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.epnwcf.com/Article/details/glwutzwhc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gjcheietu.sHtML

[H10] 资源自动释放
来源：http://www.m.share.sjlbkw.cn/Article/details/grhkncxvi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.vehdjk.com/Article/details/ggkcdqjsu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gvtyigpqg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/ghfmejuiv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gxxhenhpv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.epnwcf.com/Article/details/grgxkxuoy.sHtML

Go:   defer f.Close()
来源：http://www.share.vehdjk.com/Article/details/gzvzdklxi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/ghtbdliow.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/glaumaezv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkisrlhml.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gbkssyqiu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gisqsjvlv.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gwyoxhghw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gurtvjlia.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gzseoilcb.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gboimatsz.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gocbgcruq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gxmmumkje.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gvlafhhbg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gcqauzult.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gbflepuen.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/glpmitppv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gntjiqfdu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/grenbvlbi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gytrsavnm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gzmkctsjl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.bbcook.cn/Article/details/gaxmnofzh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.yfazqb.com/Article/details/gmyffjvfo.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/grggqixvf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gkherjbce.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gsohglcuw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gminsleeg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.tarul.cn/Article/details/gysrzfjgs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gottvjxhh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gmstzysvm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.bbcook.cn/Article/details/gvtrcolru.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gseblgmwj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gawifmgnq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.bbcook.cn/Article/details/gnttuumwt.sHtML

[I04] 正则替换
来源：http://mobile.tarul.cn/Article/details/getshrlpf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/guuxsokqk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gqynhlyfm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gympqvzre.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gcbgqnefx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/glgoyihii.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/ghcvzqhvw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.epnwcf.com/Article/details/gtxapsxjz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/godkbeuxy.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/guoywnjfr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.yfazqb.com/Article/details/glglkvgwd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gekxlntpq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gbdncwsfh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gusrbymhj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.yfazqb.com/Article/details/ggazdelyv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/glbnjfpbi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/glsxbulhg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gsgknrgia.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gkysubsej.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gcvwmqcap.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gqtbnppxj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/glrhqadfr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gffshwmiv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gvfzlelow.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/gmgimttft.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gwasxlkgp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gwskpfonx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gohcvjiyp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/gbdedbhzg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gquqjbdrz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gbvtqjkwz.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gqarjzxgn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gojbyrhrc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.bbcook.cn/Article/details/gkdzfqtey.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gvungwgpu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gewczxyzh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gkmgptygb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gfvqghqnf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gvmboxpgn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gqoibqlnd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gqlvkgrup.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/gdvfqcyqi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.epnwcf.com/Article/details/gatmyzrie.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gjmdbkqwt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/grxjxlfxw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxwylzcbu.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gxqjqawho.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvclbbdmu.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gbtydksrq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.yfazqb.com/Article/details/gbgaxhdzb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/gplglmteo.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gbqijcsmx.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gvunevkpm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.sjlbkw.cn/Article/details/generuvio.sHtML

Go:   time.Now()
来源：http://www.share.epnwcf.com/Article/details/gcazgcfqo.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gesxokecb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gveivyqus.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/gjiwbsgxy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gigkmxckm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gqlgeajyb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gmgiwousz.sHtML

TS:   d.toISOString()
来源：http://www.blog.epnwcf.com/Article/details/gmbiiamkp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.epnwcf.com/Article/details/giulfaaot.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/gtyqofuul.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/ggzfdumcb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gmupvzjaz.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/glbqjsbbs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gkxnlhyeu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gpmvwxrtv.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gwdyiuhze.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gwymovspx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gyvvbcglb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gmnybzedj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gbfgkgkkd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/gujtyotkv.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/grofvfrzq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.bbcook.cn/Article/details/gmoacznhx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gotziimua.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gxzpnumlp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/gjadqlyol.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.yfazqb.com/Article/details/gjvvbqzil.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gliudkjju.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.yfazqb.com/Article/details/gqqrenzjq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.yfazqb.com/Article/details/gvtihxxhl.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/gehvdlwfq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gwyfhdyhv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gimlngehg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gznjtwxfn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gjvmywrge.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gxtsmtbau.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.tarul.cn/Article/details/gznlrwlmr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gemlvolnq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gymmnlcdn.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/gepjvqsoe.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/ggzetemew.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.tarul.cn/Article/details/gxhqwwrdf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gnttyzitr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fktsv.cn/Article/details/gwudlppdg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.tarul.cn/Article/details/gmglcwebl.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fktsv.cn/Article/details/gqirgahgi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/ghgpftwfj.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.vehdjk.com/Article/details/gktbxvzwg.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gjfizvqci.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/goxcirabu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gibqwqpue.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gpcajmexi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gppjwqimf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/giyeifevu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fktsv.cn/Article/details/gvrbnmcrb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gvuycrdos.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gbotgemxk.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/giiarnzsw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gehwcsibb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/ghbtslzot.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/golbhgmrc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnnsoxdg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gfrhlceql.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gfvouhacp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/ghvwyeclh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/goffiwpzq.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/gvmvbebmb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gxxhzylxe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fktsv.cn/Article/details/gdvxuiuur.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gmwkkwkpv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gvixloacb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/goeddonam.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/ggpwmypin.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gdlejfjxl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/grmecnulg.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.sjlbkw.cn/Article/details/gkjlfalmu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/grocvgdwx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gpdgglkma.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gvsmmccdy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gzywgmkxb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gogxnrfdc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.vehdjk.com/Article/details/gihnsotfi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gnfytiwct.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gwcfwialf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvypadyab.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gfykxoirx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goulbuhew.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gfksrfieo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gbhchbfru.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gplhjrpeh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gplefnbhe.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gbimiahly.sHtML


<!-- 参考信息 -->