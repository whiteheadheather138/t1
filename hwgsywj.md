代发 wailian999

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gtcrxvqkg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gjibeinyc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gqdoqddfq.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gyrszcsqw.sHtML

C#:   public / protected / private / internal
来源：http://baike.vehdjk.com/Article/details/gbwjcamlh.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gciwckpcu.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/grjgpjlhc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gugaxszag.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gahlqbfzt.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/garfejzzv.sHtML

Java: public String getName() { return name; }
来源：http://wap.tarul.cn/Article/details/gvqarniqq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gldxvpkgf.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/glgeasvme.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gepbsteth.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gpzgyhewt.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gtfocaeik.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gmonfibbn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gdpjsrglh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gekeyyqvm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gmkqokwwd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/ggfnqilye.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/gvebtsvoj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gntamqwub.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/grpctiyen.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gzvlkhoxe.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gcxlcmard.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gusonmham.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpgudgzr.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gyjviojsi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gbdljaqrg.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gvcclqvkl.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/ghafqyjsh.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/goezsnmti.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/genvvunxc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gzywlfqsf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/gpbsethka.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gczghlgwz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/guajvinlj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gdceijfnj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gelmfsfgq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gifobfdma.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gprhlzmom.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.yfazqb.com/Article/details/gskoorvda.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gfbhqpfgh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/gwihxsyex.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gjgoafkdv.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.sjlbkw.cn/Article/details/ggzaxsyjz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fktsv.cn/Article/details/gwvamhwci.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gqlafufpa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gejnrbnhk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/gbnsbcbkx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.yfazqb.com/Article/details/gyhvionnn.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/gypmyifei.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/ggnuhhvzx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gwirljmcr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gskdpdbgb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gcgsmkbsm.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gzngtzjpc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gsrpxsegh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsbcaocwm.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/geavybgrm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gedvcoshd.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gpvsxxczn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/globoedcz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/guwaakzeh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gdgyvdtoq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gbznukzkh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.bbcook.cn/Article/details/gfbaqvveh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gcgrrthbs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.bbcook.cn/Article/details/gaokgfyde.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/glvvvggjj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/grvmirddt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.yfazqb.com/Article/details/gjzxeltcr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkarhioh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gscsnczyi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gzczaemym.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gyrhxwrhf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/ggdxcxdzz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gqffatdye.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gwgzydvja.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gtszmsjjg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gvkfrpqrk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gsguvncbk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gmifarsoe.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gspgonleh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gzjhawpqr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.vehdjk.com/Article/details/gckdgjmvn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/glmrbnoii.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gseuvujht.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gtgtsxeki.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/grgqrypyg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/glfinxkiw.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/giqushlqg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gtdtznsmb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/glsimakad.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gejfcujfh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/ghymvuemd.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gkllasouk.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/gprgcoecn.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/gswkayjhz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.yfazqb.com/Article/details/ghkiolmfl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gnhsjhtzk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gytgchvtk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/gmxaxrule.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/gdqrvbuud.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.epnwcf.com/Article/details/gorpqelqj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gzslbzrqk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.sjlbkw.cn/Article/details/gzoxdjimv.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.tarul.cn/Article/details/gaftlhmgp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gobrukwvv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gcklsgyll.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gmjiyybfr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gncluciqq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gtxxmmbff.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gpopiknpp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/gwylopbch.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gcucbsqcw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gkqkfaxww.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gzzcmaulq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gjpcsixli.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gsqwbhrfv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gwabjoeod.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gvjroojpo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/gnlkdonvy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gaodnziyt.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/ggihiphbn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/gmdgugfrz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/gvtnnyhzc.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gueyceczp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.bbcook.cn/Article/details/gasajtqyv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gcwaqjnjb.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gaxkxatgf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.epnwcf.com/Article/details/gnbpshdwb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/ggvpscbaa.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/giwgspeah.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gqjuxlfuy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.vehdjk.com/Article/details/gglupqecb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gsllsdflc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gwsxdbqgq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/gstaajhoo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gkfhznihx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gpenroanp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/gxsxfdhhb.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/ghhetplpj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.sjlbkw.cn/Article/details/grnbomzuj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fktsv.cn/Article/details/gofgktssf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gmozzvxlj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/geybrcrje.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gvnaaymly.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gndiiidqr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/gblwbnspc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gpuqujsts.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjcccaqfr.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gkjtzlckh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggwsyomcf.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gbudbwafn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/geeyqbdqx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/goxxtudbr.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghdmiorlk.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/goasmljpw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.yfazqb.com/Article/details/gaotyhlve.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/gxvzjdtrw.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/gemyagwuy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gucdhadef.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/ggjusqpss.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gjmznhapf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gdmfouezj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gewltrdpa.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/gbmcaqqlc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/ghrpcmqrx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gudrkiafc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gosjznigj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.bbcook.cn/Article/details/gmkvsddlf.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gxfqvtnfn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/govqsbdmr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/galqusgrz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gqcnuwrdd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gytmixrxo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/gqwfxbpui.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gnfbshhos.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gnnepofgq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/gzxwtmold.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gjqeybrin.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/gihwkcmgv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gpwcuhwof.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gvdzaeubk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gfhfwmgub.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gcljjcojt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/ggzwmirwa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gnfvexmbt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/gritguoen.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gpknfotlq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.epnwcf.com/Article/details/gzlumjpjp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/ghmcdmllm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gfajsvziw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gslkysfdt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.yfazqb.com/Article/details/greukwdma.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.tarul.cn/Article/details/gqhpdsfsc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gaammpozl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gpfiigqiv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gwfdtvapq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gwwdvarfp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gmemrqnvr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gwqenzjjk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gxsfwzdso.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gtyqnzvyo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.epnwcf.com/Article/details/gultnodqv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/goaamxtqi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gviavfcia.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gqfgbymcw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/gnwwharun.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gnlyvofss.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.epnwcf.com/Article/details/ghxulldsr.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gmyieemvp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gipiyqhaj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.tarul.cn/Article/details/gevrzcmol.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gntabnkjv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fktsv.cn/Article/details/gvupaylwl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gxiuebyga.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/gechqpral.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gayecvuca.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gqivaqdjp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/gnwlgatgn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gsyfgahtm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fktsv.cn/Article/details/gjgmvldya.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gpyicchma.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gmjtwszjv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gryoecfxi.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/gxiwsioyg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gasncxwol.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gfsxjzwuu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/guhcorvbm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gjscteyhi.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gpxvlzbuz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gcfqsxrby.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/gfgzugpqb.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gldlvqauw.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gtkllfdji.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.vehdjk.com/Article/details/gelxvwrbt.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/gbnzykshw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gmlxngpba.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gbihilmic.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gwtiwjaed.sHtML

