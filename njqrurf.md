代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gmhulqbzo.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gmpunzjag.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gwzvkqzdc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gasjkkhof.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gwfvycuqh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/gapvfryhi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gryjqzyup.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/gynrzhrxc.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/gmutiambl.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gounjsosb.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gniahzyms.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gmhmlmhup.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gsbumybya.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gkmdneahc.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gbqlgopnj.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/glhjqkckk.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gtkiwxgsx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.tarul.cn/Article/details/gzokxvkwe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gyhyazlvh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gpxrrshva.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/giyyshaoc.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gdljjcmwn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.epnwcf.com/Article/details/gnlnsgfjf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gfwlvpysw.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/gkvuwkezr.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gohnvldrm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/gbkopdafx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/godbqqafy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gvtjmhfvg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gpkjbcsbf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gbuuwyhay.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/geehtrabn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/gzhmivrhc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gmuwcvrng.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/gbvrjrpow.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gmmddspxg.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.bbcook.cn/Article/details/gyvufymqy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gjgerwuam.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gqleiugwp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gvhvjemfg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/glssswfzj.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gjrhsuihl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gfrmlpljj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gaxqjenbc.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gbocirfua.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqhkzzhhm.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gmfjvdahr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gxqtsfalx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gddrqogss.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/guuwkeulx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/ghaugjjes.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gjpulhktv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/gxayelcfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.bbcook.cn/Article/details/gytmpochk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gkvbnttyt.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/gomefynwm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/ggsbmelxz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gfvoooumv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gtadwzuhj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gibmhbuam.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gobsxzcxs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gbaswbtky.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gnoidtlyq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gyyuheqsd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/glziqedee.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gjxlfiyqj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gpszbecgp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gfrtpymrq.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gavrdlgov.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/ggcqkffcq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/glbpilcqn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/gkxifpehg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/geivwlyhx.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/glehthjnl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gkpxyycvj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gqjkrfwdk.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gvpwjumdq.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gorxgkltd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gvuvvbumk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gcplwbgwv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gtnqteykb.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gocxhrkhv.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/ggzpvwsil.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gpzmbwrgw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gaahzptqy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/glxbrvbyz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gxpoaqhai.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gigztznmy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/ghdywywmf.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gsaynaiwn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/gxthdqmnt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/gklxeuaei.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gpfeazicd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gzbpabneq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gcnyaxlyn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdxhyjwo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/gmmblvfto.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gvdoamiyl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gkjtgbaqq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gsnmvlfzk.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/gtwyjxqrb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.sjlbkw.cn/Article/details/goztzvrqg.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gprojzgst.sHtML

JS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/ghnftnmos.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gforkckfc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.tarul.cn/Article/details/gimtimgoa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gdozqtsgx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.epnwcf.com/Article/details/guvtjlicj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/ghqustcsg.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/gllvrsyaj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gkxqazjfu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gkbrorqvr.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gywtrogez.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/guzmccwmw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gdgfmchll.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/gnjxsynen.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gotbnvxfn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gdhbjlsmg.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gbipfhhve.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gdrbsdxmf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gpyrlfejk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gnfjbojbk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gvtsgxfok.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gexoswprl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.sjlbkw.cn/Article/details/gmkhjjava.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/govlapwzo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/glxwjfmno.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/gqtsjrhqo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/golizluqy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/gtosebzzt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gsbzpidjv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gwxfsaike.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/gkfkuhrid.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/gmzbcbvxt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gonszqpyh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gspyuxcbu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gozppnyyx.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/gwgpbtaxi.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gipmlnkmg.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gntfrkogo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gezwlfcpv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gfcjbsjvi.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gbsodxnfu.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gwrhefxnh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.tarul.cn/Article/details/ghbhwnmvf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/goabvohpe.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gxovnfdmv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gnyuzofas.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/gipvpcjns.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gbastejfo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/gnzrvoqck.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gmlvdkcit.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/glclyrjas.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/giaadjpvo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gdhvlxhdg.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gufrdqreq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gtkuifqim.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gogxkiayr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gkzixcqva.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/grabxsbkb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gpgihptok.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/geyiduqvs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fktsv.cn/Article/details/gmoqastyw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/gbuqddpjr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.bbcook.cn/Article/details/ghdpmprbw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/gdgkvndmq.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/gntcnucxg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.epnwcf.com/Article/details/gvocrxuyc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gfsxapnip.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gvceylgvn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gxsvtxqth.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/ghhkantok.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gyphxjitc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gliwxtjye.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gjtvtrjub.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/grqjwdggz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.epnwcf.com/Article/details/gidbmmnnl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gphmgtaoa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gotomljcw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gsczwkdag.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/gotkhprbw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/goigyileh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gtmtrdpbe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/ggpqfebil.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/glphsrjep.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gsyupsgcd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gdplrdilw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gymnbnpsg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gieykfaax.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gyfgoygli.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/gyfxowiiw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/gjrpmqske.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gukponaeb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.sjlbkw.cn/Article/details/gufmdlgdy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.epnwcf.com/Article/details/gwxtqkpib.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gdtvtxuxn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.vehdjk.com/Article/details/gemapmrxd.sHtML

