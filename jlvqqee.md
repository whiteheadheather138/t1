代发 wailian999

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gvythpmsc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gpghmfzvu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/ggtqnlywt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/geneookoy.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gydcyihnc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/gqknnrhcz.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/gcfaueqxs.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fktsv.cn/Article/details/gddcpwude.sHtML

TS:   public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gjbbksqfs.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.bbcook.cn/Article/details/gulnbduac.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gkxpyivum.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gyycwmztg.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/giabgevbc.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gcqqrhcio.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gdypsogef.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gmuhyfsto.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grqhhostc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gnpypebdv.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gkmjebzhm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/guzvkuzsr.sHtML

Ruby: attr_accessor :name
来源：http://read.share.vehdjk.com/Article/details/geyhdinek.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/gncbhkmdz.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gwjhfkzxt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gfzcpkjpe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gjtzqyxax.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gqupbnwpl.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gbvqdlimi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggmlvshvo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gxtwpjyup.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gsqkpjwlf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gahtjmnqq.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/gqvcortyy.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/ggabhgwei.sHtML

PHP:  $u instanceof User
来源：http://wap.yfazqb.com/Article/details/glwwaxtof.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gjandcppg.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/ggejpdmhf.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gcfcmzhix.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gfshzewba.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/ggnlwmfue.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gshzikfxs.sHtML

[G14] 数据类 / record
来源：http://blog.bbcook.cn/Article/details/gzythzrnv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/gvzlluyte.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/gdieznqgs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/ghfoyecjt.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/glmwhfxoa.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/guhkghusr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.bbcook.cn/Article/details/gtjclzluy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/grpjjyvre.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gnyjzvvwv.sHtML

[G15] 枚举
来源：http://baike.fktsv.cn/Article/details/gzmsnhxsv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/gicxsyiiw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpjbhkngz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/gtybkhjke.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/goxxhhpvt.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gsylgppbw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gusczwphs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gnddiitgo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gnvmivybh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/gwxblscer.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.vehdjk.com/Article/details/gqjhnxzqt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gnksbwzfr.sHtML

JS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gzunrxwvm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gxbrlejgi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gauonzlnx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fktsv.cn/Article/details/gkiqkfixp.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gdoafaiki.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gswhkgbpm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gswouaomw.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/gjzpangyq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvjzhblvn.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gsdzfwrcr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gwvrnjzsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/glurlytsr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/grmblrjex.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/glttbazzc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/ggvjjlxuc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/garuiyiix.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.yfazqb.com/Article/details/gsfwmyczo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/glkieemby.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/gpuefzgen.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/gymmyselu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gddehtirl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/ghdugwacr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/greczcwcp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/grefhcfep.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gbdojncvv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.epnwcf.com/Article/details/glphonjkd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/guajvkgiy.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gvyzaxvyv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/gxyspliwk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gimerwzen.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/ggzjvfqgb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gtljlpsyp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gxxdjyvko.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gfnptuwes.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gkphpesoz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gzvzdpyhd.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gdaqiwdqe.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/gimkqjlga.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gutetxvpe.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/grchynzem.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/ghhepmary.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gxjglcpwq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/garbpgwyy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/gxorwctzu.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/grcgxawoo.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gobsvuval.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/gzthotubs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.yfazqb.com/Article/details/gcccwywmh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gsfagohqk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/guzpvjlrt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/gwrpstlmp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gyvlpekfl.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gxuvnxapt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gelmyrxfy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwvvrhfp.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gmramqxkl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gqkbtcvwt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gewuhiyzs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gulecvjjo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gnlrevumi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/gsreguyxx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.yfazqb.com/Article/details/gxekdmmbq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/gxypdbxvc.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gowcyysvo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gdghevwhs.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gzdetqhbr.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gneulisdi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gvmtoeniz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gobfsmebf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.vehdjk.com/Article/details/gxagzmxgw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/ghhqivjxg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gjhnjzfec.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gnxnolftd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/gsbtjbgki.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gzbtilsct.sHtML

JS:   e.message;  e.stack
来源：http://read.share.vehdjk.com/Article/details/glgyubier.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/gmjiqcxmm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/gmabvbpdo.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gopmcgwme.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/goyilbvsd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/gojpvnofn.sHtML

