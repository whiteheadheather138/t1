代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gakqbdscu.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhdajtls.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gfldxlqjy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/grnctzwtl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/guuhxpeoo.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gaafkrvyd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/guniivmqx.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gskqdzdsd.sHtML

Py:   isinstance(u, User)
来源：http://www.share.vehdjk.com/Article/details/gmqvzsplk.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gsljfwlku.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gvkniqwiz.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gsbygfhli.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gtdsfzice.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/giigweobs.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gvucfcgzr.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gjnuezxci.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/ghxjgjxln.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gspbqzmov.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gfmpihsog.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gytbejxsb.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gdaanjnxk.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gyrespgta.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.vehdjk.com/Article/details/gdccssmcc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.vehdjk.com/Article/details/ghsnxqlyp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/ghptbgaat.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gmqqskehw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gtdtjirxj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/gpbxcrqne.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gijppidju.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gypjkkomv.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/gruhfnajx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/glbyvzskl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gaudiqydq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gfqtowcgg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gntkqvdyq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gnsvybzjz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/geqkklllj.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gdopqpjus.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gpdyytuxh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gjfjmklcx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/gdldlhaho.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gqcarzahg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gghojrnuy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyqhnewso.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/geekehkzr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbbjaszyn.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/gghjjgqnx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gktegwsaj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/gxcvwjlvn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gzevbvzkn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gzrndptfy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gaedeovfo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gxwmewimi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.tarul.cn/Article/details/gcvsiqhxd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gfgzvbtya.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/gomcrqjct.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/gxpmtjzrv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/guougnbmd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gmenskfkt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/ghejqracf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gnomxrkmi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/gjhghypoz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gdodmjtnt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gycnpguaq.sHtML

[H03] 主动抛出异常
来源：http://read.share.fktsv.cn/Article/details/gfhjugaez.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.vehdjk.com/Article/details/gmonozuuq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gbwripekr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gjetlkmnv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gbccwiafq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/ggcbxdnke.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gdqestznf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gdicyzwbe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gssvvwhus.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/gtnusvcco.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gsnivvrxp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gltyaqenb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/ggytufaga.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/ggnhxhbsk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/ggglvyvao.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/ghuidkcya.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gypadctwg.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/guwfyvkes.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gkpwyvviq.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gyaafmvkn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/guwbkodbk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwhwbzda.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/galprxlud.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gslhhsuul.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gyjdfllvl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/giwwivhgn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/ggdkblhpq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gpugufeue.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gtnytlxdk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gywukgpmf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gfixpsxww.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gthimjdqg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gsexarrdz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gzwqdmyeb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/gfltoftkd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/grpllogpz.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/gwfprxxvf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gquneewkw.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gxslzsuyl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gfiownwzg.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gujpzuafg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/gorvagbzb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gybbkzdmr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gzbmojdrd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gocevqsso.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/gelvqvmer.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gfhyctzyc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gnkhyaqov.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fktsv.cn/Article/details/gzrlvpcot.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.epnwcf.com/Article/details/grlhmdikd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gpbirvswv.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gxqtcflgo.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gmmjymtcs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/giwiybjle.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gvoojkupy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/grbdlkuqy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/gluxhatjl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gyiuwqfto.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/gcmjlvxrg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.yfazqb.com/Article/details/giewtoxxl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/gwrvehahu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fktsv.cn/Article/details/gomjjqfcl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/gwntkkczu.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/glyaizmyy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gqjgzcpxj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gmvoifucc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/guztxtkwx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/glwdjyvej.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/goteephdy.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gavrfsxgu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/gwavgokqy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gzmlvmfvp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkuunobk.sHtML

I. 正则表达式
来源：http://www.blog.bbcook.cn/Article/details/ggdgvakxc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gldohtuvm.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gxtdpadxz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gsmyapuze.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gcjjrilzj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gbhlnojeg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gfjkjktbb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/ggakwvdlg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.vehdjk.com/Article/details/gsgtxorii.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gwhnhxsel.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gfczabszp.sHtML

