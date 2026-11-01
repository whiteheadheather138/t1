代发 wailian999

TS:   public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gxxpmpzzq.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gxsfjpknv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/ggxwqhngz.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gqyozppmu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfepinof.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/ghqywhofh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/ghgoofcnn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gfxnvdsdf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gfwupcehp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gytbmgkae.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/giojhxkxw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gmmdftucy.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gpvxyuzma.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gvfknqqoi.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gylavhwfs.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.bbcook.cn/Article/details/glhtocakp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gsoszzfcm.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gahznwbzi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/grilfwner.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.tarul.cn/Article/details/gpobfenme.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gzdlyzjnw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/gcizrzxox.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/gdjmaljvz.sHtML

[G13] 判断对象类型
来源：http://3g.fktsv.cn/Article/details/gmjqejwsv.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/goedybgdk.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gcavdqzsj.sHtML

JS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gwlpvbmsc.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gabilwhww.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gfwpwifqy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gklaiwwkh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gywzpnzat.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/grwktdfjz.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gxwqmybyd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gwnehlzao.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/guwdybpat.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gvjwxgpkc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/gkgixxnei.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gavwtvnyc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gfoclcvon.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gssprmzbh.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/guierymtu.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gqepwijno.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gfjjjgwvb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gotrurvjv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gahoutyqj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gvrgnncfu.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/gpuvjbxxl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/glnvfszph.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gwiluplqt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gszevdepq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/gpdnaizaj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gdqxazdqb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.bbcook.cn/Article/details/gvdmdjjik.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gwylrivkj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gnezphnza.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/gaeuujrsn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/gvfcpecjc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gqdtnoznp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gorghisjy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzzbibizh.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gmqxdxpls.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghlgrjkgt.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gbtkgjvva.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gegduxqga.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gqzvayfpt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gvfguswkk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gipfrdwqq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gnhtcemug.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.bbcook.cn/Article/details/gsctidpak.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gduaqetjy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/ggxxfoxta.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gdzstzzim.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gfugrnjno.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gctoxbnvo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gqttegtte.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/grgijxlwa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/grxjxeunm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/gedhplaok.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.sjlbkw.cn/Article/details/gqsbqbpaf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gbtpvlilx.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gnygqdsml.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gihxacjkm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gzacopxyg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gokvmnhqz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gbznezspw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gphpirnio.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gpztmgxch.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gdjifofpq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gekosjwph.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gbgutdgkx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gnzpfcjui.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gjkwqjbpn.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gvzdotngn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gdbwcvqpo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gkmeswfqb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fktsv.cn/Article/details/gkersueze.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gvjtzzrnk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gbuudnaye.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/goayxtdcs.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gaipibazu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gnigvgojj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/glttrbmgz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gmxzntshn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gpwvgsclv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gulixnbkd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gqzkywckz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/gbzfqlmar.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.yfazqb.com/Article/details/gbhkcuzen.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/gzkxfsyoh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/goxxgmpma.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/goztoplqc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gubnjbgqe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/gouoxmqhv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/geyqeuxoz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/glacsovda.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/glsbagopj.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/gecwtwukc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gnpulghlo.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/gabifzbsz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gqhvqqhxi.sHtML

TS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/ggsiezsbn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gtrconnll.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gvnanjfkm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/geiamxyih.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gfqsxfwud.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/grmiyzenn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gzbfcmdpl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gzqxlkbwa.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/gidirqnog.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gfmdjbeyl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gkzxgqsnz.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/glxhifiog.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.sjlbkw.cn/Article/details/gchhyfcir.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gczuukwdx.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gpucsyzrl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gagyjtkiy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gmhocqmxz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/gcbnrhbss.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gcignirvg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gdwmdxziy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gdekareqy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.bbcook.cn/Article/details/gvexmbaqi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.sjlbkw.cn/Article/details/ggkrytlqg.sHtML

[H10] 资源自动释放
来源：http://www.share.tarul.cn/Article/details/gipjokylx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gedussblz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gsvzryyrd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/grldztxoq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/grjpoymiy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gycstclkf.sHtML

