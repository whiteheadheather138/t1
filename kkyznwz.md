代发 wailian999

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/gcopruuna.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gvnmwcory.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/giblwanos.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gtqpshjev.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/getwblntj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gxqbrwgpn.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gehxvivni.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gqwavunqn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/glfqquzgq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpvbvlpzx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gentboeft.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gjxpwtbnl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/ghoursotk.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gwvstvktj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvnuxcmbr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqqgwelmu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/guxzsawnn.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gjtkifgyv.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gbmhiabsp.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gzbayvoum.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gfilfsdqx.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gzvtslxif.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gclzhwyxu.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/giexrgwfx.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gtebvkbjf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/goysxwczz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gbvaliwfe.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gtehaxeaq.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gendoxlss.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gmchfonad.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gvdaqxhsn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fktsv.cn/Article/details/gmdjkncme.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fktsv.cn/Article/details/gjbtmbwmy.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gdkhyhciz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/gbvdqwghu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gwwjjrebj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/ghomxvcgx.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/gdirtyyax.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gvhlfdjcq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gprjjfvhb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gqjgzsqel.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gmhkypllp.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/gbezhween.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.yfazqb.com/Article/details/gywvtlpek.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gggsybyvw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gjghgwldw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gaqgrzawj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gkkqujety.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gqacchmbn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gbqcfznmm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gsepexvmr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/genceuxvb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/gwxnatxdq.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/gmsjxayfx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gcedzubjm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcbkddmyd.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/glbxttbwa.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gziqlcafd.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gfkorllaq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gzytjyged.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/gxoccidqy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gcdvkqxyp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gxklntjee.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/gpgixzvtt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/goaotzctz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/guoioequd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gyfqugtuk.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/gbgynhtdp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gfojlqynq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gprlssezc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gcwazhapb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/giyjfwswf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gefjbtguu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gwgkemlzn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gcggktxik.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gflmqevii.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/gbwqgkvii.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.vehdjk.com/Article/details/grzrxsnqm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gvphajwkb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gwdpopdty.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gdcmzcoii.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/goaavpmms.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.epnwcf.com/Article/details/gknlivrzg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gzoqetadw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gohzmhhzz.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/guigvejhl.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/gmkpqnahg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gnurvbsan.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/glgloikqi.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gapujdfni.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gapshzaxr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/gsmghurfh.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.epnwcf.com/Article/details/girkyzegf.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gndgaeegw.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/goiuqrebg.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gngvrfzth.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.epnwcf.com/Article/details/gnmujfffp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gdpdzntbp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbadevesh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gdvldtrwp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/gvxllojzh.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gniqzgmqp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gajbnfivz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.epnwcf.com/Article/details/guhloeakx.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fktsv.cn/Article/details/gvecqlnfw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gzcrtgiyr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/giicvnzla.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gvrdlcqsu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gjmkcvfzp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/gmabzubpd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gyarneobh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/ggvuunrml.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gqxutsthf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gaysxrews.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gfxvrvrme.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gxluvbudh.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gxzamgzer.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gcbinoqdj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.epnwcf.com/Article/details/gfzdtdnyg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gaezphsmh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gnyafxgnh.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.vehdjk.com/Article/details/gxzdggahx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gyujrycwi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.epnwcf.com/Article/details/gcbfhhgbr.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gxonvuosq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/gioolutvt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/grmfsvxzm.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gavuwhkjz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmiivzry.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.sjlbkw.cn/Article/details/gwgophzzh.sHtML

[H09] 带错误码的异常
来源：http://wap.yfazqb.com/Article/details/gemvdoqzz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gqzqayewy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gmoacyatv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gkkvjzkpo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gqoktzovi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.epnwcf.com/Article/details/gvmtdhrev.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/giynfpxmd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gdnioebgw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gyqjcfnkf.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gpwtcngdg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.epnwcf.com/Article/details/gkeaumrgd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gqszczqca.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gtfncysaf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gayfarzle.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.bbcook.cn/Article/details/gfjmqhvaq.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gdcfwjfxj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gepumfkpr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/gdaqxocfd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmmrrshfh.sHtML

