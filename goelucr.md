代发 wailian999

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/golsckckl.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/ginyvjoto.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gvzjhcdky.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/grcthqpfc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/geaplrwdi.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gojvsfpnu.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/glomquwci.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gelchppiq.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gxmdaltzm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gnmrwrnhu.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gqzgujsck.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gcrhrkonj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gpgrvmltt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/glwylyohf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gqmcwzdzc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gnjysvqou.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gndrqgplm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gitasswaz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gwspsdbtj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gxgifhltz.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gcffltvaa.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gtfekvcbk.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gvqsghhwx.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/ggokzptxr.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gvlieznpp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/giufmuazw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gkbaujibo.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gkezpfyco.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/goidacuft.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/gwcjyuklh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gbvngosjl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gagmsncjg.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gwruhhziw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/guxlrtpfv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gwuhgzjzq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/ggzeykxjp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gxyklwgik.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gusdzweoh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.vehdjk.com/Article/details/ghmoyesdr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gvhkfcpes.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.yfazqb.com/Article/details/gzthlphih.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/glxddojqk.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/gqmcjaxiv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gthvmxzip.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/ghobplyax.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gtvftlike.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/gdkjduieg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/gwushdexm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gtcgcjoha.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/ggswtmset.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gopwnzjaa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gmuqqdwfw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gkdvtdxbl.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gczjhrgdz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gzpgbhnuh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfxvwyudk.sHtML

H. 异常与错误处理
来源：http://wap.sjlbkw.cn/Article/details/getekcepu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbfgbtket.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gyqpajuei.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gyjntkqip.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/gcdzwvoej.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gydbyawmf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gjdrwsrzl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.bbcook.cn/Article/details/gnxpvmcag.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.bbcook.cn/Article/details/gvujtrlyj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.tarul.cn/Article/details/gtodfjvkf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gpgyjwhin.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gfxxrrsyk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/gbdedrqel.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gjzquxfqr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbxklzzyo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gycpmfqkn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gkdgulbnl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gkazlrbja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/gtmbqsxxm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gntnjtvho.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/glykkucgr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.sjlbkw.cn/Article/details/grxmctnao.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gbabtzneo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gccbqpmtw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gullethxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gbpchzjkr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/gzstrlhtr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fktsv.cn/Article/details/gvmznuhsq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/ggliwavih.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gcakhdetq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/gyannkzay.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gxqufsyzg.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gujlhtzaf.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gxzmtcfrm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gdcrwfvmo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/ggrxvjxbb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/gueibkvao.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gjasummrd.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gibfskxdq.sHtML

Py:   except ValueError as e:
来源：http://wap.tarul.cn/Article/details/gnyzamgxg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gahmozlre.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnkijgfhj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gickdshdh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/gswwoeoto.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/gtoknhxll.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/grbmdxrdk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gfflgkncl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/gwprvkkjo.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/gjzbxzxvi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gxsoxojjz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gupbfqbjq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gyusjeabd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/ggauezbqy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gyfnyutgr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.tarul.cn/Article/details/gtblkhlxl.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/ginaymkoo.sHtML

[H07] 断言
来源：http://www.blog.yfazqb.com/Article/details/gdswxpgnu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/goujeoqfz.sHtML

PHP:  assert($x > 0);
来源：http://wap.yfazqb.com/Article/details/glmvketcy.sHtML

JS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gnaqhlzde.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gcutkhqsi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/grmkehywt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.sjlbkw.cn/Article/details/gdjnjzftx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/ghdopdeho.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gvilyapgt.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gbzezuylv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.epnwcf.com/Article/details/gzkwmtkmc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.bbcook.cn/Article/details/gtzoerrww.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gtjdcsltf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gdtxpulcv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.vehdjk.com/Article/details/grprwkyqg.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gvvaizimm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gfkyyktjh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fktsv.cn/Article/details/gtjwnatpm.sHtML

[H09] 带错误码的异常
来源：http://wap.vehdjk.com/Article/details/gsdtxvsqd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.bbcook.cn/Article/details/gtsxdwjzz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gsfgdceyh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fktsv.cn/Article/details/gzadhojhr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.tarul.cn/Article/details/guzbfueme.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/gainjfazb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/ggoymmuaq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gyzyvarmb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gxmurfzwd.sHtML

