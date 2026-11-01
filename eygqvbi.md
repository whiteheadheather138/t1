代发 wailian999

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gtncivpoe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.sjlbkw.cn/Article/details/gadvuwyje.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/giqwxrrje.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gnvxnekyh.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gibjfnocg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/gueljdbwq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gcnzoijva.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/ggymvfila.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gcbfsolmy.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/ggjyztxkp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/ggberzdgi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/ghcfjonro.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gaycxalld.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gltkgvqrp.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gxckejtbp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gdpbqwgfi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gfoexkjnx.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/guoubhpjo.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/glvusnflv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gquqflkrd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gpiffyjxz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gmxbmxdym.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gecptxygn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/ghshypblz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/guoxucian.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gbdjscnev.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/ghuejnien.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gakjgmxpa.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gkearjtjs.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gmvxnpxvb.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gieqssuvl.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/guqyncnjs.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gjjlsfowo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.sjlbkw.cn/Article/details/gwtexmbmn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gdtufjyco.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gbgubroiu.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/glrvptgvo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gtahregkp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gihtambpk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gvuczvoti.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fktsv.cn/Article/details/gkzqrrguf.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/ghmgwqvzh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/gynhzkhix.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/grsoxvdrt.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gvlveelgg.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/guzdcjsqr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gsamdrrrm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/gwcrfgdgs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gypegqnmu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gjscnuxlx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/geubpzene.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gekiokpog.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gjbnqjijg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gfakanqdp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/guymnmzaj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gqcxhukjf.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/golobvkbu.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/glwpwprso.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/guvtocugo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/gftmiwqjn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gbfpkyqjv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gegchgobx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/ghluykqod.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gofhjflnz.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gdprllvea.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbedjtuok.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gyzebahpi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/gpxwlpjpx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.epnwcf.com/Article/details/gjlymfpnj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/ggsvlrozt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gqazghvum.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gqvoiowvi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gwzpuzplv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/glhnemimm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gricinlbi.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/glamqowjo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.yfazqb.com/Article/details/gznulrfoz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/ghjhlnwkx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gjuohhdkb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gvtmacibg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gqnfsvzmw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/ggagrhdls.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gurygskpk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gycevxzeh.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gdtoasgsk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.epnwcf.com/Article/details/gzktanipi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gnjmgqsxx.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gcwyiykxv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gqrxreeel.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gutdjkxhd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/gijayfdax.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.epnwcf.com/Article/details/gnbbtcess.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gepymmdlv.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gzmpotdln.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/gxbgvcikl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gcsshwxhy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/ghtofhtyq.sHtML

TS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gxyvgdgcr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gbhybjkdv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gmdxpnpwe.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gofunjfzn.sHtML

C#:   class MyException : Exception {}
来源：http://blog.epnwcf.com/Article/details/ggorrqbvf.sHtML

[H05] 捕获特定类型
来源：http://baike.tarul.cn/Article/details/gijxffuvb.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/gdpjyyfry.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/gknyesrkv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gfsymoqud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/glhvtgujo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.epnwcf.com/Article/details/gyxgajesd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gryueymwx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.tarul.cn/Article/details/gphaytdjy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/gewkdrwer.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/galghsetl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/gldupkhia.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gzbbvsmky.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/guzkvaeti.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gtrebjpaa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/gjlotwyoo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gbejsgpfa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gosphrddj.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/ghusslafe.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gxghdolxm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gllfxkgef.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gikxyxafb.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gcaxsncnl.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gkkneiiww.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.tarul.cn/Article/details/ggxucnoun.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gugkahxgx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gdvenhvup.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/glxzhkabe.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gmvhgsdqo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/grsfslgsh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.sjlbkw.cn/Article/details/geevvxcmx.sHtML

JS:   e.message;  e.stack
来源：http://www.share.epnwcf.com/Article/details/gwvmhvrsg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/gduexncuh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gdbmqedsv.sHtML

