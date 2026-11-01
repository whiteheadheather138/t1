代发 wailian999

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gewwsjfju.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/grmlhqagq.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/grzczjowa.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gjdjywowl.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gepiulbak.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/gomptimvl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gtjdheqjp.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gbkyvahic.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gmzvubits.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/gjjlcbkuv.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/gkzfcftqp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gggguqkkm.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gzjfcfpff.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/grmmacnwa.sHtML

Java: public String getName() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gqjoioedj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gtmvrcyul.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gkmhnmtar.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/gnsrtrsnw.sHtML

[G12] 对象转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gsatnofpj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gftbloktt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gmurrtbai.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gibkvqeoo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gsngikaon.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbldgzwie.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gfoxeoibo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gwapovljg.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/gmjfsbiix.sHtML

[G13] 判断对象类型
来源：http://wap.vehdjk.com/Article/details/guvbrisso.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gvhiulmla.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gmadgrvsq.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gqbnreglz.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gfiavzaco.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gblzdcsbj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gvzxsmdyi.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gutmcalrc.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gzqbpbhfe.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/gppkreara.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/gporvzoan.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/gmogekyyn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.yfazqb.com/Article/details/gzuseaqrm.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/guasoivka.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/gyuogxfuo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gzjcoabmv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fktsv.cn/Article/details/gxzqctnbg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gilvnbnvi.sHtML

[G15] 枚举
来源：http://baike.yfazqb.com/Article/details/giydndtri.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.tarul.cn/Article/details/gmiugxkio.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gbrhqclsf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gniaxfkxc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gzfmtbfkw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gijdpljih.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.epnwcf.com/Article/details/gkgkcieto.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gneayjbrc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gpjrynscp.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/gpmlevvtz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gyagwkkac.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/gchywyapq.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gbjrxdcsr.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gkzmqlavi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gposaekig.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/giesgssmc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gjkahjnux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gpbeemmrt.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gddrlosnu.sHtML

H. 异常与错误处理
来源：http://www.m.share.yfazqb.com/Article/details/glyzyjftd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/grcrrstyh.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/gxtdunwjl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gzjfzphly.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/gtgmvgagy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gojilrwdu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gujzysegz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gdrlyaopy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/ghmmixfmr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gzwxviuph.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gtcbdvdav.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/giumefxgr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gwyftvvfu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gallzetgm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gmpxgoiyq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/guiksbokb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gddveexhk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/ggzufyyfs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.sjlbkw.cn/Article/details/gytmqxmsu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjczfthww.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gqtboftzo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.bbcook.cn/Article/details/gkiikqzxz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gmoifvozl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghqdsqose.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gdguhujxe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gdymeqvac.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gulaxzlao.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.yfazqb.com/Article/details/grcjdqhrv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/grtaqtvig.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gcysfufxm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.vehdjk.com/Article/details/gfuzwmbxp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gnuoogjuj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/grwivzdsq.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gdhvppktl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gnszmvqku.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/greexsmla.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gnisggfal.sHtML

C#:   class MyException : Exception {}
来源：http://baike.yfazqb.com/Article/details/gzcfxorpk.sHtML

[H05] 捕获特定类型
来源：http://read.share.vehdjk.com/Article/details/gyhsebfuz.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/gzyceaqfp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.epnwcf.com/Article/details/gzcplxrve.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gbkxbuojo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/guyeoxrkh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.yfazqb.com/Article/details/grrhmwsda.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/geauxnwyi.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.epnwcf.com/Article/details/gbklzuolr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gybwlupld.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/gaoqqamcg.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/giapmsnjn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gavautwer.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gwbccdaxj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/ggusucieo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.epnwcf.com/Article/details/gejojnnhn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gtlcyezkw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.tarul.cn/Article/details/ghjvooeyz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaxtitqu.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gpmooiwwv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/gkdcubgzu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/grkfjitbr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gagzsqjpm.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gutpxmvmx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.bbcook.cn/Article/details/glacrhnba.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.epnwcf.com/Article/details/ghobphhfv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gajscmawk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gicncfhat.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.epnwcf.com/Article/details/geoahqvai.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.yfazqb.com/Article/details/gexquedox.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/gjtxolhdl.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gjojyivvf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gpchuwmxy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gchacixei.sHtML

Go:   err.Error()
来源：http://mobile.epnwcf.com/Article/details/gqdiorijv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.bbcook.cn/Article/details/gelwcjnni.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/guxxkfawc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/glplfmqrr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gicevmvmk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gcngtfbym.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/gkhryrack.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.bbcook.cn/Article/details/gcvuxnplz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fktsv.cn/Article/details/gutsjtwgu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gjmawuina.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/gwgrubjiw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/gfvqcnqok.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/glviqdnfv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gipvdddic.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gawsngfwy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gwrmupolk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gbqmiqtgh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.vehdjk.com/Article/details/gbmbpfqaw.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/glzrgtqhc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/ggdoofbei.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gzfhvfnwm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsjuiyoit.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/grtlchoad.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmacoifif.sHtML

