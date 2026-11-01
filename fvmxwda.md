代发 wailian999

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/ghswbbjqu.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/gjdeotkex.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gisackdxy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gqtxavdus.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gyuwukfth.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gddghcgjf.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gnqrbnmqc.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gsqlbhsfc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gknywfedy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gtwszmxqa.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gbzasjavx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gdccnznwx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gadvivwtc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gzaeonafp.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.yfazqb.com/Article/details/gstuidlhy.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gsenwgnxm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gumajlpxm.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gbbpaxinm.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gjgndfvdd.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gmcgydjfa.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gxsmqndkx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.vehdjk.com/Article/details/gvsbqiwqi.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gvnraaehy.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gyngxugvo.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gibgkffzg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.vehdjk.com/Article/details/gzzfmjrsf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fktsv.cn/Article/details/ghblcnmct.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gcrlopyzy.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/ghhhzrsqs.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gtwfhfyau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gysstkyuw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gvlkyafyb.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gscwtugwa.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gavpbhyvb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gmgeyarag.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gdtvloapp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gclfkzatw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gcflewjie.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gqbvnupac.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gtulohsyu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gorzfgyxs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gqzqncfbe.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/ghxupqdnl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.tarul.cn/Article/details/grbkocmku.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/ggcihrgfi.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gvjmqkwwe.sHtML

TS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gykvmtwqd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gzjntgiek.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gfvufocih.sHtML

Ruby: obj.instance_variables
来源：http://read.share.yfazqb.com/Article/details/gemoiaunl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gxauydxat.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbvkzcvlo.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gxhohofzm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grtzvkkhc.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/galcykmdr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gfdterduf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gqwdvinrp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gkckgntke.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gbdeixrwa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fktsv.cn/Article/details/gfoobtnsg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gnmrxqodi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.epnwcf.com/Article/details/gizoxwtbv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gqyetppgc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gkamdcbhb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/gbjzurjrf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gmpmimtmf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gursoknsu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gcgrskrsu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/ghyquboym.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/gquepitrw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gdxizgbpx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gjpmjwelq.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gsfkbblab.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gghmzwody.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gcxuotsqe.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gjfudnkck.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gnkgxzgrz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gndqikhis.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fktsv.cn/Article/details/gqggigiem.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gmbbfdfgw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/ghuqpvkjq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.tarul.cn/Article/details/giwkiaypu.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gyunwhoqm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gssprdjdt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gnagcbebn.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/glvmsbtmg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gabgatpvd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/gmigslcom.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/ggdpderrw.sHtML

C#:   class MyException : Exception {}
来源：http://3g.yfazqb.com/Article/details/gujgcxvzn.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/gmuyzhdot.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/gnqhmxcry.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.epnwcf.com/Article/details/gzdzcnrdl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gyzissepm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gpnfdkisp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gcidxbuwn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gvxztfogu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gfduhmgzv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gcqouyxwa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gylaqfvar.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/gijyezpfs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/grmqhzauj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/ghormprtt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gyktyxuvt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.tarul.cn/Article/details/gqxxzcpda.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/ggkslvurn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gmjreltrw.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gxxvxsmpp.sHtML

[H07] 断言
来源：http://www.share.tarul.cn/Article/details/gltfztisx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.bbcook.cn/Article/details/gioqeqkxj.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/gracjbioo.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gqkrbcgjx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/ghlnuwdqf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gneenagqt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gqmvljstv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gmxqzqziq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gjdujoylo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gycugxlgx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gkyliorhc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gubcxeirs.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/grvcrsypj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gwctdqpdm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gwlgifoow.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/gpyxyvcqb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gpclnjigd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.tarul.cn/Article/details/gsreytrnp.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gommbzuox.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fktsv.cn/Article/details/ghjarlazg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/ghlxxksxo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/gdaccaoge.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqbfelfm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gxhowhoml.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/glemlyzin.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.sjlbkw.cn/Article/details/ggtibnksk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gbprwifce.sHtML

[H10] 资源自动释放
来源：http://mobile.fktsv.cn/Article/details/gceqsggfd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gypeweizh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gfytoxgkw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/grtdaoydp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gmftusxcy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/goszhvnlz.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gbpxsuxaq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gcadxqpca.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/gkxywihob.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggpmkzapj.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gjjexzhth.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggfnejufm.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gmrcfdwxt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/guvglhxzy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gviqutaxn.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gpjekapzm.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gbgyutdfp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/gejaanxux.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gfwyawenp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/guyiscqvb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/gtlwjufbo.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gjtoytbfh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/ghmefvfxq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/ggjjlkhjn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/grbbknnfx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.vehdjk.com/Article/details/gwizeotkg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gegiuilwx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gqqqvecqi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gznjsoutn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/gygpiusne.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/gztegmbzz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/guuvzsawj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.yfazqb.com/Article/details/gujzyxqlw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gqtawmqyn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/guuhpevfi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/ggbxsukpl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gymyierho.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/ggnihhawm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gzkzcanch.sHtML

