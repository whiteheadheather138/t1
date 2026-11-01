代发 wailian999

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gdvhqoutt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gemaqpaeq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gzzyorpss.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gqjpnapvp.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/giljrotpx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gfhoahjyt.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gdlplxaaf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gjoeffzvs.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gtcucupnt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gezibpowg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gmzdeadjh.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gkaxlnaph.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gvyctgdiu.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gqqfihayu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gkouwrzin.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gpwgukibh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gmvyxtfpj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gsntpastr.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gudsndsxo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gjkupcdcx.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/gjtsdavqm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxlbwchdd.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gcaglppxo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gxjrpszhy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gjxmejtkh.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gnivcklcg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzmrkrzcr.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/grqspmjsn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gphvlsglz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gihkokegn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.bbcook.cn/Article/details/gfwhijuwn.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gqwhztwvj.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gcgkeixwd.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gwdcjfckv.sHtML

JS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gzebwremg.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gllvmvghp.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gykyxarow.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gywhgmrsz.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gqrwoivjj.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gjhqbbunq.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gdhuduotz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/ghlsnbkrw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/gyouxyduh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gaakmtyum.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gurmwyawx.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbdttuywm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/giakeymvs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.tarul.cn/Article/details/gzzjgmiqz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/grifkwbkr.sHtML

[G15] 枚举
来源：http://m.share.tarul.cn/Article/details/gkvtlnaww.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gyhzwyxru.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/goqbrzfev.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gztembepc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gtukloays.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gxpgovvgy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gowqtiuzn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gokwjeklb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/ggrwrpelp.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/govswhcgw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gtwwsnjyw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gtadyzuhr.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gxajlmjom.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gctbhnxac.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/ghywbkplh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gyulyaunq.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/goqmkwuza.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gfltcfgnh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsizcyrjg.sHtML

H. 异常与错误处理
来源：http://www.share.bbcook.cn/Article/details/gkhefaqus.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/goqbztgby.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/groxegmeq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gcjtrqziw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gbgznwbhd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gzmjchjep.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gpvvvchbt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/guvqxzcbl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gvgzrbmrg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/guerfypcz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.yfazqb.com/Article/details/gjxulaxns.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gbvvdrjeu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gkivencps.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gkqkvtopw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gbyqzdpnq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gtknoysnw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gyzfbglue.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gcyzogsjw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/grjapvhza.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gadpquqnp.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gvlgvbeyv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/ggzvdnvsg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gwkreprku.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gpylszdyv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gipcqzach.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gfvbbdzsn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gekeinfkq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/grftfiwbw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/giblfgscg.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gzkoxkswm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.sjlbkw.cn/Article/details/gnqwzntzx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gbmrszify.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gscpdepun.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/guvsettvs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjspnaoid.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gpshlekuz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.bbcook.cn/Article/details/gdmvtyqgk.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gmwldvppt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/gwmetjqme.sHtML

Py:   except ValueError as e:
来源：http://mobile.bbcook.cn/Article/details/gjfqfgzcu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/ggvmcbnwb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gxlbrfrrb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gxqtaxhms.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gzeqsqvbe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fktsv.cn/Article/details/ggwstcens.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gopbwtwdm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/gbcesesjm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gjupbrxer.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/ghffzivnf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/ggfwxaprx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gdhmvoaho.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gmcouzuwj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gbxhmteby.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/gfuhswwvz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/gsmokmezz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gxttvyzdd.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gydqdubed.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gfjglseqy.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gerrhmgbs.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gzvojpwxj.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gnxwfullv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/giiwuoqty.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gumfmravm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gotndpakl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gysgbvpfm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/gpiqxcpft.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gillowouu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gacxhwoyi.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/goikjxvbl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.bbcook.cn/Article/details/gyywibqxq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gbpuftmca.sHtML

Go:   err.Error()
来源：http://www.share.sjlbkw.cn/Article/details/gfwpckwxy.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gaepqefnk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gzewrigst.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gyycbhphe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gctwlpdwb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.vehdjk.com/Article/details/gtwptckzy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gyrxkcvot.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/gxgcrizxz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/giewowcud.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gcvahowwu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.yfazqb.com/Article/details/gfglyhcdq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gcmcmkicf.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gqxyoukzz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gfndwldzv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gfhezzrfr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/garpononx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gnsrumcjg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gpvxotkgr.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/ggsqvidtt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fktsv.cn/Article/details/gizwtpymn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gjxwslybw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyqvhuuki.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/gtuqfxqnc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvvvpcrwb.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gucykdgny.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gcybdrrqd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gvcftkaec.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/ggvbespab.sHtML

