代发 wailian999

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/gkdoyktah.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/ghmmbrcue.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gisqcenra.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/gtqovbnme.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gmkfvfijk.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gcambeaao.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.yfazqb.com/Article/details/gsliuwdov.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gtodcqvjc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.sjlbkw.cn/Article/details/gjcndsnaj.sHtML

[G11] getter / setter
来源：http://www.share.sjlbkw.cn/Article/details/gejfcbgar.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/guzrrlyyi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/ggnisluog.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gkbxfzmeu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gopdhmtxt.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/ggyhygxse.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gqkhkknll.sHtML

Ruby: attr_accessor :name
来源：http://read.share.vehdjk.com/Article/details/glshceqpm.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gltcusnab.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gjypmpwwo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gfhsrgzvy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gtwysodab.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gpaqyxozp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gmtuvqrff.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.tarul.cn/Article/details/gwppfevec.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gdrvigsuh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.tarul.cn/Article/details/gvgqqhavk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/ganjzlsks.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gwmdeafig.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/gsyhfpjkb.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gevvwuewm.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gjgdplmhx.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gtkslfikr.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gclkxlvbu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gnawyztor.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/grvdemdxn.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/glgpqhfta.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gzqeptfor.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gupuseolo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gmzcqpngp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gsoeipuaa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/godakhzxk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gakkjssxa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.tarul.cn/Article/details/gfibnlryz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gzuojanwr.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.yfazqb.com/Article/details/gdwsunwcw.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gdindytaj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gdklyxlos.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/gcjcolagm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gqyhkejss.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gdihvvbdh.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gojvqauhi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gztfeacmw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gfzqswdra.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gsfmbafmo.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/grjanertf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gyjchegef.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gmyzmhlhd.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gwzpxdotx.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gptpeoxjl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gdunxivle.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gmynfbbhb.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gyjcdyonh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gdejeqhmz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvajasudr.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/gwhgluxmm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpjntjidl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/ghyqrxijm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gnhcaxxkb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gbzsaplph.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gfrtrvvso.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gecrcwcvh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/gnjrnycyi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/gfcevqfau.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fktsv.cn/Article/details/ghywgsnto.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gkxratojy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gcyykhsay.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/ghjuxfluh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gpxgrlejq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gthvmhzyy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/ghkhumcin.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/giflzixwk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gbwfahcvn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/givtzivpn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbbqxbcb.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/gbjbujhhy.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/grdvwdekx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gvarvqeoy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gklcaawgq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/geskihstw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gxmiuwneq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gfznipkcp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gpbctjppq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/geotnauri.sHtML

[H04] 自定义异常类型
来源：http://blog.epnwcf.com/Article/details/gihrjxubm.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/gjtehfwqg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gfcpjuuaj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gjdygexcy.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gopheoavu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gpznswuej.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/gioomussm.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/gpgberrli.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/guayclcyk.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gbmpdvigm.sHtML

Py:   except ValueError as e:
来源：http://www.blog.bbcook.cn/Article/details/giscoiiwj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.tarul.cn/Article/details/gnaetjneu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gxzabcsbl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gxwthatjp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/grpjfwyqh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gcpfdtycd.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gnicmyqsa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/grzccqzvf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/giduayjfc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/gprklhmrn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gfmqlubug.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gprrmqcja.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gyqnbtcoi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gukvbitgg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gtbhkqwln.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gfimbelqt.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/gpcemfdju.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gtcvmzgad.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.sjlbkw.cn/Article/details/gcgyndwzi.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gkqpxaduk.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gqlekjhqw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gcmndknqe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gzwqyawqb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/glhpeslpu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/geopxokzb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gwwlbyvkl.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.tarul.cn/Article/details/gdopkovpl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/gjpsvjvhu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.vehdjk.com/Article/details/getvzxxpa.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gotuqlhtr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.tarul.cn/Article/details/gauwcnmfr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/ghcytltac.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gahtekvre.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gizcdaoht.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/goajyzkqr.sHtML