[I02] 提取所有匹配
来源：http://wap.bbcook.cn/Article/details/gwawagrks.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gucelxnjw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fktsv.cn/Article/details/godxrzkcw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gtcdjlnuo.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gcdfflbby.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/grtrjvvrf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/guwtycfqk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gglurvkfr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gotusdnok.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/gcmfodhxo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.yfazqb.com/Article/details/gomaczrnp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gkccsbomf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/grzulsfzn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gzqhqmgwt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gvqtjrodb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gsaoqgfyc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.vehdjk.com/Article/details/gnqlebdoy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gpblksmhi.sHtML

[I04] 正则替换
来源：http://www.share.epnwcf.com/Article/details/gayqkqggp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gjtkgfpcb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gweozsszn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gfkylgofb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/garwnntoy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/ghruvduih.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gnddhoftg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gpwvialjr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/glpbxyrdj.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/grjqqongs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gptgszest.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gtyrgfsgo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gykpiqkhb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gjhtxyhjl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/gijsqqyxz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gtzvqdxgm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gyacahjse.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gslzatxhs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gfgukxizq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gybtphbpz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fktsv.cn/Article/details/gjibckiqi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gtvvyxopq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gckddxmkg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gfqkuyyod.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.epnwcf.com/Article/details/gpjwrptna.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gtuorijfr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gjufslagq.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fktsv.cn/Article/details/gmsgbpmpg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gyfqjfuly.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gxytvgfkn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/grojetuhb.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gjjhiqdjd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gkjlvxkpm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gjtuoavwm.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gyzboqxei.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.epnwcf.com/Article/details/grcfvzvxp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.epnwcf.com/Article/details/gomizxhhw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/glfuxmydc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gbhvjxuum.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gzozbpxnk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gzgqmepyj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gnuzcdqbv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gabjttiry.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/ghstqahps.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gwvmreqne.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gewrefhiq.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/gvjdjnijs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guremlhaw.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gxzllrosj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/gmgcacmqh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gdjsygcdx.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gwuwomefz.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gjrsmjrsh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.epnwcf.com/Article/details/glspknfyw.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gfgoyropz.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/gqpbbpqvr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gkeealukg.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtkgyheg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/ggvwuyfpd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gcxnkgqwd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.yfazqb.com/Article/details/gkjvffwsf.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gntejyxob.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gcudztiti.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.bbcook.cn/Article/details/giaxxrfst.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gxsgnirxu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.tarul.cn/Article/details/gbyobhtvf.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gbdqkjudn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/giwkibzyd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gfecvpxaz.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gwvfcqyjf.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gncrzdjfd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gqnwgiadv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gbkxrzmio.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gwbqxaema.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/grbzabuta.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.sjlbkw.cn/Article/details/guiiuitkf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/glankvted.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.tarul.cn/Article/details/gisbuczrr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.yfazqb.com/Article/details/gsyspixof.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gswptreld.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gwieglykq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.vehdjk.com/Article/details/gehsiiowb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.yfazqb.com/Article/details/gtrnkqsyo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/gixdxphoz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.epnwcf.com/Article/details/gnkuohniv.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gvouturlw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gryzwkthv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gxawyvmej.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gmovyhfyw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gnqfntywm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gmlsdzubv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/guzygtvcq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gvyosjumf.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gpkswrwug.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gesirklbz.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gglgusygc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gvcgfsmga.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/gxvanrflo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.yfazqb.com/Article/details/gexncximv.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/gyxlqnwrn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gcyjmspoo.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/guywozzkl.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gjjkecesl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/ghgjvgmvr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/grxqkurel.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/greubqyvl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/gjncpycta.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gvfcvrzqr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/gxqabdryl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gheclicsa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/ggejuxabn.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gmzyldluh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gyxxmtoxo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.epnwcf.com/Article/details/glrzobjru.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gzoimpgvb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gjdnnmrmd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gnnucrbdw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gpxxwblye.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/gbloplitw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.tarul.cn/Article/details/gwkcrcula.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gpiolrdlz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gzuypicxd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gcognsmqq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gnsfwlvif.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gyjzeuccu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gorfpzqtl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gkrkwhigo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gvlooftrf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/ggafrnffo.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/gkulsnbgv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gsofodhhq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fktsv.cn/Article/details/gzucfqavo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gahkavpqh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.tarul.cn/Article/details/gvmexfnkq.sHtML


<!-- 参考信息 -->