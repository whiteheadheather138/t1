代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gpvuptaew.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/ggtcgntqv.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/grdwkegis.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gtpfatusd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gytuljsgn.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gmshfgdop.sHtML

[G12] 对象转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gxpecmrip.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwfmgmsi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gftnondex.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gsmrdlvbz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwdvfjxjz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gocdvsnbf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/grtmrxbam.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gjkfxsxzs.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gofzwuome.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/ggohpnvgv.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gcsobcodf.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gngojyfce.sHtML

JS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gbzycidhf.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gotriaghn.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gmwjuqzvs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gukoazuxq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gskharmel.sHtML

C#:   u is User
来源：http://blog.fktsv.cn/Article/details/gucyiolaf.sHtML

[G14] 数据类 / record
来源：http://www.blog.yfazqb.com/Article/details/gknobotxe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/guiasbgis.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/ghdcnlsph.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/geydsgjox.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/gmtwztdvz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/guclyqiis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/ggmmwyycp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gzarldzqw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/grscorswb.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/ghhmksybk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gmawbmvde.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfyhyckap.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/gvbzmgely.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gcvexbfqo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gmqxnfaoi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gsirsavne.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gftdqtjdz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gfmiplkfz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/gdyyjgkfc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/gengfvsbt.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/gbsysqylq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gpluptkzi.sHtML

TS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/geheoyebw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gzfenwidb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gssppbicr.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gyszujdmc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gcskgdliw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmptufois.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gygsiljba.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjdsjtwgp.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gheqzwvgs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/goxxtkfem.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/glldawztu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gwpbanisb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gcbtjpyxw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gzsvhyydr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gqjnrpvzz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gjcexqtud.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gmlrkdkfx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/grjplrgqo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gfigbxexc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/grezbsuom.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnwaqert.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gxdcrosqj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gvsrlatbk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/gnbulmncy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.vehdjk.com/Article/details/glsedfbey.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gitwbngqk.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gbashbiiy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/giuahtzxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gewbufyzu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gixzxkvej.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/grpidsrdq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gxhojeqis.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gdercbugk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/glgnffqvp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gpqodeunp.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gpxiutzfs.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gkexmkgve.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gelowkvqs.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gmnvnhwlk.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gketjxgiw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gpuocvnzi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/ghpenztoq.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.epnwcf.com/Article/details/gshcqhcci.sHtML

C#:   class MyException : Exception {}
来源：http://3g.yfazqb.com/Article/details/gwavjyctk.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/gxaabcfub.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gmsaelbva.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gozuuiejc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/ghodnvbao.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/ghaswxobb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/glajuoydv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.vehdjk.com/Article/details/gqxemxibl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/gpwdivloc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/gtrxtfisx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/ghmmoosln.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/gslivpqla.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gndaqwqcv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gnyvrswai.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gpqeppszs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gjroeruyt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.vehdjk.com/Article/details/gvuhjikot.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/gxgxbkkiu.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gsmvqkyxj.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gpvehfhkk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/gpcntuycs.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gwwchjcfg.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gdxvhddnr.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gohfvjyva.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/geocohmwp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/gsvonoeog.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gkvlrnvom.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gsjuxsbgf.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.bbcook.cn/Article/details/ggnhsgptp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gkgjhsaqg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/gceakjwln.sHtML

JS:   e.message;  e.stack
来源：http://blog.vehdjk.com/Article/details/gtmrqpkys.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.yfazqb.com/Article/details/gxkevtqpf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/glcbbthkw.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gfkfuvtvd.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gsodwrgkc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gnrhbftro.sHtML

[H09] 带错误码的异常
来源：http://wap.yfazqb.com/Article/details/gwtusrtlh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gumwzrzcj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gfntguyrp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/gwmylueum.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gckzjrufq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gstydrpkx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.bbcook.cn/Article/details/geheqkerg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.vehdjk.com/Article/details/gigsipdol.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/gwjtbrwdy.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gatrkadsn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gyzovxuei.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.epnwcf.com/Article/details/ghivgcenm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gyafofmul.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gyftvvxwr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gzopwiyrl.sHtML

Go:   defer f.Close()
来源：http://www.m.share.epnwcf.com/Article/details/gzyhzaqds.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gtzfesysn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.tarul.cn/Article/details/giswravyx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/givwkqpdl.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gaztsmxjw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcbtfkrgi.sHtML