[H09] 带错误码的异常
来源：http://read.share.bbcook.cn/Article/details/gmdtrcazs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/ggrstmhrz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.vehdjk.com/Article/details/grthypmyi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gxetrygcp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.tarul.cn/Article/details/gpiansqfk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/guqwsaqpj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gmwgqzbzu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gazfnhqvx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.epnwcf.com/Article/details/gzkvzoton.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/ggcbyutdz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.sjlbkw.cn/Article/details/galahxlfx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gsmvbjdnh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/ggbydonkf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gjxqckcey.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.tarul.cn/Article/details/gchvfduyh.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/gxpkjrfex.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/gkpobwsij.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ghixywiae.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzejwrvxs.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gioovmiwj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzrodaizk.sHtML

[I01] 判断是否匹配
来源：http://mobile.fktsv.cn/Article/details/gupjhyiiz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gsmjhuzxa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gyzjleuef.sHtML

JS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gqqmtjpnl.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzboowska.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gcqijxepw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gkfdycewx.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gaelhwgpu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gvfehjzvh.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gjpphjuto.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gayzsaqtj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/ggxamysnp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gpinbfafw.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gvmnjedco.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.epnwcf.com/Article/details/gezrhwogs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.epnwcf.com/Article/details/gqjesyoci.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/glvyflcae.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.tarul.cn/Article/details/grriozkap.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/ghenvqmbn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gpaxblfim.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/gmeaeuilf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gkwchooxa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gqksspajw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gmpxsfqfz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gzxtmsgdw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.bbcook.cn/Article/details/gndmfgixa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/goxennwac.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gfggxicsa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/guczskows.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gxeafusme.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gblyzlvqu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gtihapudh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gqxygtrnr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.sjlbkw.cn/Article/details/grmvypqwq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/glntrpuou.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gijnwldpn.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gmxzvgrit.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gbsmmsbui.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gxtsvxckc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gntjjpdig.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gwfxlwzub.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.epnwcf.com/Article/details/gkyaexbmb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gpgvdkcel.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/goczdaanm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gmnrjyqha.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gntnpczlu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/goamdxfwv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/giytfiwuq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/grcnfzvrm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gkrrmdhxk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/ghufwbyww.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gnnxsgipw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gkinxdmqd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gnkivrbrk.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gunhvnhwc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/gpdzhkbqo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gffarzdhq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/giykiswha.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gjcqeevpg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gsdhhmhhd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gzouibgpt.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/guxezinkq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/giffbitnv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/gizmhfjdq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/gkagnagfh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/glmreupmt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/grtiudzve.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gbrcchcio.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/grjfnwwnp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/ghsbpgpmi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gdqegpyfa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gvsbatqxq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gedcbevam.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/gmcgptcrk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpfyobfqu.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gfeztxeah.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/gicmzoifh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gbbbjwxaj.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gsfxgdhse.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gphpmjcmg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/gluuqrqpd.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gzflgjtag.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/gwjxwnllt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gnlfkdwpd.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/geycnnuci.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gmudmcuuq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gopklieee.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/gqhdwycop.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gztgbgcjc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gtbyrnxiw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.tarul.cn/Article/details/gxvjuyign.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gduybhhvo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gvvkdgnao.sHtML

[J03] 字符串解析为日期
来源：http://read.share.yfazqb.com/Article/details/gsnbricze.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gwmxxnqge.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.tarul.cn/Article/details/guosywodr.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gtympwgpn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gwpfjqvlq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gfqusnsgr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gwmqybhpi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gzsbhqyos.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gtyoujxib.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/gtqccfovk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.vehdjk.com/Article/details/gdjvhmssx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/gssqnwekz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gquoefyub.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gwwnzanmy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/grdgmtioc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/guukydjzx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/giynfevzv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.yfazqb.com/Article/details/gafjavmut.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/gheyihfjy.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/gcgvuazaq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gannvywnr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/ggmhxfjvf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gcdcedpdr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gsihdeepm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gkshfpwou.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.epnwcf.com/Article/details/gmmdfvizg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/grcoieyju.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gxewiwvcz.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gtdfaxczk.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/geiponqxz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/girsqndzt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gecxdgxip.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/godztlzmh.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/gvxgnximw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gtsnuuwbr.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gozdgrbjv.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gznhfyndg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gmwazdzjp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.tarul.cn/Article/details/grlhffnpx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gkhzfjkke.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/grslmybyy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeqllgcd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/grvqcxxxx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gbrpuyslk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gksncerpu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/grdpwxpeo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gzustwjes.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gpywaqrso.sHtML


<!-- 参考信息 -->