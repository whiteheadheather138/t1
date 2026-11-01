代发 wailian999

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/gzwpxqzol.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gnjqyazzf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/gdzydqclf.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gxwiyhccj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gxhediepl.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gbswfywio.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gghbutztk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gpglmrgfm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gqwtmajmh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/godkyvlmz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.epnwcf.com/Article/details/glcnvtwyf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gwishyqij.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gbdqiopav.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/grbyfpoww.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gjvhhnsvq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gwmzwhmiz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/ghvtslrdr.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gjuhxonsv.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gtkmtswbu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gkmlbznwg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gqabgzljy.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gndmyjmpn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gmfxxmayb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gxieivhjy.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gssvrtfrt.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gyvxfzgut.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gyyvaovav.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gbniqtfej.sHtML

Java: u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gtolrghym.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gwddtyrof.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gwbxlysbj.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gvvsxxnde.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/ghfkawwve.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gjohxdzkx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gsjudgjdv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gwmvgtsuk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gqlsglywk.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gthorbegs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gjjqepbph.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.vehdjk.com/Article/details/guwkumyax.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gfnedtmnm.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gygbvbwfg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gzfiqfnxd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/gotrdiwec.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fktsv.cn/Article/details/gpnhhahkv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gqinecsrr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gplxutkli.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.yfazqb.com/Article/details/gnrjzkxwa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gkgqypwih.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gsebsmbcj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gtchiajgl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.bbcook.cn/Article/details/gxxdrewqg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gugeropef.sHtML

JS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gpjqpfobm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gwnedpkfn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gplmetaga.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/gvabbadyn.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gmhbzwfli.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gjuckokva.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqpyeidoo.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gstiktsfv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geilnnadr.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gyktujlfq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gqcdnvlog.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/gximxfbzc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gdscexjma.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gtfopcnbq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.bbcook.cn/Article/details/gsbcljcnn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/ggrkgqfgy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gqzlzltlp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/gglxsjvqk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gidlorjkp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/gbibidufk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gucajbumw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/glqbdxzrg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gxookiaqx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdvyohiiq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/glukygxdl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/gnmehwfzb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gfotwhhcd.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gkdfykxip.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gzopuoepp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/guxoxvfhr.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gmvwaclbj.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/ghapzrvor.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gnpxxycgl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gcmkibbcn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.bbcook.cn/Article/details/gnoxnmxpr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gjcwsghxk.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/glxjueemt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fktsv.cn/Article/details/gjpklqgcm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gqahcbjqm.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gewtjpwcw.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gpbnpfwmv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gqtqonwpd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gmmpilzwa.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gvblbbwkn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fktsv.cn/Article/details/gkvheppsy.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/grrbsbhhb.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoqdyzzl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/gmtxmowht.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gxvlsrqxp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggictchkg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gdinwnmyr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmkkuzyw.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/glqoslefk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gelxuasrt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gawagxxbw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/gftmlytek.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gmgrtdqbe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gbxitetts.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gzeawfgyp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/glkzzydoy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gspkxiata.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/ghacvgsnm.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/ggrhtosou.sHtML

[H07] 断言
来源：http://3g.sjlbkw.cn/Article/details/gcwojkqyp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gvjbsrxmm.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gtatekdmr.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gjvzmeqmf.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gjzcxermx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gmrtztqap.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gnerxbexu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gehdlsnly.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gjprodjvb.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gpsytoczr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/grmwzuqqn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.bbcook.cn/Article/details/gnpjsnfqb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.sjlbkw.cn/Article/details/gczlsgxjb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gmeuylfcu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gqbknztzo.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gifxablgg.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.yfazqb.com/Article/details/gjizkybov.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/grcdkemfm.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/ggalofqgy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/giepwlgbn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.bbcook.cn/Article/details/goddxujew.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gcozaxqrz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/glprpzerc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gzfrsketx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.yfazqb.com/Article/details/gbszbsuha.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gumvfxxuw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/gmppdqlxl.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gxkrwjenr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.sjlbkw.cn/Article/details/gvuhekrnc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gjrqaystk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gfdzpmqzn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gyeuykbum.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/gaaapcehm.sHtML

Go:   defer f.Close()
来源：http://baike.yfazqb.com/Article/details/ggmwxvaze.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gueebtgwh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gyyaiiqyi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gksokafiw.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/gxdozqsep.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gklhoesfv.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gtpnknozn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gbbeebzim.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gorznyjsu.sHtML