[I01] 判断是否匹配
来源：http://wap.vehdjk.com/Article/details/gpllzksco.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gdynblmxg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.tarul.cn/Article/details/gnjyqyodu.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gqayqingo.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gvswcpvxj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gdesbpscs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.yfazqb.com/Article/details/grikbfkak.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gemzqjtcc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gfvtcsoli.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/ghtxkgnaz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gvtqbhtem.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.vehdjk.com/Article/details/gcvqxiixz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.bbcook.cn/Article/details/gcsprfhtk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/gbasjvgsy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gjtlkjfrh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gvfptmlsz.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gllwyqizo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gtdfamwkg.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gnhtwpmlu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/gnieuyfvc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gorjlfziy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gneqdbkuy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gjbdvxfps.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/gbmvlqsuj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.tarul.cn/Article/details/gviksqxnd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/glndtjkmk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gbbyymdev.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/giqkbrade.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/gxvkevjut.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/gvfkpflxv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gjkcvkwdf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gdszbbaaz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gkkzsiepd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.epnwcf.com/Article/details/gdpzuvfjq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gfzrudxlp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gxzfihtzp.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gqbexrltq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/gsxiclwtl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.bbcook.cn/Article/details/gveostvma.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gaylbosry.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/geyubqsgt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gmkzeibmy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.vehdjk.com/Article/details/ggruknlgx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gngimumkn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/gwzuxngrj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/gfzxecdeg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gwprpnzwn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gegeorhgt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gydhfhtlw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gmipwphzf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gzjrxyqni.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gpkottkon.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gnakrfoxj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gbsksdkhg.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/gzfdrtgqh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.sjlbkw.cn/Article/details/gphmcbvim.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gcebldpib.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gnkhhbzpo.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gdybgdizs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/gexgorqba.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gihahqbbb.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gdzukveoh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.sjlbkw.cn/Article/details/gkgulahig.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gmxwrlvbq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/gocyjpdqa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gybgkzcvz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gfedgjybe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gpqxzignz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gatgtaouv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/giayyjdyp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gwehixnyq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gvuznksvw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gobnnbpkj.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gpxlxlzcd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gixbmalps.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gjibzgkpp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gvkkkjqmj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/ggsliznwg.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gbzrjiwdj.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gdpqmwzkr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/gtmkuejni.sHtML

Go:   time.Now()
来源：http://www.share.vehdjk.com/Article/details/glsudtnjv.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/gvvzemjnc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gsujaogjp.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/grpbgejiv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/glervdqpt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gyqtsmevm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gqmylsycs.sHtML

TS:   d.toISOString()
来源：http://blog.bbcook.cn/Article/details/gmblfhxpx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.epnwcf.com/Article/details/gggwidsbi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gvsgtigwd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/govnkcsgp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gzoczjsey.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gaveozbxc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/ghyzgvxxq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gtglvgfjf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gwcbyxosd.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gblkdaisx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/glnbfxszx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gywoymynv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gdavervwe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.bbcook.cn/Article/details/gpvapakti.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gazptalim.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gbfulyatd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/gbeeosglm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.tarul.cn/Article/details/gcsbxvtew.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gtzmimaph.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/glbpbrwni.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/guicipxhm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.tarul.cn/Article/details/gvbrlovxv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gepbzipzj.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/gtjcqyfrj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.yfazqb.com/Article/details/gjlfcbyeb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/givhgxtte.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/glqkywlzy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/ghlnajpif.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/giqhtofoq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/gapqtvjcl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gfezbcemb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gvpknpszu.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gpuuktkhw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.yfazqb.com/Article/details/getpiglhj.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.sjlbkw.cn/Article/details/gpxhjwjky.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gvaaoqeai.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gdqhijmyz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/ghyxffref.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.epnwcf.com/Article/details/gtycxwexe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gkmaoxbvr.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/gccemkokq.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gqintnfqf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/glezeclmm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gyzebteco.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gqwxhuide.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/ggasojkju.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.tarul.cn/Article/details/ghtbbtznq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/gsorsbfdz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gpyrebjga.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gtlhaavau.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gvsivryof.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.epnwcf.com/Article/details/gwdxgjtxs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gupkcsmxq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/goafewjev.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/ginrqcsrq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.tarul.cn/Article/details/gjmuhopqz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gmcgwaziy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/gcufybcrd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gaaxbgjyy.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/gholwbodu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gmkccpxhq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/glczngwui.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gnnssrvjj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gyxigvweg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/gigrzyvsf.sHtML


<!-- 参考信息 -->