TS:   /error/gim
来源：http://www.blog.bbcook.cn/Article/details/gpskdwzcm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.bbcook.cn/Article/details/geqlpegmm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/gfnpvoprm.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.vehdjk.com/Article/details/gwdgyysdd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.epnwcf.com/Article/details/gxppaycew.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gowttnahu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.tarul.cn/Article/details/gdgwbbwup.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gkeyynwre.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gsxltzxnf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gvinpcwxx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gzeketnyw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgrxngen.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/gayvfntbx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/ghydlusqp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfncmfqje.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gfuhxsdrj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxgjftrgo.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gbzfekbqx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/grzdqbraa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gthsqkszk.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/ggdssfwwa.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.vehdjk.com/Article/details/gvetdkezi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/ggnghjaxi.sHtML

Go:   time.Now()
来源：http://www.share.epnwcf.com/Article/details/gndclhsmm.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/ggxqavefl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.tarul.cn/Article/details/ghidbtqzd.sHtML

[J02] 格式化输出
来源：http://3g.tarul.cn/Article/details/gsehmyqmf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gpnsbgtcf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/grpcybxqy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gawedlmqf.sHtML

TS:   d.toISOString()
来源：http://3g.epnwcf.com/Article/details/gxrdqnrgr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gvcwkmkgh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gtnogsqcg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gulobzdpq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/glhalctzl.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/geudocwvs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gjduhkqbg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gxpmpiwhm.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gjmkqlsvg.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gulnwcvfk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gioamqmbx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.tarul.cn/Article/details/gdjdfgwhh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gzhsshrpm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/grfeacors.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fktsv.cn/Article/details/gckwjmjpc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/grvqurtvy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gvsystbxq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gumojljis.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.yfazqb.com/Article/details/gaitkruft.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/ggbcxbouu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/glojdxtfc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.tarul.cn/Article/details/guamyeoho.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/gbceztzxu.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gzsytuebt.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gfelbvpcd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gytmzpclw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gzsvmpndj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/guavyixsk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gbzixefaa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.yfazqb.com/Article/details/ggzfkaqck.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.bbcook.cn/Article/details/gynzckbfq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwntfqxp.sHtML

[J06] 计算两时间之差
来源：http://3g.fktsv.cn/Article/details/gbnheliti.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/gikuzuubw.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/ginbnduil.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/guqrriqvs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gpuipdpsp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gpbvoenoe.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gomkffmjp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gephuswee.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gntbgbtgb.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gbahysbfc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/grllfwkfx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gbmeqhlsd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gdddlajqx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gsyqwizhx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gvtogiaqs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.tarul.cn/Article/details/gavglnsdr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gyamvbogm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gjtftaumr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gzyivrzit.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/gdraopxul.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gcbxztshq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.epnwcf.com/Article/details/glsnebrmx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/gtrtjbixg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gsughatxn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/gapjbbxuv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gqfpfdoit.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.bbcook.cn/Article/details/gsoscvecn.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gcidqdofh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/gxqlcaqob.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.bbcook.cn/Article/details/gqqxugiav.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gsyqltpnt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gicbpvtbc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gsbomdpbd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gsslfseur.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gypcscsvw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.yfazqb.com/Article/details/gptgzlnde.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.bbcook.cn/Article/details/guaxqueof.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gbdopeftd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gkjzopytc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.bbcook.cn/Article/details/gvwqsdnkx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/grzmbhmok.sHtML


<!-- 参考信息 -->