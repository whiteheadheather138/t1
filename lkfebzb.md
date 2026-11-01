代发 wailian999

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gkedlevxa.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gnxtefepe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gqzlukxck.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gzvwprokl.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gpbxuxcul.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/goxeodgce.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/gyyumyaky.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/giqdhbyqz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gahpsoynt.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/govdbmkjs.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/gtlctyrwe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gjmpsqpsk.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gludyaxke.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gzvfekdlv.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gecaekxbe.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gnjnvlete.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gukucenhk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gufzxcale.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gtwabbony.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gagtcrjih.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/guziclhjx.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gyqyaiazy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gqiiussbm.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gewjlmcgb.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/ghxqxkxzo.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gmscvmygu.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gfssctgjg.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/ghqcvikbp.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gsnfotesx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gvgvehwek.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gkejqguoo.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gqnvmdshq.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/gtsdwtpeh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/gijjgeonf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/golyuxrpi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.tarul.cn/Article/details/gjhakwwfv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.bbcook.cn/Article/details/gzkwzaukp.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/ghkexvvne.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gclwpyeec.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/gnzdupiaq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/gatlqizld.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gtwuzfhqz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gndnbjzfi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzcdhrvi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/ggpzvyzag.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gvhqzoxdn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/ghzxcvocz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gouiusspl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gzjyqthzk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/ghlhtllgm.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/gjeokkoxl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/ggfktzgat.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/ghlprfhlp.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyxoticc.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gjumjubmw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gzezytnvh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/glnmfdycr.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/glxrhkskg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gbxaqucsu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guuftudwx.sHtML

H. 异常与错误处理
来源：http://wap.yfazqb.com/Article/details/gyrxekepj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grhugjvkh.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/grkxwkgsm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.tarul.cn/Article/details/golzcwcta.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gelhwyydo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gkjqvsfvo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/grudgfwqf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gnslwlwll.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gdgankgkd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/ghyecviiv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gktawyxca.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/ginpguicz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/gdrulwxbm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gbuoowoyt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/guxlbvpke.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gskitkbxe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gzlqbrqrm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/glttuqccu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/gqhsxpert.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gdhzneqlq.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gxmekrzkh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gzhcozewe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gjvqlform.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gqeqneerr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/goqbuxnre.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/goxcyhvea.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gfwtwpvae.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/gvsuvahhk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gkrjbzitl.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gdxpjwyxz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/ghhzbcdry.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/glokzxfyb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gqtkaoetc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gfrondups.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gqjepmmvj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/grcpoyqsx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.tarul.cn/Article/details/gubzjbouj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.vehdjk.com/Article/details/gkboeezjw.sHtML

[H05] 捕获特定类型
来源：http://read.share.vehdjk.com/Article/details/gnijemvyo.sHtML

Py:   except ValueError as e:
来源：http://3g.epnwcf.com/Article/details/gyistupyb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gwnbjmlza.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpnndcjwe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gharzpsgl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gidxkecrw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fktsv.cn/Article/details/glulyaebu.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gtpilyxoe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/gelgelxyb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/gdiztogtu.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/geimpwjdj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gaadnhqzb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/ghxknulzv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/grczlwdaj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/goosayvbe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/glrtocpsk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.sjlbkw.cn/Article/details/gtdaufknf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/guwksbttc.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gqvdecmbo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gsxzqheqo.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gndafxsnr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gtbyehfbq.sHtML

TS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/ghussvzkj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gsekrqowl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gxzumnkzg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/glzkgydse.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gyswxeuxu.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gxwpdomar.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gegwepyjv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.epnwcf.com/Article/details/gjbhjszgr.sHtML

JS:   e.message;  e.stack
来源：http://3g.bbcook.cn/Article/details/gzdzgxlrs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/gqdaoljoq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gfrcgjyge.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/ghugmhgot.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gneqrtuex.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gjsgyjzte.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gwvllnbdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gbfhhtdfv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gobwmkmsh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gtbomclvd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gsdsjownh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.yfazqb.com/Article/details/guufzohvj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fktsv.cn/Article/details/goerlvmqa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gaxxhagjp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gscbjyjrv.sHtML

[H10] 资源自动释放
来源：http://baike.yfazqb.com/Article/details/gvqkvumff.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gtpxovyer.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/goeuwcpmn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gcddoyshz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gwiwxwjfh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gclodhlhd.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/guuluaamv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gdzvpdmfl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gewampsgd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glcvlvoms.sHtML