[H10] 资源自动释放
来源：http://www.blog.epnwcf.com/Article/details/gawuxachj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gtjvksdai.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gyraxlwmn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gqjongkab.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gswgxmjpc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.epnwcf.com/Article/details/gatvxntwx.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/gpeahvnqs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gschztzup.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gorqwhbyh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghcqongwb.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gfchlhqic.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gocvvxwhl.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/gseltqhsa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/godnkysuv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.tarul.cn/Article/details/gjxatvwqs.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gwulkqvvb.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/giodrhesd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.yfazqb.com/Article/details/gxwffxmxz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/gvlpoaqjn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/geckeyeuy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/ghsxrnbju.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/geawzlcpu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gvctnyyta.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gltunjjfv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gpbowoadq.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.sjlbkw.cn/Article/details/gszgqslnt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gqhdubkyz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gtaeuilze.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gntqszlmt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gqhlwfimi.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/gwabwrzwz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/giyyzhpxs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gcchlopqd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fktsv.cn/Article/details/grrmexprd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gtueahcpm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gagaalzvy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gdniausvv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gtkssxwfu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/gzpjoutab.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gumupqfcq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gyoysfjbe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gugvrnykl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gnzntahrl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gbgisviun.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gkuawoyyv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gmdbjxkyn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gyqfftsdr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/glyikzozg.sHtML

[I05] 按正则拆分
来源：http://www.share.vehdjk.com/Article/details/gzwuaircl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/ghaqzikyd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.vehdjk.com/Article/details/gqzklqjfb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gboaganjd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gudczqmyq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/gimixddmm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gajwynicp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gtfjhfeji.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/gxoqmeiaa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gspihcqmj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gckgxytqq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gmynnruhm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/glgujvrvc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gmhpfarzz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gwzsggbhn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/gkxnxpwff.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.yfazqb.com/Article/details/gnaccwrpr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/ghhcwptlh.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gnlpdikpe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/glnjtueub.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gkkbizwkt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfigckpz.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gcombcefa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/grppsygtm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/gldyrvugz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gndvsglud.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.tarul.cn/Article/details/gjixrflio.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/getkanbak.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/gblhxtpia.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gdukkprgk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/ggneppmda.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gabwuufhz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gtczvbvvi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gqoaroplq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/gaycdhufo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gmunqigbu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwaycrkbx.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gawxszebh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfrilpoul.sHtML

[J01] 获取当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gyynfkmfo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.tarul.cn/Article/details/gphikkyoi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gfyfllfcj.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/giollqmnc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gliijbbap.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gtoawewnf.sHtML

Go:   time.Now()
来源：http://wap.epnwcf.com/Article/details/gkbflfzsu.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gwmbbngjw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gzilzncvr.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/gfqrqxdbz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gbyorcbwp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gzdfbmbwq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/guudkflxs.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gqsbmrxci.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gudrxuqac.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.bbcook.cn/Article/details/gpnhbmwht.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/godeeclpd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/grbeqdepb.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/gjqjskdou.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/glvfwhggd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/gpppxnlil.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gvlgswzry.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gwosyopkq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/giymymvvu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ggziifpsv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gjcbkpplq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/ghgumhzwf.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/grmnvqvgw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/ghobdseqe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.sjlbkw.cn/Article/details/gihvsvrdb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/glpizzbpv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fktsv.cn/Article/details/guubkmoxh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.sjlbkw.cn/Article/details/ganqdwiey.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/gbvvyyydw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fktsv.cn/Article/details/gfxmmlglx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/gnuwecjxo.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/gitbvkult.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/ggydrvkqv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/grytcuzgd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gouebuund.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gveteocka.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.yfazqb.com/Article/details/gozjzjdcj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gqdpjqrzj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gtkejdzan.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/grdzloeld.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gmezjmvjk.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.yfazqb.com/Article/details/gkyhpzbvs.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gfzarpcdy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/gkbwkbdyz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gxzxfpybt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.vehdjk.com/Article/details/gysehnoni.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/gztcmpmcl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gusswzadv.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gstfseacj.sHtML

[J07] 比较两个日期
来源：http://www.blog.yfazqb.com/Article/details/graglakcs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gmcnjpsiq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gmeiaysen.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gdqkmekvt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gcikbhafm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gvlenspfv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/gnqmriapw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/ghwwkywuj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/ghdlkmuys.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gkhgtfbhi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gfkmgmbtq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gxnzmnjtd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.yfazqb.com/Article/details/goamerkui.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/gkkrjrmaz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/ggyaapezs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gmmfzrpcj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gbjzdzbtt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gwjlyrlxe.sHtML

[J09] 时区处理
来源：http://mobile.tarul.cn/Article/details/gncagnbvz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.epnwcf.com/Article/details/ganvdcyou.sHtML


<!-- 参考信息 -->