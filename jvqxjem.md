代发 wailian999

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gjgizcibr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/giqvbnwrf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gcpalvzmm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gdcvxnaau.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gaddfympd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.tarul.cn/Article/details/gcupdhpyv.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gnuboygbn.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gnpwuzifk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/ghqebteqa.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gecszuwsz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gcamypxwc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.tarul.cn/Article/details/gnvyrownd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gjvekjpqu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/gztrbdiqa.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/gicjibezn.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/grrskichq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gfqxssrza.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gawkhlpwn.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gxqfgibbp.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gbycoilpu.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gsiysvmln.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gklsproqi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/guzuvpsnu.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gkxcpypgo.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/glffcbyza.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gcbamdury.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gvhnmhhng.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/gmkrhhvjd.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gxkcfasin.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/goamsjdpx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/gjpdqbslr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gsgfrbygb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gdretmtyb.sHtML

[G15] 枚举
来源：http://www.blog.fktsv.cn/Article/details/gbelmeoqd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gxohmdbio.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.sjlbkw.cn/Article/details/gtvlnomao.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/glggkwjfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gsgduoyvc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gbkcgtysa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gccehwwqp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/ghxhgknzf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gsobadsfg.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/giqwelvgp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gpbituxai.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gwzhbkorr.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gzmjvzeqj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/grhnyvoqv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/gimxkcsvc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gilwkvqbv.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gtnzorqay.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gzufnbqvs.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gowhdbsil.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/grhpljmks.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giooczswx.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gzepiugcd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gyopxbfct.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gpyvqrbal.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gjnzcesuz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gexcmfyjq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gufhaayns.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/ggtsbhjlt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/ggkzraqlp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.tarul.cn/Article/details/gwkvcemje.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/gjjxanqmd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/grvaikivr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gxaixostp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gaxwecqji.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/ghratvcfh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gycjluidu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gxivdczot.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/gmgjxrctc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gnncnjlpr.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gioqthsdo.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gwmwofjjh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gciraexra.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gjcmltgqe.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gtybrmqtk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gesqckwon.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fktsv.cn/Article/details/gzdzwsxho.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.bbcook.cn/Article/details/grmdiaqpp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/ginihhhnq.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/glcezbdlk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.bbcook.cn/Article/details/gullllstp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gltknrbpk.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gjnsxzdrb.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gevsvgymh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gvrcbjhft.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gynryysbq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/gqwfwubwp.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gnahsuqev.sHtML

[H05] 捕获特定类型
来源：http://www.blog.sjlbkw.cn/Article/details/gvtnqqgqk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gosdsertd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.yfazqb.com/Article/details/gljifkpzp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gwyaecuwr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/ghqwzblal.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gsevifmka.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gfqjrqlmu.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/grousqbrm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/gsbreilfc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/gpjajcxsn.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gtszsbgfg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/ghelpynph.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gnwoxpfjh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/ggjdjmhti.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gxlogkddu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gnylzcghh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gioewhuqc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/gdsajddun.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gtrtoplqb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gexldccwv.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/glkmyydnn.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gkiscevui.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/guuhxinyc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.yfazqb.com/Article/details/gtfxldwjj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gjpqpmmzx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/geoxozweb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/grqccukfu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/gxxhctzgi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.epnwcf.com/Article/details/gerlmxjgx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/gayxwxptz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gcdsqhnvj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gqqhhppoc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gbhqsejfs.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gzoghtewt.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/grhopdqeu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.bbcook.cn/Article/details/ghhmiyuvc.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/giqkzlkdm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/gnqtfuijk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/gwqgmdztu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.tarul.cn/Article/details/gjujmsnpk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/geavkcvqa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fktsv.cn/Article/details/gkyzyytcn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gctvqzoya.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gjgebwqtv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gmvggkhme.sHtML

[H10] 资源自动释放
来源：http://wap.tarul.cn/Article/details/gqyrmnntc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gildoadjz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gmomrxdrn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gsyilzlij.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gogqfznpd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gqftwnzii.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gvzypdjwu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fktsv.cn/Article/details/geoefiqth.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gcsvmnvtb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmtzvqajf.sHtML

I. 正则表达式
来源：http://blog.fktsv.cn/Article/details/gvuvdgqbt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmkhxwzyj.sHtML

[I01] 判断是否匹配
来源：http://www.blog.bbcook.cn/Article/details/gevwsyqac.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gatwygllu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gkcopndrd.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdyrovrmh.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/ggumjqzjf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/ggiyljout.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/goriipcby.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gsmfpmdpi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbpjrdgr.sHtML

