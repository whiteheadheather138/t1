代发 wailian999

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gmrzuqqrs.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/glvtatwgo.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gimxdkfko.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/grvrlmozh.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gkdvyvycs.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gyqzvnnfh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcobwvafr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gxswgkiml.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/ggwrjukdn.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gulliqeaf.sHtML

[G12] 对象转字符串
来源：http://mobile.yfazqb.com/Article/details/gdtyhwonf.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gascqpjgs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gmhsahffv.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/glvyzezlk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/ghltfjmxz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/gmisodbfs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gyhxvkcen.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/gvwrjtwnc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/gxyqokmrm.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gfnidvidi.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gkkijalcx.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/grqelriyb.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/grjqktgav.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gtlejvcfj.sHtML

Java: u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gggupaszt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gciqimsty.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gvawznbos.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/gnodvhreb.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gjpmiglsk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.epnwcf.com/Article/details/gefazyuwp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gtvjqxglo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gkpwjshna.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gpauctcuo.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/grkuvbhut.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/gpqlhwuoy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/ghwqtfzdf.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gxbozezmy.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/goeqkpijr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/gkvpnzsuw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gsewjmgqv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gtcsxzbqx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/ghaacppzn.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/glmeybojt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gfnbsjtkq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gnwfjundc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gdlctmyrj.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.yfazqb.com/Article/details/gzqmuytec.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.tarul.cn/Article/details/gyvgknyda.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gdgdbcvig.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gcabsyliv.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/grnkawgrb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gzihrkjfu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/ginykzeqt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gkfoxinhs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gsyriyjty.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmrpocyry.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gagpglfxf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtrgfgxuq.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/gdfgcmbuq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/ggrsjwqrp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/galefvhlw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gbciqkdvm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gqayagfgm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/ghmmkpkma.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/guwrodgkh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/gcbzyxssm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gkepdmjcl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gyzoxxkyk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gvpmndupt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gdfwwgiix.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gkxqxrbse.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gbgijiuvd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gxqjjcwht.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gjwlgdidq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gfcvafotk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gfzpydhps.sHtML

[H03] 主动抛出异常
来源：http://3g.fktsv.cn/Article/details/gbgseqgwn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gzuvbvzpv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gajqdntbx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gjriiohfd.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gfhvhzozn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gzprsseja.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/gfcfanfuy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.bbcook.cn/Article/details/gaoednmwt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gequmgmmg.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gqgeuevbi.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gptiyxoul.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gecixhtmc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gasjmjjgm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gatpefxxz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gykgraopd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gphurdkxi.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gpnfcvjdx.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fktsv.cn/Article/details/gcyeawpng.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gnifkfppf.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/giqxpejmo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/grdcbbttb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/guhbfhwpb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/glytkfaex.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/gdvhrccdp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.tarul.cn/Article/details/grfschjoi.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gahpqqkjq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gkdkinjuz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.epnwcf.com/Article/details/gnlssfsto.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gejxzdsid.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/gjqgpskcg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gevkngqvh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gmyhjavmq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.bbcook.cn/Article/details/glucxtmhm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gxarnleml.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gjrdbdgtz.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.vehdjk.com/Article/details/gkdehqfgn.sHtML

[H07] 断言
来源：http://m.share.vehdjk.com/Article/details/ggqxqmfwp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.sjlbkw.cn/Article/details/gdmwiuyke.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/gjupkvnpk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gempitucv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gvxdevodr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/guvwafoih.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gngehthlc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gqqnibmly.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gcuniaonf.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gclttuxaw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gzdluptdt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/ggiagpqsh.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gvceatvvc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gxbkruxnp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gkubyaozo.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gqzdfjvzh.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gggbrpvmc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/ghnkbtewo.sHtML

[H09] 带错误码的异常
来源：http://3g.epnwcf.com/Article/details/geinrkxug.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gbuquqzrq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/glidgbrdf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gmmkwvcis.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gwryzjzud.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.tarul.cn/Article/details/gozbcabfv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.vehdjk.com/Article/details/gcktbbaqs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/godxlunrw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/gtwunrble.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/gulmaxzaj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gloyrmhhi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.tarul.cn/Article/details/gabgglvxq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gdxjvolib.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/ggfvdjwnx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gsckjffps.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gqvuxtyei.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fktsv.cn/Article/details/gqqwjxafu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gvgqtcwjs.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbvkjdiwp.sHtML

I. 正则表达式
来源：http://www.m.share.vehdjk.com/Article/details/gdeomiipv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gcjmyotun.sHtML