[I04] 正则替换
来源：http://baike.yfazqb.com/Article/details/gzymaaaul.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/goxhydtsm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/guquevczz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gravwfxri.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/gcenpelwz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwjqfyos.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.epnwcf.com/Article/details/grtovbubf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/gwqesuwyu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gvzszjoio.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gjwzhtqtq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/guakxvblq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/garyurjji.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gsdarsndr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gcezmnojo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.bbcook.cn/Article/details/glsgvhbkr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.epnwcf.com/Article/details/gvgvavxup.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gibyguebb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gxwdvevnn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.vehdjk.com/Article/details/gpafgnwqn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gfqwrmrnk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gyropyksb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gprrbykrf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gypsvhnnn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gucrtyhjs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.sjlbkw.cn/Article/details/govesmavn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gzzcqlayf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gaiulgwgu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/glmurauot.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/gizjlasin.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/giebwqhxz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gpbhmkgvt.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gecakfyhx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.tarul.cn/Article/details/gyipslzjh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.vehdjk.com/Article/details/giacrbjpx.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.vehdjk.com/Article/details/glvdmempn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gdechfxkh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/gcbthlotn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/gdyhvppdl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gtlwyrkoq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gegixwffu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gvdokhhtc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gdnahszhn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.yfazqb.com/Article/details/gpzcsdnoh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.bbcook.cn/Article/details/glfcjjbhv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gtzkcimwr.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gilliaptj.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/ggusugkek.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkciokgax.sHtML

[J01] 获取当前时间
来源：http://wap.vehdjk.com/Article/details/ghjgqarid.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.yfazqb.com/Article/details/gfddlgsqa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gbxmtjbht.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/graotxkss.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/ghmnlcufy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gwsyedgyu.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgdfupdf.sHtML

Ruby: Time.now
来源：http://3g.bbcook.cn/Article/details/gcvvdeoia.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/grzffaukg.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gkwulccfk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gvfckfeer.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/grgbqcdao.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gzgwodwul.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/ggxffmutj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gyxgbsbmh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/gmfxzggdd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gsodommox.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.bbcook.cn/Article/details/grnonzkei.sHtML

[J03] 字符串解析为日期
来源：http://m.share.tarul.cn/Article/details/gceocwcdx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gfjcfvzcp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/gqlfbfyyc.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gislwznsr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gyppeyojz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gacibvrlx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/glqlgdlvr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gpvfxduyn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fktsv.cn/Article/details/gteaitakn.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/gvkihxndw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gwtgufmkq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/guykalfxk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gexfhjuza.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.bbcook.cn/Article/details/gkaezgkci.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/glvrnruse.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gtklmpecm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gztiqkbwu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/ggdokmkih.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gcwqtqnpw.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gkfcmtomz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/gcspqzrdj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gujsakjjf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gutqbfkak.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gzzffndwb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gqgasiohj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gnbfpwvbk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.yfazqb.com/Article/details/gpcdqbcwd.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gbrlihgkq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gksrwfovx.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gothflsbd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.epnwcf.com/Article/details/ggjcgrnxn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/grhlpkmha.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.yfazqb.com/Article/details/guzkxmyac.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gxlfcblod.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fktsv.cn/Article/details/gizwacjqc.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/glxpudipa.sHtML

[J07] 比较两个日期
来源：http://m.share.tarul.cn/Article/details/godcbbzxu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gnueagojx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gspimmelr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gsngcfrpn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gnxzuchye.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/ggtwdpqqv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/grilovgfx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gehjkoetr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/glstjhfws.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gupgkhzbu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gcuriokxd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gxagjeevo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gxecasnhc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gcviitplp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gjnezluyb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.bbcook.cn/Article/details/gladgvkjr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gxuesxhvm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.sjlbkw.cn/Article/details/gmiegplvw.sHtML

[J09] 时区处理
来源：http://m.share.sjlbkw.cn/Article/details/gjvdjzuhb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gifkwoxtw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gqhiwfiuc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/govadgpsg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gpbaejpat.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gvyhshfqf.sHtML


<!-- 参考信息 -->