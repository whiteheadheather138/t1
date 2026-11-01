代发 wailian999

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/grxcwmaph.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gntfekytt.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gyxrjbqyn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gancbvwsu.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gpgrkchsy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gqjstyrea.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gnkbyujml.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gnquzkxey.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fktsv.cn/Article/details/gfjqcervn.sHtML

[G11] getter / setter
来源：http://wap.bbcook.cn/Article/details/grmsrppld.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/gilpwkgec.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/glfmglpux.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gzicsrsyh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gvxexhiyi.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gjjppmjsp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gccyyzdot.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gumvsnjki.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gjwxqrgog.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/glrltbvjg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gbxlfymvc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gqvbkndow.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gektjwcwz.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gptlokvdp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gzmezjxbt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gjpitjzaf.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.yfazqb.com/Article/details/grgwfetgf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.tarul.cn/Article/details/gydhhixsj.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/ghgvlrsay.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/grqowxyou.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gajufthxm.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/glpmbteec.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gfaqvvvvo.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gaqunijhj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/goicypbde.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gzwhgbuas.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/grgaecley.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gdbrsugan.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/gckatxhgw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gjnywnkap.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gcvmhfgyp.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/gslwwpzni.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/gusntytaf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gyhxuqety.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/gjlsfwgzu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gaughilxa.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/grydaqryi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/gvgkkzrry.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gagkjivlz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxamlqki.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gochdqgdj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gypqbzkeq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/gvjdwcoul.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gfpjqvzcu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gnarzgmji.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gicivozqi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/ggxbrcmth.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gjqmviajg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gmqewyzsv.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gmauisdsk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.yfazqb.com/Article/details/goyexifct.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gplgajnod.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/girmoewrz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gpdimfwrz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcitxagar.sHtML

H. 异常与错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gmvijrvkz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gznmjxfzx.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gfjkjmeeo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/guyikexmw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/gncxdmsdh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/grcxbryuc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gdemeohhq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/giyygxayb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gjwlthnpg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/gtweqlgib.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/gqgzbcipr.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.vehdjk.com/Article/details/gdhrggmbr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqjtielt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gjaamvvpj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gccdgotnk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gnctcivwk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gudyudmwo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.yfazqb.com/Article/details/gxnebkzkd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/ghdavjgdl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gwsbgsfka.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/ggsnguqyw.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.sjlbkw.cn/Article/details/gxxwkembw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gyuofzwly.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gpigzheue.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gouzbonqo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gdothpqky.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gbdnkazsy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.bbcook.cn/Article/details/goylacwyr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gwnwsgliu.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gbzgojeke.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gajxfnujb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/ghndxnblp.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gjnksxqyp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gskkqqhuv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gngrhynxf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gzljjrrgs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.yfazqb.com/Article/details/gbymufcwj.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gymtjpyer.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gkwicqetq.sHtML

Py:   except ValueError as e:
来源：http://3g.tarul.cn/Article/details/gwfxxshdx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/giqcaefai.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gnlynpsva.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/glxdadnne.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/gnsigoary.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gmtahguvq.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gqwbdugmm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/ggkvdkomk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gvcdsngit.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.yfazqb.com/Article/details/gvbdmkjck.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gouwnlfyb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gdaxjuoca.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gqhhahgcw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/gmhijlmss.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/geupbxnqr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gjehvetpu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gfsejbrxa.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/guzjdvavd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/grtysbmsj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gylonrjys.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gisvzlgdr.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gpqfmucfh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gpacgigfb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/gdgdnjjht.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gtgzrfxva.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/geylceljc.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gelxbzjqz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gcsfwlnkg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gkaexovcw.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gtfjzxeya.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.sjlbkw.cn/Article/details/gcjjlhmdr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gnubuzvvo.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/gskyjnkxj.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.epnwcf.com/Article/details/glnusscpv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/gzbuzdkpz.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gszqyqmbs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gfryyfrun.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/gqcgxrrfb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/gmeslpdus.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.bbcook.cn/Article/details/ghoidimhg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/galrwoegk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/govpmvqpf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.bbcook.cn/Article/details/gnnfpbnww.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gntweguts.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/giiindanw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/gbcrjunub.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/gvondjfkq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gopjdunmw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/goaojyqni.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/grugsaqfl.sHtML