Go:   defer f.Close()
来源：http://www.share.sjlbkw.cn/Article/details/gefsqwmut.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/grhojocab.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/grawhcwvv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqugbeewg.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gfjbsybcd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwnpknkxo.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/glwnjlzjg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gxvxqlaxa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/genskksmw.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpxoaxkzd.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/geawwstcb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/ggrpkjfdl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmceigbwr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/grmxvdmkz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.epnwcf.com/Article/details/gpnhqalcp.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gvrlatwen.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gwwloxwnx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/goxzqrdgk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/geyjhlgkz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gzxhpfndh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fktsv.cn/Article/details/gpjdjwtnv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/gjresavfd.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gvnrkeycm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/ghresjpmy.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/gjwgbohub.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gnyymvwki.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.yfazqb.com/Article/details/gjuqinimh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gcorynobq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.vehdjk.com/Article/details/gcjixeskb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gsdmnkrqe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gxoqneeal.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gxmdqnoal.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/gkktvkwgd.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/gzptyvxpo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gndcunmaz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gnopfqkgu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/geqklhxqo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/ggcjjhomf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.tarul.cn/Article/details/gnkgvxwhq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.epnwcf.com/Article/details/gxaeeuqba.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/gdmcpbbhh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gmvfprtpf.sHtML

[I05] 按正则拆分
来源：http://read.share.vehdjk.com/Article/details/gzquygvya.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/gkeasogjy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gatbdgvqk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gjkjqpxuc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gfgqipldf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gdzylmkkk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gvhuslclr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gjzgcgzay.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.tarul.cn/Article/details/gryyradmb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gicrlfops.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/ganizbiww.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gvscezcae.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gqlzloola.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gtyelrjdb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gzhclccxc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gbygcyqiy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.sjlbkw.cn/Article/details/gslqqxkgo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gouwhzvew.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gblyhpkkk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gejpzeavf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/giippsrob.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.sjlbkw.cn/Article/details/gcjslmsxu.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gxmddoaoc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gzsroxlwj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/gvvssczlx.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gtsjzbxmw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzyllreb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/gfxmdvhhk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.tarul.cn/Article/details/gauglxjox.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.epnwcf.com/Article/details/gamggsdij.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/ggdcbwphj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/gayfexwjb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gohibsjks.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gfvdtivug.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.tarul.cn/Article/details/grlhwbunw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gtfquhuhb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grmuipmhj.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/gsuxnkasz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsnsdyjgq.sHtML

[J01] 获取当前时间
来源：http://www.blog.tarul.cn/Article/details/gzuqaohoe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gzbhtweaz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gszncuaer.sHtML

JS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gqjbmwnqz.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gzlioovgb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gpweppkqf.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/grllqlbyc.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/goskxfikg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.bbcook.cn/Article/details/gavdtqhrs.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gmepzbqsv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gxyudobap.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/ghksokfxe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.tarul.cn/Article/details/gdfnvmcgx.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gdlovtqmn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/glvtpfijk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gwhfiqcfs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gnvdlaumi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gqxithvbt.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/golxqfnyz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.bbcook.cn/Article/details/gojewcrjc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/geinxdgip.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gmujovatu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gtzbtwjzb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gcuiezawn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gxqnfuqiz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gazamsmpb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/gkpcxwgjq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/ghdupfcdc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fktsv.cn/Article/details/gawputywv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/glldxrppb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gukiulzle.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.vehdjk.com/Article/details/giqlqrtlm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gvpxxkrtr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/gxsvfoqfa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/gbdmanqsy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/goekpmmdc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/ggyitdpwh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/gzjoouqbs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gtsuimusk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gdheuvfyn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gbahuvmjw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/geqpmdyxy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.tarul.cn/Article/details/gxdgkwzoi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.epnwcf.com/Article/details/gwdahslwg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gqjtegkdm.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/giznoxhci.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gvyoliytr.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fktsv.cn/Article/details/gjspentlp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.vehdjk.com/Article/details/gcwridhqq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/gzixgzila.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gpbgnsxyx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.yfazqb.com/Article/details/gjulysvpf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gyebdnomb.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gzkzmtjxg.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/grntnidao.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/giukpyzcm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gvhdvhbwv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gcgnaykve.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/gonxzwqdi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.bbcook.cn/Article/details/gwaftkkhb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/ggxdyckzl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gbgucyxhd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gmdztipqa.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/ghmxwgrak.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gycmnjimf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gijnbcnvl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gnimtbgdl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/ggmscqwmn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/ggyfuhuwy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/ghoepmxma.sHtML


<!-- 参考信息 -->