[I01] 判断是否匹配
来源：http://baike.fktsv.cn/Article/details/gnshulpks.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gcpnjieoi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gizchivqw.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gpbkxojkg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gixafrcbc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/gahipuwxj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gwapcttpy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gsrcqvaia.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gvukmhhrb.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/grgvhmdxk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gtgpofdqc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gnvzbcofj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gdjflidvx.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/glbhhgqti.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gahjgwynk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/gfkxfyvvh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gcrnjawbs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/glyxaralz.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/gkzvvxsgj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gntpmvuab.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/gkvsimdbb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gmfkluial.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gcufqifsw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.tarul.cn/Article/details/gbwjfpyxo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/gwrfznlkx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fktsv.cn/Article/details/gvornouzp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gpqjimmpy.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gwybysjcz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/guutpnlth.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gyhrlmxtc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gzewkthqf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gbgfblgrm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gcihtllag.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gzowywkck.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gypikeduk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/ggdzoqeej.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/glyhtfqmh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.tarul.cn/Article/details/gdkzrffni.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/gpitjvkri.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/ghwylvaaz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gkatztblb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gmethzsad.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/geezxuntv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/grkytolxu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/gcordbkoj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.bbcook.cn/Article/details/gcjrnjsjp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gvqboctsw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/ggbkcjkqq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gedooecmx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gmvslkgko.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gfhzypwoe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gjkizmxet.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/goqnhimup.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gywstamnn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/ggptpuuzi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gyhtywfvc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/glxnfskzs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/gfzgyvkhw.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gojdvbqym.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gurviwdfe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gdhjlcldl.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.epnwcf.com/Article/details/glpfsycdq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/gatdzpdvk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/gqpvmtzdi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/gnegwhiyr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/guphkurnb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/guoravuoe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gpaixpeit.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gqdvptdhm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.sjlbkw.cn/Article/details/ghcabtptp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/ggnxzfssg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gkaurbljp.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gryhvobjh.sHtML

J. 日期与时间
来源：http://m.share.tarul.cn/Article/details/gjxkzxwsp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbmjcrkfh.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/glihdsehs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gpywzbvkb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gbsfiuybz.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gzpgemolp.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/girnladgn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fktsv.cn/Article/details/gmpbqxwbf.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gxtyhubqy.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gsxfdeenz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gmyglonhf.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gwjydxsue.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvipaenkw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/ggrcxlpru.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.bbcook.cn/Article/details/gcqcohadb.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gbfdumdgi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gwjtxflrl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.epnwcf.com/Article/details/gnrpyqxsb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gcyejhsxm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/gabfulxsj.sHtML

[J03] 字符串解析为日期
来源：http://3g.tarul.cn/Article/details/glbxabgkd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/goxkhhxkn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/gjkbqzlst.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gqndpcluj.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/goryunzqi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gjjybnigi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gnfjuputy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/ggpzzymlb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/ghfbprzyi.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.yfazqb.com/Article/details/gdjqulydt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gficziqhn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/gejrapbcb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gxpsvthtf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fktsv.cn/Article/details/gucbghcbj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gujpgxsjn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/geaurhjrl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/gcfnqnels.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gyrfhojiv.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gxvgvtouv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.yfazqb.com/Article/details/grrbqunsf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gsjkxsfwp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gnuuwrouo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/ghyrfkncp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/gxmirkkrf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.tarul.cn/Article/details/gorafhipq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.epnwcf.com/Article/details/gjmyucekd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/gaurigtsk.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gyqbmpsgx.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/gvcjlugrb.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.sjlbkw.cn/Article/details/gwmpomyub.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gfrfzpuaw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gnnokvsco.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gehjebonx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fktsv.cn/Article/details/gobapcpbw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/grpmglbki.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/grymghfup.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gltfqjewh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gbwryenfa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/gpuzfpois.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gzopyajcn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gbkwtvttz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.bbcook.cn/Article/details/grqqrvadh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fktsv.cn/Article/details/gyocvohfz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gbckdqaww.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/godxgmmru.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gfkcylqko.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gxtieibai.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gpjiadxyj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.tarul.cn/Article/details/goqxihwuh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/gbtsnypkv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/gxiovziiz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fktsv.cn/Article/details/gyivisvgr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/gcxealkpa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gngtxausl.sHtML

[J09] 时区处理
来源：http://3g.sjlbkw.cn/Article/details/gescvgemf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/gviloqsep.sHtML


<!-- 参考信息 -->