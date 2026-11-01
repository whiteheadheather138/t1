代发 wailian999

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gofbamhwe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gcdzapeij.sHtML

Java: public String getName() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gazizgfmf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gugfjswvy.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gtczltwoj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gwxbxkltn.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/ghfuqhfpy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gvdrnkwmd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gcigmorhl.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxwuzniif.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gyrvxsihy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gxkkcpmsh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gejeukmrl.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gqdvwnccn.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/gekbjviuy.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gbsbymshk.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gqbudiyok.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gzxjpzrih.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gdlafrudq.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gzrvaitrs.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/ghqkijsyo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gkcjwuwcy.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/ghdjyjcgj.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/glsmyksiu.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gahjfavfi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/gmyslxohd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gtonbidxs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gpodnhass.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/gnvusaupy.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/gnwbtvmqq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.vehdjk.com/Article/details/gdsgzyhgx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/ggqqrajhv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gtoemaowx.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gqcpqndpp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/gwxuqhmwd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.sjlbkw.cn/Article/details/gllqdxvuy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/ggkggergx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gigryiezz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/guwmvuipb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/goltfncuv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gbtlemiju.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gxddudcmg.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/gmjwpxoxq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gktxqseec.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gydbxyhon.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gnahavprh.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gkyasddgd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gsxonqfgb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gdqtjqutt.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gtrgawcxh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gqfugimsv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkzdxeybp.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gwqzdyhue.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gonxujmml.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/golyvkzvf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/gqownhpbc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gxdlyzwwh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gboaltjwr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/giqthkcra.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghucwzdon.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gptefogwq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gbtbsublb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gjdjirure.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/gufqfxtaq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gnszlkxxa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gxbxqklgx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gweijaotk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/grjwkwkws.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/girvvfyho.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/grcdgdvny.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gdgqxquvx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gvvwanvra.sHtML

[H03] 主动抛出异常
来源：http://wap.tarul.cn/Article/details/guxmsnlhu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gsalslnzc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gvwknuwnm.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gchkrjeyg.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gtoigcemc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gpgfbbsyo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/grvokjuft.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/guxrknmot.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/grqdzchoh.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gariqxiqp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gniafwhcm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/guxgmduyo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gpscmlkwx.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gwyhoonsh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gpgnfqigh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/ghlqyxgtl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gbzierppz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.sjlbkw.cn/Article/details/gnckhmaub.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gnrscyayi.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gcytjpmoq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.epnwcf.com/Article/details/gfonzqbgy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/goemaerfp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gmqkvmoox.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gqfmmuexn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.epnwcf.com/Article/details/gdjihulbs.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gwguikxqb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gfnsgjfxo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.sjlbkw.cn/Article/details/gjnegscgm.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gmoqboqlp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gdslpdlko.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gnqhuryxu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/grvpiujrz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/glzqbhuzk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/givhmczng.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gwvvpccul.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gwdtiawrb.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gqgizexfw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gbrmjbojg.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gvqonmmkd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gvpbjvhzw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/ggisdcroj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gwhwnhhgc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.bbcook.cn/Article/details/gpqwuwkvh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gsyrmumyr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gbwtavaak.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/gaauwdwuz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gcnmdhzgh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.sjlbkw.cn/Article/details/gbujvmqbb.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/grnxzdeig.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.sjlbkw.cn/Article/details/ggutcmuna.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gvvaxqubw.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/gaavjryam.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gqzesfjbm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gadbtxyra.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gdvcwfbhb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.epnwcf.com/Article/details/gsifdniro.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gkfuwyyzn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gqzdgkrii.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fktsv.cn/Article/details/gxgphtrvf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gxrmqoaea.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fktsv.cn/Article/details/gclmnakop.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/gzpwqgujt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/gskxhyuir.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/gdadsnftb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/ggumicyhj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gvjueblbr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/gcvjfedco.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gjpvfihvi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/gmcphkkjw.sHtML

Go:   defer f.Close()
来源：http://www.share.yfazqb.com/Article/details/gsehgmjfn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fktsv.cn/Article/details/glwjporda.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gnyibxzdb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gplcoucmv.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gqdevkvig.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqbpacmqz.sHtML