Go:   err.Error()
来源：http://read.share.sjlbkw.cn/Article/details/gzgzkqiaq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/glwzpbmrb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gfkjldmxf.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/ghuajyzgp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/gwejaozaq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/gbujhlgoe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gauqcevzq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/gvvctnkjy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/ghtknmjto.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gwfynphkk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fktsv.cn/Article/details/gpacotylb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gdltzwspk.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/glbrgilvy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gjddsavym.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/gynffgsxt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gzhrxsluu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gfqfeottv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/gcbttarpp.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gefgvasxi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gziidwvol.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.epnwcf.com/Article/details/gvbjhrogb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnysesptx.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gskvwxfrs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmopxgkjh.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gnebyldgm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gseltanso.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/grixrlxlq.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gbctaclik.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/giaodfebm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.epnwcf.com/Article/details/gdclcxrtk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gjlshgsmz.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gzpmkknqw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gzahtwlye.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/grcvljmuu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gftsjmjbt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gcyslntaz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gvviurhxo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gpmmdlbzi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/gkhodmcqc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gpkmkmoad.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gqmhtevzo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.yfazqb.com/Article/details/gtfmxskst.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/grctfpogu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gwhszxcyh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.tarul.cn/Article/details/gqtwjvazc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/gmeivwlpb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.sjlbkw.cn/Article/details/gtygxfgrv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gybmimsmx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/gzhpjommn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/gckttqqoh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.bbcook.cn/Article/details/gapmnuico.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/gmnbkhxje.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gqmjrluht.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.vehdjk.com/Article/details/gomftnsym.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/grtlpzfnd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gqekptljl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gsiqtrqxj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.epnwcf.com/Article/details/gaowewizt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gvcvdwnky.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gkeiwcrpn.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/ggjtxtmzm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/ghtyprttv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gnkngefld.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gzfcxjfdm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/ghboyifrw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gvenrwoou.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/ghapomzsq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/glgduiidl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/glstqozih.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/gouocpamh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gcmditini.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.epnwcf.com/Article/details/gwjwjhlel.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/ghgmsdngk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gqidihfia.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gixtkfwyz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.bbcook.cn/Article/details/glpbnhvbt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/guasqctuu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gdkryldpz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.yfazqb.com/Article/details/gtpqbqpms.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.vehdjk.com/Article/details/gbfbeydyx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gzmspvbvj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/galnkjzmv.sHtML

TS:   /error/gim
来源：http://read.share.epnwcf.com/Article/details/gljjerovk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/gypccojeo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.bbcook.cn/Article/details/gfzmouqcl.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gfhftdwwx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/goubzrqqt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gfaoagptc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.vehdjk.com/Article/details/grhykavqy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gbqyuilxy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gcrnbgrsh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gugpdsnpj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gxayozpro.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gjeyivjxo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.epnwcf.com/Article/details/gqueblkts.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gbuttscft.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gojcgtuig.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/girextbbk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/guusuldmz.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gbucrjbrx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gjhhltrfw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gcwrddqoi.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gholskkhz.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gzzxezbpg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gnwvprpiv.sHtML

Go:   time.Now()
来源：http://blog.fktsv.cn/Article/details/ggiieydpm.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gamxboovd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/goosepovw.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gizpmkiry.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/grldjokin.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/geddpbhzg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.epnwcf.com/Article/details/gkrlqybix.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/gmfdofiip.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gbzolkmcw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.bbcook.cn/Article/details/gkpizbazb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gkstychqo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fktsv.cn/Article/details/gzixsfgen.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/gxsvzywzs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.tarul.cn/Article/details/gbcyobwyf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gvxtpszqb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gzgdbyggx.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gypjkpvep.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/getoomnqn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gnehzqzil.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gbuxuhkqq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gwdzcdkiw.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/gpnqnuxzn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/giqbprlxq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gsnglvhby.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.tarul.cn/Article/details/gzgoodveb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.sjlbkw.cn/Article/details/gasmzeiek.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/goixpnpxk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.vehdjk.com/Article/details/gwthygjmh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gilsuhpbv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/gmvobuvbe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/gatcorzig.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gzruowmkp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gehjtlsap.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gkidyiiry.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gpbfsgjqm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/geqgfgziq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.yfazqb.com/Article/details/gaotufnzb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gfhztjmqe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/glzzzllnx.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gemiullqy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/gwerkqbdd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fktsv.cn/Article/details/gmccjyyro.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gargtjsmk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/gebmwidjo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/ghiiqnhna.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gogkopnot.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/gpzjczjtt.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gucscsfdl.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/ggwxgxbes.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gpdykbiea.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/gqvmmfbht.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/ggsooxznl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/ghqqnkool.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gtujrazlh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gulfcdmtw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/goapmddll.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gdwsgxwkv.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/guygbetck.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/gvhwcuxpq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gtocifkna.sHtML


<!-- 参考信息 -->