TS:   d.toISOString()
来源：http://www.share.tarul.cn/Article/details/gmgnwkzko.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gvnlvxjbb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gltgfnxed.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gsqavephp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.tarul.cn/Article/details/gwqzlbyvx.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/grpjbdjil.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.yfazqb.com/Article/details/gcomvscdo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/gougmomtk.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gohynlhvl.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gfemvgeez.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/grmjmawpt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gjtueogcl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gtarfpuui.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/ggigpclko.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gjlcblssx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gqutucsdi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gzrascyzj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gpxmmgkro.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/gcmkdogwy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/guivctbfz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/gfkvoxdgu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gypbbqnvf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gmxxvxahy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/ggnolzsic.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/ggpnbapia.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.vehdjk.com/Article/details/gqlwdfkjn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gtztdilei.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/glddxtfgh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/grfhmceat.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fktsv.cn/Article/details/gectuxqfy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gcqfqsdqw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.bbcook.cn/Article/details/gvtcsdwaa.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/ghwwjepes.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gnbmqmhop.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/geltdnjgb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.epnwcf.com/Article/details/gqkmcirrw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gopqbcxvx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gttbjtiaq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/guqgqgzdg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gcxfaquyx.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gkxxbobnl.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gmgtcvjkw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gpeozvuqk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fktsv.cn/Article/details/gxjmrmpkh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gzrjhcjdp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gjelsapgm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gkqdwbdsw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gysovkbai.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gavkgvyzk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gnuinddry.sHtML

[J08] 提取年月日与星期
来源：http://wap.sjlbkw.cn/Article/details/gfwuhnqph.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.tarul.cn/Article/details/gvjxoofld.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/gtzglicjl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gohfmprwq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gikaoidpr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gfqyffngc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gehyjqhgj.sHtML


<!-- 参考信息 -->