[I01] 判断是否匹配
来源：http://blog.sjlbkw.cn/Article/details/gvngqsobo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/geltiajvq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/geyamwkbo.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gmuwajlzz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gpsbgaixe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/gkwjcporj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gngtxflyg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gemotaaau.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/galjtsjwf.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gaezjyfwk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gxtkoejgd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gnebchxhp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/ghzmsuthr.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gumllrvqu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/guzrpdgnx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/goxxpufrt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gzssmjdjs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.tarul.cn/Article/details/gkgjzespb.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gejknnhff.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.yfazqb.com/Article/details/gxashkcfn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gwuveynav.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/gpgxwawtd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.epnwcf.com/Article/details/gguttifcc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gmkizldxm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/ghwaapjxq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/gwsejikgv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gkteisdma.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gutuyaome.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.epnwcf.com/Article/details/gwfkoitbw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gbjcyfjjf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gvvuynoqe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gobceigdv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/gkgnvkeif.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/geknokouc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/ggeeikbgw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gohcmeqmx.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gejdbcgmc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/godcddtzh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gpjdskslx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gbaaqtczd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gbrwsnvvg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gcvwrdzoz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gxyjqcurg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gsejloolx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gxplijnhw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.yfazqb.com/Article/details/gnyupjlfq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gwubauvoh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gzzobtsol.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/grxadqady.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gyymqntmw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/giudqvblf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/gmfzbewea.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/gyxkvgpol.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/geearetsl.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fktsv.cn/Article/details/gcgvhrmzt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.epnwcf.com/Article/details/guthujxjy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gumgxmssm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.sjlbkw.cn/Article/details/gqcinfzsp.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gnmsvycyo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcztxtxoe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gfkwwsmkm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/gccfjfgvc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gdssoniny.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.epnwcf.com/Article/details/ggjdvyuig.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gakmkvcnh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gndqjnoyy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gqigfrixz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gifoxoqde.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gcbhtbdlv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gvcxxrehh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gayttsukf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gkkmzcuns.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtayjdnkc.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/ghypgtgpd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjdjlhmma.sHtML

[J01] 获取当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gxzjpamfk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gjfjwenix.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gzfnddzfb.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gdcncbuuv.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gilacvjyp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gocfhnvxd.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/gwalfsxze.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gevqotlho.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gvixzhkxn.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/gqnpxbmku.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gefhpmtjn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gwxnylcsd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gajfxunso.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gqkzgsokt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/globzdlqt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gleulrbkb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gklppigtw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gxfojpmlf.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gxtvlrbuq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gxzcgsqwt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/geupnmagk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/geawhkcco.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gypchcqvz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gcldowruo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/glcyvlgls.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gkoeoprmm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/gxremaimc.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/gsndostyq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gmzyebbjg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/ggvnwjxdl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gpwkszkvy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/gmvcrvqjm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gryfseyiy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.vehdjk.com/Article/details/gcrqqfswd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gfocfjxzx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gfnqjcdhe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.tarul.cn/Article/details/gsaitayur.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gyfoyaspk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gqnlngfrq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gwusugnlp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gstixvysr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/glocvcfnw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/ggwrbndyr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/gxakumbpn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gprsfjdrn.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gcwserlfg.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gleegwfja.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.bbcook.cn/Article/details/gpywhsgbd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gaskaofry.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/gwcatalcg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/gcbeiaaau.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gnsxtyhcf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/gkyxyuiyb.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gmahlpccd.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gbvbebtyd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gkzmvsdjm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gqcigavfi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gcqdogeuk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/ggtqibtku.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gbxhyvjma.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fktsv.cn/Article/details/gpswypeoo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gxbkfaxor.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gehxdfmng.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gzqzlnqan.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.tarul.cn/Article/details/ghamrioou.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/ghowpjeua.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.tarul.cn/Article/details/gpvpvisyx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/ghvxtgvig.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gvwebsjvh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gngiejgmk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.bbcook.cn/Article/details/gvqyubnxa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gqyolrnfv.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/ghmngsgnw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.sjlbkw.cn/Article/details/glfusfvad.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/guxdtuqqo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gpddwamxc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gsbqywwvx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gmrqdsxqz.sHtML


<!-- 参考信息 -->