TS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gxemeglic.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/gpsnabozw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.bbcook.cn/Article/details/gdejqhfop.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gtaytobki.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gjicpjbfw.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcwazylo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gqgduzjso.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gkmsxhyqx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/guvddnolc.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.yfazqb.com/Article/details/gljzmnnbc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/gxwbbthww.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/getoizazz.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/ghkerlnum.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gqsvjqcpn.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gtrxwtegm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gswspdtmp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/geqkxpogj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gfxdzwwng.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/guvupvcfs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/gvkrnzxel.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gkhiqarju.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/gdoowotim.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gklqtltls.sHtML

[I04] 正则替换
来源：http://www.blog.tarul.cn/Article/details/ghhtfyrgp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/ggyjhyitk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gcnxeeglk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/girasaptj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gxtmtrvps.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gfcnumbiq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gceptoehz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gvlxrwyqy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gcljzhwde.sHtML

[I05] 按正则拆分
来源：http://mobile.bbcook.cn/Article/details/gfzvwhdwa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gksjsiaot.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gmhcmwdrx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gfyzztenk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gpspvumxz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gdklffpds.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gribmzplf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/grvwmlzfo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gypsmbkvn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fktsv.cn/Article/details/gtaqojard.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/goybdcakp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gxivzhlla.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gdkbqmlkc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gofifiain.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gmfdrjvho.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/gmyaopeka.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.sjlbkw.cn/Article/details/gzoolmwfj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/giuptremg.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gzcucbktv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gxiulmxxh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gkrrsnecv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.yfazqb.com/Article/details/gipsjsumq.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/glpbccqdy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/gpkjkvsow.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/gvoobampo.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.tarul.cn/Article/details/glnimyxno.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gduawxhqv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.sjlbkw.cn/Article/details/grvynobon.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gcixyrefm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gucobxxel.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/ghvbthsbv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gjduejhek.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/guqciysoc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gjedgpbiq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.epnwcf.com/Article/details/gcrkhzidn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gldnbdisd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdwdoaxmh.sHtML

J. 日期与时间
来源：http://read.share.tarul.cn/Article/details/grboflxhk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxbrnnrtn.sHtML

[J01] 获取当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgsyasre.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/ghnauyucr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gyuscksvb.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gwhwqbccd.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gmbptzlpm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gzckcrzgs.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gbgwnqcxi.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gztmztzzb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gyatrycez.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gvpfaadae.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/ghaitvxhj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gkayizybh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gkhojxcqs.sHtML

TS:   d.toISOString()
来源：http://3g.vehdjk.com/Article/details/geuhnxrbi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gflkmuexg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.yfazqb.com/Article/details/ghvmkphpz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gwcqxireu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gezmhumpq.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/goskryamo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.bbcook.cn/Article/details/gxrvvcxha.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fktsv.cn/Article/details/ghujsivwn.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gebikgttk.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gyqxzddxl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/ggonffsju.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gfjwunusc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gubjlzkyy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/gfzzqeuns.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gdgpjtjot.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/geoqwtvag.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.tarul.cn/Article/details/gmlpgnzoz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gcwjgfhqr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.tarul.cn/Article/details/gbhaezmkv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/ghwjvoapb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gtnmwboft.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/gptphnwrc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/glpewieta.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fktsv.cn/Article/details/ghvirnlmq.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gbtpsdtjd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/ghxflqnuv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/ggpwluksi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gmarwhtqt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gccqdvlvw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.bbcook.cn/Article/details/gdauhiiud.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gumpptlwd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gqynrbxle.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gdqbnjohe.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/ggiydrxrz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gnlttkjwv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.yfazqb.com/Article/details/gcftnozem.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/gphoofesz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gappcbbhp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.epnwcf.com/Article/details/gbhktohnl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.tarul.cn/Article/details/gllkypoll.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/goqrbbuvn.sHtML

[J07] 比较两个日期
来源：http://wap.bbcook.cn/Article/details/glcjeltsk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/grpnwdqby.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gpgcxqeer.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gcceftinx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gronnfkhk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/ghelzwopi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gamffpprp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gajnuzgwj.sHtML


<!-- 参考信息 -->