代发 wailian999

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/gsvppshws.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/gggjnexni.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/geqgphzol.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/geiesiqws.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gtkxbzzeh.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gfcmngjdd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gulmygygs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gbtcfesys.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gphqnxesv.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gjmpvdvac.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/ggirceieo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gqyeerfny.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gmrpdyexe.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gabwgndcm.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/gqrrzlujk.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/giqyrhuhe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gjrzorazx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gjaedfptu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gtoqybhqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gxtuttnou.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gaqauuftj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gewqzdeou.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gfvnquhcd.sHtML

[G13] 判断对象类型
来源：http://wap.epnwcf.com/Article/details/gwkogmmqt.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/geykvjhbg.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gptmzcdip.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gnpzbdtww.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/girdbkuzt.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/ggdsdaqev.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fktsv.cn/Article/details/gjndbtxta.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gfuorrlbj.sHtML

C#:   u is User
来源：http://m.share.fktsv.cn/Article/details/gdpwjqrmp.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gmverflxn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gdaddmzms.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/ghmxaqbjj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gzmqmmzfn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.bbcook.cn/Article/details/gnuuvhmhu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/girppogjy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/geeqvtvuq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gpmffegdi.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gzgrmturi.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gxpyrvzuf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/gbmqgvzqk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gbbmughti.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.epnwcf.com/Article/details/gwpxxqlih.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gvkxpjwwq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.tarul.cn/Article/details/gvkapukar.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gnblnedob.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gkxvrllpt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gzwvzutiq.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/gxcufonll.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/garlrbqfr.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gelowlpwl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gaxyculaz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/grnhzlxoq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fktsv.cn/Article/details/gliiqafzr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gpybrqndm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gjjzzgyqk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gcchxflbj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvrqfxkgb.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gtttlfxdp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gicwszfca.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gbsggcbbc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/gphljnucd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.yfazqb.com/Article/details/ghtvujjev.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gehfzsfol.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/ggsmpkmrk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gfjeeixql.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsuqqish.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gfpbftdmj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gnycaadwj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gdwcfiayw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gshwkuoac.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/guwputubv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/glrzdvtxx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gwtwqbhsn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gbyicuqkm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gjalvrhjl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/grebgjnrt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gfgyhvkao.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gmciihchl.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.epnwcf.com/Article/details/gdlxkqzyg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/guekmeyfv.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gijgkdtua.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gaaihydgj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gyafjfwsp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gumtsdjbj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gdfarbsgn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gtpvlcjnr.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gevbefcvn.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gazvbuevl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/grfpkotcj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gllmtypqk.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gijtlfbno.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gxcujtgya.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gwsjsowqj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/gdjlnsyuv.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/gyweagjbq.sHtML

[H05] 捕获特定类型
来源：http://mobile.sjlbkw.cn/Article/details/gqaaolimd.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gigbmyzjl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gncbulqxi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gkddeqihk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/ghljvnzbe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/gpdonnrvv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gbpfbqgry.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/ghstakrol.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/grcqqpzhz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.bbcook.cn/Article/details/gjxsptrqs.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gaxikdtnp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gdbboqclx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gqgrqjmfk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gtvegttqs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/gjljhghbn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/gaqlcuauu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gzqzrasdb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gpwtspfdn.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gkgaipsmt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/gkaiylxkb.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gkciplwtc.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gllsoovfz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gulqmvyio.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gsjsniqfl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/gmghnjbov.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.vehdjk.com/Article/details/gjgecxjrh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gdwpbogxi.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gblfrcdtq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gvyxujrpl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/gcnaydgwi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjpxmuvb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.sjlbkw.cn/Article/details/gjtqfurge.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/gcivlgcvw.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/gessutosp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.sjlbkw.cn/Article/details/gurlcoejq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gjcambxiq.sHtML

[H09] 带错误码的异常
来源：http://www.share.fktsv.cn/Article/details/gahhfbvgp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/gxtdawakb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gnhgrnlcz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/gaezjrbfj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/gqzdmzeug.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.tarul.cn/Article/details/gdsifwude.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/garphlpti.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/gcbrriqow.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/gctnvajhk.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gojmfirbb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gcnzmlvqa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/ggksxfpnm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gyddveogf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gwhsyscoh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.vehdjk.com/Article/details/gndqdubqr.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gaoowpbni.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gdnfzngbb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gzslcbevb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkcricqux.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gzkbdgqdl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvjxeozrk.sHtML