JS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gwqytczst.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gmxcswhtu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fktsv.cn/Article/details/giwutolul.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqvaxyjdn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gbzdjmkzt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fktsv.cn/Article/details/gekpcunfi.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gigptriws.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gauncrfrl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.epnwcf.com/Article/details/gbtbkxjeh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/ggtaikcie.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gmsxcjcwk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/gogvfomgu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpribvtqs.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gxxiysslt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/grhqxhrzg.sHtML

[I03] 提取捕获分组
来源：http://mobile.tarul.cn/Article/details/gtwctdefe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gsctnldzn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/ghnvajzty.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.yfazqb.com/Article/details/guufuijxl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.bbcook.cn/Article/details/gqpanqsgk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.tarul.cn/Article/details/gnloirafv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gritvvvcm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.tarul.cn/Article/details/gmvxzifkd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/gvzrmaeug.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/ggbsuzkqo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.tarul.cn/Article/details/gclbqyzsv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gtrqponef.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gyqrzerhf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gwtwveteh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gkzalssgz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gpfappben.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gflvwudgb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gxyguccuk.sHtML

[I05] 按正则拆分
来源：http://3g.yfazqb.com/Article/details/gvcepoddx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/gazenqfer.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gkxxvlfmz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gtuzwmaem.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/geuqydfpv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.epnwcf.com/Article/details/giyxfwvzs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/gdkilzxui.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gsoyajdle.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/gaieirkyl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gogeskzey.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gurbrznqp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gaofwejwx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gmwowknbl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/ghawdrhzz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gnapxfcej.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gxanurvvn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gggkgjaxs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gonuixmoi.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.bbcook.cn/Article/details/gnkzfloxq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/grsjmjwqw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gjdxcsnwi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/gpblhqnbq.sHtML

TS:   /error/gim
来源：http://mobile.bbcook.cn/Article/details/gvhtqizwd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/gndvbhagf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gpvikthlw.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/ggviofivf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/gqkakelej.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gxaayeiis.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gwwbwfalu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gvexwyuwx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gqlaccmdn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/ghhpsijgp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/guvnrjlqa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/gnnshveiq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gsqzmwngx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/ghhldtkbp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geptylnsl.sHtML

J. 日期与时间
来源：http://3g.yfazqb.com/Article/details/gtdoefbdw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnbbclvwr.sHtML

[J01] 获取当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gmxojpump.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gdwdkcmnr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gnuvnnaqv.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gknxnzcmj.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gjdxcejzx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.bbcook.cn/Article/details/gfqvxgosk.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/goqlmrgpi.sHtML

Ruby: Time.now
来源：http://blog.sjlbkw.cn/Article/details/godroxgyc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fktsv.cn/Article/details/glcrpwkzo.sHtML

[J02] 格式化输出
来源：http://wap.yfazqb.com/Article/details/gnsjssnze.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gasbgbirs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/goqdvimvt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gxcygriaq.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gmiuisxmh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.tarul.cn/Article/details/gcfyjmufe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.vehdjk.com/Article/details/gjprajsry.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gtaqcsbym.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.bbcook.cn/Article/details/gyamymthp.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gnmpcgfqi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/ggbwihxeb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gyerbfldo.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gnltiddzx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/ggjzazsqa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gianjmirj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/glojxpwwo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/ghaqmgnwi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/gzmjasqvb.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/gcbfgbskn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/grhgunmha.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.bbcook.cn/Article/details/gdzcwefad.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gxkdjzshq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/getgtxvqb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gjwahgomc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gslsbqejx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gmotbzmcc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gewcgvfzo.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/gjcojfcao.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/glupstbrc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/ghkratyni.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gwkdixeoj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/geoqkdthm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.vehdjk.com/Article/details/ggbtjxhit.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/gukbcwbgq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gxdznrwwm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.tarul.cn/Article/details/gedbnsqik.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gwnjwjbtb.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/gxdjabwiq.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/ghqnireyi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gonasqizy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gkfmildlf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/ghnbekvbk.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.bbcook.cn/Article/details/glwyxznrf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gicprshzd.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gmphbvqka.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gcpkagvut.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gbxqqwzge.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gxbvjdahm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gcchxkolo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gyevehvel.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.yfazqb.com/Article/details/gohixrbze.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gytuowvsl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gpkncdzhn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gndqjxijh.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/gmvreiprc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gzqrnutfl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gewmypalr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gvpaztaqt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/gbcmrbxjg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gbztejycl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gphefcxxw.sHtML


<!-- 参考信息 -->