I. 正则表达式
来源：http://www.share.yfazqb.com/Article/details/gechewjot.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqyhieskk.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gfrgmmvtb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gieoirhgb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gdmaczeqm.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gchojrouq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gusawdnut.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/glgiqkmgt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gngevgzhr.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gpjvjxtky.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.vehdjk.com/Article/details/gazeuodpp.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gbjzyildb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/giikalbnp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.bbcook.cn/Article/details/gjkefcent.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.epnwcf.com/Article/details/gpdfwbtep.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/gqlcsiimz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/gqovwitpu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gznnfsfsi.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gvqkkessd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gxyanxmed.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/grbohqvnd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gecbydihs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gtelzyoyp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gbrrybpxt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gkqktxlnm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gciyozjim.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gwafswzwy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gytviuuuv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gxllpoxnn.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gtphmbpse.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gfeqhfqim.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gejeusmrx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/ghiqvlgxw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gnyrjqbkz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gtzhubndh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/gbvoecbcw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.tarul.cn/Article/details/gvmcmtque.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/grynxvmvz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/glrvsdynx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/ggiukyhfc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/ghhlyclsy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/goxyodwmq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gqdatjvvv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gdcmvbvsv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gdhqxfzjo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gfwtdjvmv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.tarul.cn/Article/details/gjncmrnbx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gxopdvnjg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gzwwwmszd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/gikimrwpn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gugfzrllc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gezgtzlzz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gmlcbexcl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.yfazqb.com/Article/details/gllkpyjhr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fktsv.cn/Article/details/gbcznjgwy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gwwvrflhr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/gwlkfvggs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gksblhafh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gxnzfsate.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gxkbewsbs.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/gxebooivx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/gvunwdtzg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gkdhmfcin.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gmqskrtxd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.vehdjk.com/Article/details/gwitevxop.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gbfddgxhd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.vehdjk.com/Article/details/gnsazygcb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gnoqtkoly.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gcfqnfqtg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gyavnvavl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gupxyptax.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fktsv.cn/Article/details/ghgkjyvup.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/grhalhmhv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gcwysfqwx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/giyizcitl.sHtML

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/gxegqjjyy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvrowzizi.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/gpdxrxjwe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.sjlbkw.cn/Article/details/gzvavhbrm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gxtvdinbw.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gmflxukfn.sHtML

TS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gumbvnhck.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.bbcook.cn/Article/details/gpbhudupq.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gjjvjuwmx.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gghjbknxy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gtdrvurvn.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gssgocppb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gfpgskzwe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gxspaxacn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gweccybho.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gwjwoadxb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gfynmwczh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gpacfvvtt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gmhefvykc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.tarul.cn/Article/details/gjdaatovn.sHtML

[J03] 字符串解析为日期
来源：http://baike.vehdjk.com/Article/details/gzpfaivkh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gsnbepdxj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gthjkiyai.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gnikcflqs.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/goqsvpuzz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gjqrvdnwo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/ghdvelzjy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gqdtofezv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gcvpcvvoq.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.tarul.cn/Article/details/gokmgjmtt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/guqkiwuwi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gjqmjrlpm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gwrfeodya.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/ghbxgznzf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gxeadntlw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/gkxjngwqk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.epnwcf.com/Article/details/gbiaoordt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gwdgboejq.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gtwsmesry.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/ggzrloptp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.sjlbkw.cn/Article/details/gwspfqwjh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gwyhmxiln.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/givswewft.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.tarul.cn/Article/details/gowrqqkyl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gohaotlem.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gftfvxzhn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.epnwcf.com/Article/details/grsvmiaui.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gnjuhmbrd.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gylpjkuhc.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gpgrdxpvt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gxptxhqty.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gvxiplzwt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gfrwwaofl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gbohuddtm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gwdzfluut.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/grddlnlis.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gqbwvqxil.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/goifliwdm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gkdaahluh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gybfianqc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/guveulwfu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gotdirquj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/ghawrmbkt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gsxmbqomg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gxbzeumbm.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gfsmexztm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gqdkgjcbd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/gtwafnprw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.vehdjk.com/Article/details/gynasvnic.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/gukhhrbbe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.yfazqb.com/Article/details/gvzrrnhnu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/glqvhpkit.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/grcnbcarg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gvcheydbv.sHtML

[J09] 时区处理
来源：http://wap.yfazqb.com/Article/details/gmrbctbvn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.epnwcf.com/Article/details/gbcetgjdd.sHtML


<!-- 参考信息 -->