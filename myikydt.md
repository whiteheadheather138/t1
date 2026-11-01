代发 wailian999

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gtlyiqjch.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gzkkgtfgm.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gmkhdoqnc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gkyhodltf.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gmmfffgmp.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gahgnocbe.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gtuxqstmi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gjjvixapt.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gbowfmlxu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/grjcgyfux.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gpezrgqqy.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gdwkdnbht.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/ggcxqlgki.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gidslzawb.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gtwsiwlqf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gsmobigwh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gemiqqwdb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gkdyzynea.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gfrysuwku.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/gazywkbiw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gwknmtvms.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gybqisvhf.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/ghcfazctf.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/ggqmbwhtk.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gpuhfabeo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gmwcqncft.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/gdepmwmwr.sHtML

C#:   u is User
来源：http://www.m.share.tarul.cn/Article/details/gpdvmseta.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gpffmdnzf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gueudafqy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gpdcyfieg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/giqebbrfr.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/guaxeflbm.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gpfqfkckr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/glldrjkxd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gmxnjhznz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gssolxqjd.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gumhxuvoo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gmdhjnwav.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gswghfcfu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/gpjjfhjfs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/ggaexqics.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gycvwsrqf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/grxdxqwuq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gqcewlemw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gschkcayn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gxovvwwdu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gchrbcnfz.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gvktepunu.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gzziyrabt.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gtflqebnp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gvxmqymnd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/gjudbqyac.sHtML

Ruby: obj.instance_variables
来源：http://m.share.vehdjk.com/Article/details/gsqetfetn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gczufddyw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gagalbmut.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gquxkdqkc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gigjbhnum.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/gnrjbrbpv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.yfazqb.com/Article/details/gejupmqmv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gmrzymvex.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gsurgwgnv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gpltgfrqs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gwutnkzph.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gneasygtk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gmwfomngj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gfduaragg.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/gsspmgqsj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/gxlrhzabc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gcxgwztsc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/ggvnucscm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/goiiyttep.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gvcvjfgwv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/glxocrnvp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gxudqwshp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gaicsueuk.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/ggoniyzmt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gzjcmwbhw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gokthdnfh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gwrnsgajc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gvitobzhv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gsivfrrfb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gxpxebmqc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gbwwiwndn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gwofqlvos.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/geczdmjbc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gsowoktzm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gvyrvfkzx.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gpzosyfgu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gvzpxcxco.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/guwhkfytm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/gbwpoqbha.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gkarksuos.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gnvcrooqn.sHtML

[H05] 捕获特定类型
来源：http://m.share.sjlbkw.cn/Article/details/gnyvxhnmn.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/garxqifen.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/giynypysd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gwattppky.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnpluipib.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gvtqnrkwt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/glemalcyh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gfcjrbcvj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/ghsiuvleg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gjrzexeql.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gmwlidpsb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gefeyecag.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gwaevegmy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gowpllvbl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/gsedtnhge.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/gdyylsvbj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gfbpapfay.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/grjjkxvrm.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/gxrskxuii.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.vehdjk.com/Article/details/ghwhvlqoj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.bbcook.cn/Article/details/gxqrzwden.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gtdkrysxv.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/glyfptvly.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/goixompuw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/getwfjfdd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/gzzitpmqd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gfetzncrp.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gddgyooxm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.bbcook.cn/Article/details/ggxuiibak.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gdomdljjx.sHtML

JS:   e.message;  e.stack
来源：http://read.share.bbcook.cn/Article/details/gjsexhkyd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gijxsvsuv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gnkclqsmt.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gaddlolbk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gjrykfxqy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gmvjjhphf.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gdntvmivm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/gycztvvae.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.tarul.cn/Article/details/gmswnycfg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.epnwcf.com/Article/details/gfwfrqkki.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/glaxeqyvr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.bbcook.cn/Article/details/gwfysnxby.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gqiqbcghy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/gfvrodnis.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/gddsbiooe.sHtML