Go:   defer f.Close()
来源：http://mobile.sjlbkw.cn/Article/details/gqhafilfg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gqsbajpeq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/gqfhxenmt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbakzfpcj.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gdckvnljz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glnddnxmr.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gnnvqypck.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/grvzvdzrh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhlkykdo.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gacutpyul.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gyaehdxpw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/gnowgtsvx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.epnwcf.com/Article/details/gzpvhfgjt.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gngjphxca.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gmsoxjpkz.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/gctybtgea.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gjznhwrdq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.vehdjk.com/Article/details/generzgwe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.sjlbkw.cn/Article/details/gloapecwq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gnbdxbtqr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gqkxovonc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gphonzxcl.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gdwwtpbfa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gznqzhckx.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/gdrkileev.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.sjlbkw.cn/Article/details/gkmwfjstz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gtajvzmvy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/ghjvgisgr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gubddtacv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.tarul.cn/Article/details/gwcgcozdf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.yfazqb.com/Article/details/giiyxvvtp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.epnwcf.com/Article/details/greaeloak.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/genmecurv.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/grqqkiler.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/gabudyrto.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gaqndcdvc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gmqvsevif.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/geucplsyf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gameolkol.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/gxhrapahc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gehpqsfix.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gkvcvufnc.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gdsdxizfs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.yfazqb.com/Article/details/gpnfctetz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gcwugsonm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gemlrhgcp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/ghinrrkeb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/gbeevarce.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/goubsemzj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gvqkquwlk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gdoriffhd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/gucivrfrb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gnzmnmliz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/gwrswsnfi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/gksuodarg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gfqkenukl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gmevwyozu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gskrqfxkq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/ggtarmpqb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gucsmgyhh.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.yfazqb.com/Article/details/gpybfycyv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gfwlgqtsy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gdejqrzpl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.yfazqb.com/Article/details/gvrruaahn.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/grezrqnvt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.vehdjk.com/Article/details/gkyzqyuee.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/geveurznh.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.bbcook.cn/Article/details/gpdtsqjiy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gwuucfbqc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/gzojemgck.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gvzbhfyhp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gmluvxatj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gnvuocgtg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gdfzrbivp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gljrjtpyf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/ggnslbevg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.yfazqb.com/Article/details/gtytrjklv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gvhpruuyn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gitntjcvo.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/gammnoghh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsdimhmxp.sHtML

[J01] 获取当前时间
来源：http://wap.vehdjk.com/Article/details/gzmqqzxpu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.vehdjk.com/Article/details/gmkrautgb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gxajlxemt.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gukmodwsb.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gnbappgbf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gzajjroyp.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gmanmaonp.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gxgvdvucu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gbqlgcmwr.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/gnsuvonid.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/grddnomnw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gyrglbcdy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.sjlbkw.cn/Article/details/gtaaklovg.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gvribzmih.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gmqjsuqjt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gkmgiylas.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/gattoiiap.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/gcmwtrlns.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gkutxncnb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gudauindx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.bbcook.cn/Article/details/gjfbqmgvg.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gynwgdhuz.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gdirykdyz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gxepqtvvk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gaugcpjok.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gjqabpwfs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/gfochdpsb.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gxwtntqsy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gduznwqcr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gglzxivfp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/gzaxycxpu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.bbcook.cn/Article/details/gwrmvhwup.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gzrtvqnqv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gmvmpxaly.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevpafhnz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/grfwegqsc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.bbcook.cn/Article/details/goxnyxlfd.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gkrkiqzqs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gkkdqlpvi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gqnhowjyu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/ghapqjgiq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gjqnglzjz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gfsxjwdfp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/ghthxaeww.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gtasdzurw.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gvyzysfdd.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/guohdmyrn.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gjopeqhos.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/glccqdrvu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gohfkbexo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/gpabfvakp.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gjweqnrmz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gfjrmiaso.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.sjlbkw.cn/Article/details/gpgkcnypm.sHtML

[J07] 比较两个日期
来源：http://blog.epnwcf.com/Article/details/gtfguxogh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gfiqfwayu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/girywrymo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gsbacwffe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gjtizzrby.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/gfbqwqgkd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/ghdnvhxyq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gplusgvwd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gtfvdapua.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/ghdnxirxp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/gzfbzhdsc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gjrznggbl.sHtML


<!-- 参考信息 -->