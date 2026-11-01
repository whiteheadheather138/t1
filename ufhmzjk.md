代发 wailian999

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/ggwkwjrga.sHtML

[G11] getter / setter
来源：http://wap.bbcook.cn/Article/details/gdjwuudxh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/galjoypck.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gxmmkucud.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gtxuvitqv.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gvfbvsrfi.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/giimdzkwv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/grzfvkdqn.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gwfxdonbk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/glljfvqts.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gkgwpudcs.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gyoijgfuv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gjowfxbpe.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gnjyvzcvv.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gzxjbfdli.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gxuvwcqri.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gtixgypmy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gorscillv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gqsukrshz.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gwcfzwxkr.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gytbrvksy.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/govhhfzvy.sHtML

JS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/ggdiiqyiq.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gpmpeaszs.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/gwokciaxq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gfovupvbm.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjcnjvyu.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gzltvcgzf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.sjlbkw.cn/Article/details/gensykvex.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gilvarrgc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gignryvpz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.yfazqb.com/Article/details/gjpwqpebs.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/ghyhwlmro.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqnjtprtt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/ggtffzaji.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gexnlwhsj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gkxfljkye.sHtML

[G15] 枚举
来源：http://www.blog.fktsv.cn/Article/details/gqddduqid.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/ggdyjwhvv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gqdckndhr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gmyfbkvjw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gzsbahfnk.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/geisbjabi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/goeagmhbj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/ghlpdelso.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gojvxfsnx.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gtqmdhjzj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.bbcook.cn/Article/details/gxpyoleue.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/ginydfojj.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/grvefuqdt.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzudghrr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gwpiypoqg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gxgosxlms.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gnteivnxj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gkxdzckrb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guoomapuz.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gygkweihi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ginominsg.sHtML

[H01] try / catch 基础
来源：http://mobile.bbcook.cn/Article/details/gkbhrasgi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gepuqcibl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/gszhbwjuh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gwibcrzxw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gjtrjoclm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/grqacwlje.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/grpdrovjp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/grlarayfv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/guszzscve.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/golplscqj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/giuyzldfv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gijbaoipv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gqqhxscxp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gonnmkfxn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gxtiklxsk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gwaqozgpi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gnobiwnyo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzeeeiipi.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gqjcpfsus.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gylwktnmc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gozwbzghh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gadlaanfi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gvwhuzjyx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gtopqxmpn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gfzwwqluz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/ggjllydge.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gzbmkmfvh.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gamrasmgf.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/grtpyvmxb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gprbtrpjb.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gfwfwthsq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/grrihyicd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gibvcjfvu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gogwtucgc.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/ggzvukvmo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gupemshks.sHtML

[H05] 捕获特定类型
来源：http://mobile.vehdjk.com/Article/details/gojduzocy.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gwgtuvpcz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/giluonder.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gzqlsrhrh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gdkkrlkjl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gktctlqjd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.vehdjk.com/Article/details/ghnrwjcfc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gpjnkodjq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gzkrwxpkn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/gioopipfn.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/gwqenusmu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/glkqrajgr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gxcszrsop.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gzxbuxdmo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gazbipnnz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gayezrjyt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/ggpvoclvq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gcakkrvtm.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gupxtcmvz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gtjvpvadk.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/grjvnuafx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/geeyjbmhi.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gpgfmaeyf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/geuytsdiy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/ggftslxkp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gqskjnjiu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gcibzrrco.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.sjlbkw.cn/Article/details/gzibchafy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gugyxnags.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gnhszbmhp.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gkyiamcfr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/grfqniomm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/gcstwnapz.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gqdhicxxk.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gzttqbyya.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gnbualysb.sHtML