[I01] 判断是否匹配
来源：http://wap.tarul.cn/Article/details/gvhwfrbrn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/geabrrlxg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gjptwztoe.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gtledzpbe.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/ghiehsezn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.tarul.cn/Article/details/golupkygw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.bbcook.cn/Article/details/gyhgazjvt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gbslffyoj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gnmshnkbf.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gcsqfnkmk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gdzxmuyww.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gehejrjcq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.yfazqb.com/Article/details/gqxphdguz.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.tarul.cn/Article/details/gsbhatwrm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gfhxqpawh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gozdarmqd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gubwcegbr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/gbopndzjc.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/ggpvvshqh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gkpsqgwmf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/glmaoezeo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.epnwcf.com/Article/details/gshyftkbf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/glfpvwiyl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/giemltftd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/gfpdgcoqb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gdflddmmd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gvhbhskqg.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/glfowaxlu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fktsv.cn/Article/details/gcxsekzeh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gcsvwpeqw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gdgzuglwt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gsoipkhoc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdavvimwi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/gunacjcip.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gixrgpcsf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gmbcwnpco.sHtML

[I05] 按正则拆分
来源：http://read.share.epnwcf.com/Article/details/gnvmxrezh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/gvrshmmst.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/ghktlbecs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gizktvttn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gukgxrjhi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/ggaumwjvp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gcuoqjmsd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gcbghudzm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/graizancm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gemjbemle.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gxsxspjzs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.sjlbkw.cn/Article/details/grltncyzb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/ghpsnvflp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gdkpsxsmy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/geosuqmiu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gotwvcqmc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.tarul.cn/Article/details/gsaurglfz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gtjolorye.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.bbcook.cn/Article/details/gybfgynfb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.bbcook.cn/Article/details/gtpzffzku.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gswasjkqi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/gdidgvdni.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gbxxzwegb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.vehdjk.com/Article/details/ggfvtxhia.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fktsv.cn/Article/details/gpzdrarcq.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gosiiyyrf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gnpfvfcot.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/giirohudd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gqlxusgev.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gzpiehuep.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gkodxtjfe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gbmengbzc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gcqwvyzlb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.sjlbkw.cn/Article/details/ghbuwgzgp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fktsv.cn/Article/details/grckzelau.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/ggiehvvka.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfrrsujf.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gdwsiclrl.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/giolbcisq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gvrbkblxs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/geauavgta.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/greuvvejm.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gshijonvc.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gtgyshuka.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fktsv.cn/Article/details/gsajhxpfn.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/gqyxvlson.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/geeqgbyjk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gtfyqgidn.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gjqgclpsn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gwarktbwb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gfcvzrdlq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.bbcook.cn/Article/details/gzyazlsie.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gahplwtrn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fktsv.cn/Article/details/gxaqrodbe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gjisqivgn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gijcvxjrr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gsvwcmkng.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gpvyqizzh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/gwmvhlncf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gtlbmxpth.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/ggmwfsymx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gfrdzhghb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gxscjbxgn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gtpekvuee.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/ggrvvakho.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/glilwvxxq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gnazsuouc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/ggpviheak.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gdumirsbz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.tarul.cn/Article/details/gwcfpibjf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.yfazqb.com/Article/details/gmocsftfn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gepywesjn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/gaqfcwreh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.yfazqb.com/Article/details/gxshefnjo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/glulsquam.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/gbeggyckp.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/gsyiwbusr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gxaadgoaz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gjtnqpwuk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gambtdikq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gzbixwkrk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/gqsruxijw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gpkyjvqmb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gfjuzhbyg.sHtML

[J06] 计算两时间之差
来源：http://3g.epnwcf.com/Article/details/gcrqfteev.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/gxuvlihcg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/gmqsqfdfy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.epnwcf.com/Article/details/grcpngsqp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gdowkskdk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.tarul.cn/Article/details/gpfnispvr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gwrnihnna.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/gekhzkjyh.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/gggjkzhcq.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/gbmuysqxy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gihllecco.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/gfrefdoev.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gkzmiiyhr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gtjnmeujd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gittqwkak.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.epnwcf.com/Article/details/gevpzxcjh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gcmatuuxx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gqibjhfwv.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gadvpgbpi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/grmfupokr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.vehdjk.com/Article/details/gbcfjpnni.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gclrvsslm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gmsmmvpul.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gznvpwako.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/grrhikubu.sHtML


<!-- 参考信息 -->