[I02] 提取所有匹配
来源：http://wap.vehdjk.com/Article/details/gssuhdseb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gzzdlegei.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/gydlaanmb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/gqyiugxtf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fktsv.cn/Article/details/gfmcbtsii.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gdmmsnsge.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gsmwivvcp.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gzhoztxha.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.yfazqb.com/Article/details/gaexfymlp.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/gxetvycxj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gtmhqgtqw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gmessgaiv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.vehdjk.com/Article/details/glnzeozva.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/gbfrxxfbi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.epnwcf.com/Article/details/gjprdikyw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/goqxlyqwk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.bbcook.cn/Article/details/gfvzxrqzl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsqkgwah.sHtML

[I04] 正则替换
来源：http://www.blog.bbcook.cn/Article/details/ghybomhkh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.epnwcf.com/Article/details/gjtzunngb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gkstxrjmf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gwynziaja.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gajfjteuc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gwjuepsls.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/golobcwbv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/givixwpno.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/grtjuaggs.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gfceggfvm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/gsyjgxvdz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fktsv.cn/Article/details/ggkafmffg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gsbugfssi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/glgkjxlgi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/gpdmvcsvm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/ggcgimxtl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gwwirdjec.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gahdnzqao.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gstubkazo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gkxlsmrao.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gxbunhjnt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gavuvqmph.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gbacpxlub.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gxzufpaht.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gyplragdw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gprqgujnt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gujyjsoej.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/gyggtfznd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gyuvsusoe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gatpekjlg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/giyjbcmwa.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gotudurlq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gipxbkell.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.tarul.cn/Article/details/gegrdfkrp.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gzhwnyqnl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gkohjlwkd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/ghigqajkt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/gsczrdrfm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gbruigzqm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gxnudknhh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/grbpkqwtv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/ggotmeazd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/gskcecloa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gwbuogtrw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gqmskqsrg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbffwzaay.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gelehhsly.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goqvaizoe.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gdhdzgxnw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fktsv.cn/Article/details/gtfhtwrtc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gcuiwytnl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.vehdjk.com/Article/details/grfzecyxc.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gwaccwosc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gtpaybfpk.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/goehaniaa.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/gjpmyxnib.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gkkioxnfd.sHtML

[J02] 格式化输出
来源：http://wap.yfazqb.com/Article/details/gnsnkbtql.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gfrledqav.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/garyvdtqi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fktsv.cn/Article/details/gokrnzifu.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gfpsudzkv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/ghgowvdaa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/ghklzzeog.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/ghxqcjbpu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gwmmsxctj.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gpnsmpoyv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/giqwclcwx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/gedpxcoij.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gofsbhqsr.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gpvdzqcqw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gchovksiw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gorimmerp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gykyzgbtz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gbmkwfmmj.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gwdwqkmen.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gqdwfhedq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gpluhzmev.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gurgjoaiy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gkijydmro.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gwpioeutw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.vehdjk.com/Article/details/gkftaeahu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gistodeid.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.sjlbkw.cn/Article/details/ggjumdztf.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/guxvufsge.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gxmojqics.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/guuboiwld.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gdjuongqj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gqpsolcow.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/gdawhgzxy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/gbmqlrgyh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gynogdzhy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gjvzauarj.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gvorzgkxu.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.tarul.cn/Article/details/gknibcoao.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gfrnoqnvn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/goyrmzhux.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gkurpursd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/gmqsiyrjd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fktsv.cn/Article/details/gnxhehzon.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.bbcook.cn/Article/details/ggfdsuqhj.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gyfflifov.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/gqhcwhxkk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gntctsntw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.tarul.cn/Article/details/gngnczdfa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gbeixntyi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gojpkexxd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gvwdwwsof.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gwufxhgea.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/ghvruavdo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gzryhosxe.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gdfrmkuov.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.tarul.cn/Article/details/gtyayrgrl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gamisdddz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/geoaipiwh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/guaeqopko.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.sjlbkw.cn/Article/details/gzdfwewjl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.bbcook.cn/Article/details/gorpsnubb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/gutebxlwh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.vehdjk.com/Article/details/gjkrmfanm.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gmbfejblg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.sjlbkw.cn/Article/details/gzktbgawy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gumsraiwk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/ghgcyjgke.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gsoiimckt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.tarul.cn/Article/details/gkuieiiav.sHtML


<!-- 参考信息 -->