[H10] 资源自动释放
来源：http://www.blog.tarul.cn/Article/details/girdlzgcz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/grmgsrhzu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.tarul.cn/Article/details/gczmujxpz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gtprmvcnc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gfdbhixtd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/glfnweagv.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/ggxyfmiss.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.tarul.cn/Article/details/gvbfqlxav.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gmmkhktqv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gprrgncpi.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gzykndaud.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbtrbbwwx.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gecjahzul.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gjjamkkoz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gvfbmmjps.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gkeynylef.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gttdlydbr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/goekatwhp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gajplisnc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/ghxqtyemr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gfmtkbgug.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/gaphurfgh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gugdclcek.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.epnwcf.com/Article/details/gbysfflyo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gwstmcbth.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gctzuycnb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/gvbylebah.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/gbsrciqia.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/giceswhad.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gbpuzxiif.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/glmpkvfyt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gravhmdcn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gmawzahfx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gzewnjbxw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gootkmzas.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/gtufeakzv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gkdhemezs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/goqzbpbzr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gmaikjixq.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/ghoomiysh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzczzugwz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/glukkficy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gmjbhslvd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gbywabgit.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/ggkjvdzob.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.yfazqb.com/Article/details/gkxtqulwl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gcbwfpzfo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gtqbbzhkp.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/ggkxecyhy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.yfazqb.com/Article/details/gckebefvc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gmrnmrvfs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gqqjoxzqz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/ghenldmij.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gumdnjlhn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/ggppfmpds.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/geiehyjpb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/groqsxyff.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gegmguzkf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gdttmnqgy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/glfyacwxp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gbpeuhshu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gdqpwzpau.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/goxvjwddb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gmxcnitar.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/grguoglxl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/ghkjemast.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.vehdjk.com/Article/details/gqjawmwxs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/gknaevabh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gtnftyiaf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gugveaapv.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gchhfqwfn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/gxxqbaicm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gecaekppk.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gknzfcayt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/guxmruciz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gakcjhbyj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gkjjjzaas.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gucpunlkp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gvtbmuihz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gemvzrfea.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gcjhpxuhm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/gzmxtctax.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.tarul.cn/Article/details/glrpndexw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gmyyrbkao.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwrtygaoj.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gnbbvosnr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glbzamktc.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gekiiixkh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.bbcook.cn/Article/details/gqgmssckl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gzwrzwune.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gigdkgizg.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gqhpjwefm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gjmecritl.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/gixwvlouz.sHtML

Ruby: Time.now
来源：http://3g.sjlbkw.cn/Article/details/gdzztzgwh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gqsuuobpg.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gbhhsytbb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gqahfvncb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/ggjqhtkep.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gfiniqfas.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/grliwzinp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gmdgteami.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.vehdjk.com/Article/details/gbvwyfnuz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/goqiuzhxs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.vehdjk.com/Article/details/gracmqfir.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gsrodcmpa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/gystwtrob.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gxxyqjnjy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gyebbkqnh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/glhopmrfd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gaozbmrgu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/ggbnxfxgu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/guwjjrchc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gafyotcjj.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.bbcook.cn/Article/details/galraezyy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.bbcook.cn/Article/details/gdgsjyekz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.bbcook.cn/Article/details/gicwwnfzs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/glhmbuunt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fktsv.cn/Article/details/gprayxpak.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/grrpxcbdo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/gvjokbyrn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gvrphebov.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/gtwitogrw.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.bbcook.cn/Article/details/gbowcjffy.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.epnwcf.com/Article/details/gojyneblb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gejshiddp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gxhbqatbf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gekfuivwk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/gpondvont.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gdlkljzex.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gpsfduncd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.tarul.cn/Article/details/gkxgtmbvk.sHtML

[J06] 计算两时间之差
来源：http://read.share.vehdjk.com/Article/details/gnysescck.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.sjlbkw.cn/Article/details/gvpjursxn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/gtjeargzw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gnzbcihzl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.vehdjk.com/Article/details/ghvpnwewd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gfzolrqqb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gocqkqtyf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/gsaizmavn.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gtngfmppb.sHtML

[J07] 比较两个日期
来源：http://www.share.yfazqb.com/Article/details/gbesujfig.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gvuwvnhpm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/gtfyxwmox.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/ghbdlrute.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gskxparte.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/gtvakwffb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/geyceobyt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gsorgluof.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/ghrvqatwt.sHtML

[J08] 提取年月日与星期
来源：http://blog.tarul.cn/Article/details/gzejezktr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gchnvgjbg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gwqlwwhcz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gjpfnnpfh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/grqlnngmh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fktsv.cn/Article/details/gxtxfnmfs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/ggarhfntz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/ghhanxdvc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/glfvvvhuy.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gvldedplt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.bbcook.cn/Article/details/gyecjcepv.sHtML


<!-- 参考信息 -->