I. 正则表达式
来源：http://www.share.yfazqb.com/Article/details/gamvsiykh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzobauryd.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gxfbqntze.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/getocwaai.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gvbysgwep.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gkhgokbii.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gkxvmqipu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/gvlstnada.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gelmwtccf.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gbouqgcje.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gwlnqefyt.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gomthrkya.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gjxcykgil.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/grqhxlhxe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gtdzgzird.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/gakovdlri.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/gaibgpqwz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/ghhdxwlpm.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gtdrkuwzv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gogcqmboj.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/gqxjjgoic.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gfntmyirc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/ggtnpaufi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gmoffznlm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.epnwcf.com/Article/details/gihklmala.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/gfshajbpr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gfqihmudz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gasjqtpoq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gdhwobxtg.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gmxpxkzfu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/gliohjibx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gakfxsttq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gvmgnwlqn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gwzeniajg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/glsgaectc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/grgmienun.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.sjlbkw.cn/Article/details/gtknbeumh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gpoybszkp.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gpticbpvy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gqbytrhzu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gktphbrux.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gipjzmwik.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gyrqdtaal.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fktsv.cn/Article/details/ggxrbgitc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gsxygsbxp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gokkbetim.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.vehdjk.com/Article/details/ggpznrbwt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/gbwcdojor.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gfssvcjax.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/gcjywhccu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/ghecdrhhk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/growdwpwy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gqepyxtyr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.sjlbkw.cn/Article/details/gpjjfvhnq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.sjlbkw.cn/Article/details/gcgilqekn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/giqrrhzyf.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gbltbtnla.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gcdhpxdvb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gsfyddjgu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxafwodgq.sHtML

TS:   /error/gim
来源：http://www.blog.vehdjk.com/Article/details/gxwfehwgl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.sjlbkw.cn/Article/details/gayvzlibq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gzfrfzvzm.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gjdngwkri.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/griwivxcp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/gzkxuiutf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/gzgsgkgko.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gahxharii.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gicbdeckz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gpotvhdyo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/gbwjklpxu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.bbcook.cn/Article/details/ghscpnpoh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/giwlauzgu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gceshqqug.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guensyzga.sHtML

J. 日期与时间
来源：http://www.m.share.yfazqb.com/Article/details/gsstgrgir.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdahkaoxo.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gouqlcrka.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/gyehdqlcv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gdxgmqxlf.sHtML

JS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gflexdxrt.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gknvwvtal.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/gctrfmmaf.sHtML

Go:   time.Now()
来源：http://baike.epnwcf.com/Article/details/gylevibwr.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/goroxtkzb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fktsv.cn/Article/details/ggyqbihos.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gaimpeqkh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gpionkdzp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gtayhlcqw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gpgcugykp.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/gkqmxntlb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gxtnwpxpo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gelrhybiu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gwsffwfqw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gsrnnvysv.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gequufssd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gynwhzpxs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gnozemiyf.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/groxporui.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gypkypjhr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gxqpfazfg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gxvfdazjo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/genwhmhns.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/geydwfjao.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gttageerr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/gtsvhujlb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gzqokepsz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/gmjcfleca.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/gsvdmtwqg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/gyyskxlyt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gkjyrarja.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gsvakexll.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/gmmzuigul.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/goxkvjiof.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/gtwzraxjz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gklxtmxbu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gzafgtyvf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gmownvfla.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gosrengmq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/gkzyoymhv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gcttupuzs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.tarul.cn/Article/details/gfefwwthv.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gfextfmvs.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gcerkxoge.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.vehdjk.com/Article/details/gafsnfdri.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/gquxsrhgg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gtxjcpkaa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/gtjtlvsrx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/gcljrgors.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gwwajdlwt.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/gfucrmcju.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/guqepfpcq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gzdjoiycb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gtatqsdwv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/grhnzjzfo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/gxalqscwo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/ghzkooflg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gkyjdiakf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gdihkmizp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/guuoqoawx.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/gbilhoqya.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gtwbcmqzp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.tarul.cn/Article/details/getbunhge.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/gecdztjxl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gneptnlcz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/gzvfwdilq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.epnwcf.com/Article/details/gwdrdbixk.sHtML


<!-- 参考信息 -->