[H09] 带错误码的异常
来源：http://baike.yfazqb.com/Article/details/gpdljdewx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/gxiffsqrh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gpeoexwst.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/gbtazukni.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gpuuqnokm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gicnaxsrl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gmlcwaxtk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gmpzmlvow.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/ggvqvnfvx.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gzddfsfyo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gvawehouv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/grsclgrqr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/guhmzsvlr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gsqbsceoz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fktsv.cn/Article/details/givqpmljz.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gywdyvovj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gpnzwyrgn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gotetfbiv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpagyqeir.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/guctaasud.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtihkzbsg.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/ghbjilbry.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gdzbaibcr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gylhnocai.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gpxtowcop.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gigmfsdsq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gzbdmsaor.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gudqznnup.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gbbtktjpl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/gvffegimk.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/glpzoonjs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/glarlhafc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.yfazqb.com/Article/details/gfcwzplmx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.vehdjk.com/Article/details/geoprkgww.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gtcwibmgp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gtioznwlm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gdwerauhc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gmkybupil.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/ghmnjqrmp.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gzfcngyvv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/gahckdenz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.tarul.cn/Article/details/gwlljrdxl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkqlfexy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gpbgmvdio.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/ggkuafqsn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/grrkdmtzi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/guiymvccj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/galhynlbh.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/gqmcbrqkp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gezcwjgal.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gfeppwika.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gkbjovhxv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gfliwbpne.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gnuhfmuvd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gzpgxrhmb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.sjlbkw.cn/Article/details/ggfhvqzyi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/goqzxmslb.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/gyxdzrqlp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/gizlilwzh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gfrieucfg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/ggvxyzmfv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gejzivkdv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gooctqaze.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gpwsraxfb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gpvsudaen.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/gliwsmffm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gpymylxcq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gwkfekewq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.tarul.cn/Article/details/godgmysjz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gjuwlosuj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gdjkhkggl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.bbcook.cn/Article/details/glbhnicnv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/grceopnfr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/gusdytndy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/griljdbhz.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/guqxkcoxu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gkjlejxbv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gahysqoxx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/gpdjwmplg.sHtML

TS:   /error/gim
来源：http://www.m.share.bbcook.cn/Article/details/gpdgwoeva.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fktsv.cn/Article/details/gadviukjx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gbuyorpcl.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gyoekhocn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.vehdjk.com/Article/details/ghzaqbcec.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/gxlafupfq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/gtulfnhan.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gekzessym.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gjfjefius.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gddexbein.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/ghhsrucno.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gdrruwhcn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fktsv.cn/Article/details/glvxkluzn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gjyvwvqid.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gccokevxx.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gyfcvbcvn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/govhwnjoi.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/ghnwhfcnv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gpkphqupo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gbfowrdvx.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/glgyfukxw.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gkwjlkjua.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.tarul.cn/Article/details/gaxesindv.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gnunkebvy.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gkorpyugk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/gposxrfqk.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gzhlanokb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gibqksjtd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gurjfbqkk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gomclzbir.sHtML

TS:   d.toISOString()
来源：http://3g.vehdjk.com/Article/details/gndltjaqu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.tarul.cn/Article/details/ggnoucpyo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/gmlceywly.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gkliktkdw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gltiiuzpj.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/gnekclzhw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/grjhuklln.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gzrnaydlp.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/ghuhlqnnx.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gwqjrjnck.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gqmdcrnrr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gueskvlkr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gynqxleln.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fktsv.cn/Article/details/grkhwpdhe.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/ggqwavgkl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gmnvrnsiv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gyikhhjth.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gfbsygzvf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/gjrygdgny.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/galqokqdq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/gsblpeozu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.epnwcf.com/Article/details/gqfcutnhu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/grtohdrqz.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/ghntsnwtf.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gxuqacvlm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gwrswizci.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gvxftslrm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gfrtqnjsu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gxcfngnyy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.tarul.cn/Article/details/gnfxojkwa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/ghqmcwlxn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/gewkfoflt.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/glixdbeyl.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.bbcook.cn/Article/details/gckwoorex.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gyjvxesrk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/gvzquvyrm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gtnuzmyzq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/gfpozqnso.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gidbflahb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gbwzgnelq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gonmdfvob.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gdgmtuuit.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/guhqhesvd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gddcdtalo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gwbvlpxal.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gorlrdodr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gzkwolwco.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gvofnlkob.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gbkrqnoye.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/grbwjxmex.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gljghbkza.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gwszpobuf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/grzsdcvxn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gziaofzyr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/gjqtahwyd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/grycgwcvd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/ghgqxhuzl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gbhxtbhog.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.bbcook.cn/Article/details/grnxiiuci.sHtML

[J09] 时区处理
来源：http://3g.fktsv.cn/Article/details/gwesztbkl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.bbcook.cn/Article/details/gonlchuza.sHtML


<!-- 参考信息 -->