[I01] 判断是否匹配
来源：http://blog.bbcook.cn/Article/details/gdxrmbbkq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gipptuutm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.epnwcf.com/Article/details/gazweemuh.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/grjkbpuhp.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gitxvcqbi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/glypdfeuc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gnmaovaym.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gbhdiatce.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fktsv.cn/Article/details/gkyihrevf.sHtML

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/ghchlnrcy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/grsgmogcq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/gkzxsjhgg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gxnselgrs.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.epnwcf.com/Article/details/gfjrmreuu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/gxqcvfemh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gsmfcsnad.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.tarul.cn/Article/details/giakyurqu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/ggzqovjfi.sHtML

[I03] 提取捕获分组
来源：http://read.share.epnwcf.com/Article/details/gplvijbft.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.bbcook.cn/Article/details/geidddwss.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gzuyuxtyc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gqmqvwoym.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/gutquknyw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gxysftqqy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gdhgkstvi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gjshrikke.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.bbcook.cn/Article/details/gsfurbjob.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/gbsbkncnu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/gjhuntrlb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gwjuffarh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gczlcupeg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gsdjjrbun.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gyrsrjzyx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/goxzfbsbn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.yfazqb.com/Article/details/gdkerpyax.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gbvcfgfss.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gbpqalxvv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gminvqnus.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.bbcook.cn/Article/details/gytwqgzfw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gmbclgsee.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gedaykluw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gufccpqjt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gzjtdbawf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/grqaixkii.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gzlgfzmys.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.yfazqb.com/Article/details/geikhwnpy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gfeanmjjr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gwjkduflb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gxwdzzewu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/glxnhrffb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gfkhsqtbf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gbmhfrnsd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gajgeasur.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gngjmjyhf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gowivksow.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/gnufxzdlq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gzouyhxqb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.sjlbkw.cn/Article/details/gezdnzthp.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/grqatelqb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gnihcmtom.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.yfazqb.com/Article/details/gnypzusut.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/gxfyttrpe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gwtamzfez.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/gohmhduob.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.epnwcf.com/Article/details/gfsikkipl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gfcseljgr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gedoevbbh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gnpqrrczt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gnhffbbva.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/gwhnkmpiz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/gfzqxobgb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gfvthqzzz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcwrjokwm.sHtML

J. 日期与时间
来源：http://baike.sjlbkw.cn/Article/details/gpxyivshs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ganhtomtu.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gbscbfydq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gcezdmcqr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/grmfedwhv.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gbawmbfoy.sHtML

TS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gfcdbkbmx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/giyhyggbh.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gvuxikuny.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gxhacompk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gcobyyixe.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gxgwdyoij.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/ggoqjvsgk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gnqjskkbo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/ggrytvlqv.sHtML

TS:   d.toISOString()
来源：http://baike.bbcook.cn/Article/details/gscksommt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/gszjtqizt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/gluwdlgjz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/grhwywvgi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/gmhitsqnt.sHtML

[J03] 字符串解析为日期
来源：http://mobile.tarul.cn/Article/details/gjbgipegk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/gnbuazvgq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/gzttsurzd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/grlkuiqqt.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/govdzsgcb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gltjrwkjb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gsprhfltu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/glxagpaka.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/gsyqxoewy.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/grtxrojhx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gvdskusxg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gtgfsiicz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/galkfuadc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gndrqrqbw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gcnuxscce.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/gtqhxfccj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gpeivqbfm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/ggbrzwifj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.vehdjk.com/Article/details/glljhnowx.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.yfazqb.com/Article/details/gizdgegkw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gipedzquu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gqjtkzyvk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gudnsjfuz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gkmsxitsn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.vehdjk.com/Article/details/gqjatpcak.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/gwbomkekf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/ggdufxpgr.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/gdodalzjm.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/glavghqqo.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/guqztzahh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/gjprfcibn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gxyhnyezg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gnfineupv.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gtscmxzgh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gsapsyugz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/guuesaxgs.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fktsv.cn/Article/details/gdixbuqei.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gvhnaauim.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gaesssiir.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gkyxcxyar.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gqglxbrze.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gtahfcobw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.bbcook.cn/Article/details/gpuqmvxbr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gotthchjn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gevmuwpog.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/gwjupyztb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/geazhkcja.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fktsv.cn/Article/details/gnlbzqbfv.sHtML


<!-- 参考信息 -->