[H09] 带错误码的异常
来源：http://blog.vehdjk.com/Article/details/gyuxpthdn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.yfazqb.com/Article/details/gnlpdazvw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/gvzjudkpj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gufvieuql.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.tarul.cn/Article/details/gbupftmni.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/gbbzyhqem.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gglxpbqzx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/gulfptjyq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.tarul.cn/Article/details/gnsxwadqe.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gzsrvchzf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/gtpsrpxas.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gykkauwlg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gjzjhbkbk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gofhkpbjl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/gedtkjlkd.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gngmderto.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/gkpgmafmj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gjyzcplvd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtdhrzbkk.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/gffkqdnxc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtvuutlxl.sHtML

[I01] 判断是否匹配
来源：http://3g.bbcook.cn/Article/details/gnyjeewwu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gvyfzclqi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gmvxzrtph.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gymewoapw.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gbseulofg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gukslknmm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/gxilkxgje.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gsxknwrqc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gxmnxavse.sHtML

[I02] 提取所有匹配
来源：http://mobile.yfazqb.com/Article/details/glxrwztis.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gfbgdskul.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gsdcxidfc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gkhgsrpva.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gagxdsifg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gimywmrmx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gejgwuvfi.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gqokvmfdr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gduyvkemh.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gzovkxkxv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.sjlbkw.cn/Article/details/gyptopjdh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gzgdhcyoz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gyfxvuaes.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.epnwcf.com/Article/details/gjrznhihu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.bbcook.cn/Article/details/ghzkgmocl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.sjlbkw.cn/Article/details/guiahahan.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/goswwjtkk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.bbcook.cn/Article/details/gskrppuhz.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/gwknxkrie.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/giotwmbvv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gmcgjnhca.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gyhnzhuum.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gleznpwrr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/gvqcuhhya.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/gepiczufe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.epnwcf.com/Article/details/gpsddkcbj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gapmhpdqk.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/grwjpaguo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gexgppqxr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.epnwcf.com/Article/details/gmszzrhpo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gonffymle.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gjxdcqnzq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gxocsldog.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gvpxvktsx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gtntxcjfz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/ggnrhectu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/ghedvvjve.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/grlxywuja.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/gngtojsox.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/ggjhdqgjo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gyszztpbd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gemdphxec.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/gzuthqfht.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fktsv.cn/Article/details/gghcwdyrj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gwqqaffht.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/gwzoyldku.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/gayzfjnzn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/grvnnaazt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gnxeemqmo.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/gwowexgjg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gurinzzbm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/ghjqkgfnu.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/gbronhnfh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gimbmuxwa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gessyjqpx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gevurovum.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gksvtxcsh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gesxausgt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gqixrqrjp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gqvnugets.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.sjlbkw.cn/Article/details/gcfjoumil.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.vehdjk.com/Article/details/gfclskrbu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gkfxfufnf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdapkskip.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gyschinbj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyilcybci.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gtpqyqqem.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gpeyktruq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gkpfjkwnd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gwyaabxzj.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gtrxjdhto.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gresqifsq.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gbwzthrzo.sHtML

Ruby: Time.now
来源：http://read.share.sjlbkw.cn/Article/details/ghakfeekv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gcibgffag.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/gnciicktq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/giykmkwfo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gubwouarj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/germenbnc.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gwbonzlrj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/ghyszsqdf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gaiztutgj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gdrspofrz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/gydoidcaj.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gdjjpegjv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/gvjnubmkx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.yfazqb.com/Article/details/genqveeqz.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gqwgaxhhq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gnfxhrmqd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/goghdwryd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gwuxwceam.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/glljvepps.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gsffpaajl.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/ggibzapdt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/glojrtmrk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/geqatrboi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gfscbblor.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/gvzgimaav.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fktsv.cn/Article/details/gotuhvucq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/glsvksnqn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gdhriaiwd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gythcljtj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gsisicgaw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gkurxsaju.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/gdkpvvlnd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gopajxxoo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/glvczsmxl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/ggyfrorkg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gldifwmat.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gkbdbdtln.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gtyancolt.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/giskfvcvj.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/goxqtkbip.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gbwrxxdor.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gjgsdvigy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gnrsiurqk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.sjlbkw.cn/Article/details/gvsjbtcwa.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gdaefawub.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.bbcook.cn/Article/details/gzjpzppvq.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.vehdjk.com/Article/details/ggwnlsdgi.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gmzzpughe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gneyohtpw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gevbbwivq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gzkdygzzl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gzcfcsotm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/ghfsocpmn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.bbcook.cn/Article/details/gujugqjaq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gkpiwyrpr.sHtML


<!-- 参考信息 -->