代发 wailian999

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gmbsniwne.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gsgufdhhr.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gqsopvsuj.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/ggnjrdysd.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gjhshrjmp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.tarul.cn/Article/details/gjzgxobni.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/gemulhzse.sHtML

Ruby: public / protected / private
来源：http://read.share.vehdjk.com/Article/details/grrcvagse.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gthpkonpw.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gbiyleege.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gxyzewiug.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gjzxeixjb.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gimtvhbgl.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/glrbpnnhq.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gnztqytkf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gadymvruk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/gkexqaafa.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gntkpxhda.sHtML

[G12] 对象转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gtctmunzh.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/grjextovn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gfvakhqmu.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gtxcxehov.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gercgmbhc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gfdyqsoop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/ghmmuvfer.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/gorrtcybi.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/gwyjfrper.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/glzsnbngm.sHtML

Py:   isinstance(u, User)
来源：http://m.share.tarul.cn/Article/details/gupnvaexk.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gquavxjvz.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gbkqnyqtr.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gyqqvxgem.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/ghicsazav.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gmtnmbrad.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/gdpgakqzu.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/grhoisevz.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/guwupkvqx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gqucathcw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.tarul.cn/Article/details/gwkwukxao.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gyybcgexx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gswghrcbw.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/ghlhyiqlx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gbwqjwoux.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gyfmcuqsm.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gsxogxijd.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gzgtxxehl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gzwwxhiqd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gfmpppuxw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gbxboydoa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gtpdcdeyq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fktsv.cn/Article/details/gtigpystn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gvbnmmjoc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.vehdjk.com/Article/details/gncikrmzh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gzfgcwsmr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.yfazqb.com/Article/details/gpngwgfbo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.bbcook.cn/Article/details/gskjasbty.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gykjoujqg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gxwaqawxb.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gzhlymogo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gymnbiwvv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/grqargtfo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/ggjkqjjpr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/glhcfaytx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsqqcwlcj.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gjsrbcgcx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghvkdsxqv.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gdrywrzpr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gtosqykop.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gztpmxcdr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/glfzukrfo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gjnwoyxnz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gjwaqjilt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/gbttfucpg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gtleyxept.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gfkgfhchy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/goqqbipnj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gnxnogqvr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gudvvsksu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gztskenkk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gqawhpozr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/goewyktay.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gmzdvaoay.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gufgvejbv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gljpsgwjl.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gjvmkitel.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/geldgqtqk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gwfdoffmp.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/glbagbmxc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/ghzmycuqa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gsxsxeokt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gpterarpt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/gnxgttbuy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gmrzrrteq.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/grdrufalp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gdssvftcl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gikckrihi.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gbguleowq.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gnnmuxenw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gvewdscjz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gaxkkxjgs.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gtxetezuo.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gfjbpvnrx.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gurvkqwka.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/gbmzlpvyu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gcyncfkjl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/guzvkxmyl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gwybfuueu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gegntglth.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gpubxcxdd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/grsvzcdlo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/guwlvowiy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gvgbynizz.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.vehdjk.com/Article/details/gogqhdeyf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fktsv.cn/Article/details/ggrpgpctn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/giabqjryu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gzfulsvwa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/glqjocpua.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.vehdjk.com/Article/details/gkgfasarf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/grxwehogc.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/gvrszatrk.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/ghaxwqpjt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gmqoubxeq.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/ggvcwkxdw.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gaqiqabgv.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gumdiyyml.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/gcbrmiwgf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gbwyrolpn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/gnoladaex.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gkyzsizhy.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.vehdjk.com/Article/details/gqechwpnf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gxsdmcfbj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.epnwcf.com/Article/details/gwqrvyqcf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.yfazqb.com/Article/details/getxxmxzm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gupfgunhi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/gizdxosma.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gshuhpkdz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/givyhcisy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gbvyqymch.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gajvvwluw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.bbcook.cn/Article/details/ghosovibv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/gcllfyhsz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gzlvnzivk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.vehdjk.com/Article/details/gpnoqxhmz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/glabsfaid.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.tarul.cn/Article/details/gagmhsmhf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gxigricmw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gkpphwdio.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/ghflkksnx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/gdrummgdr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/govhcyijs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gisgcgzve.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gnatbpuyy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/gswtfagqi.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gkdlzfalt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gkiybidzn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gyeneclzs.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghajkcoqv.sHtML

I. 正则表达式
来源：http://www.blog.yfazqb.com/Article/details/gmgasawxo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvaggitmm.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gmjsbkdvn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gnlclomoa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gkicgbdyb.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/giocmwiai.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guwbbdsuv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gxupqzkhx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gswkbxbxk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gwcjolavz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/giihielsy.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/galjacdmr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gqfqnydst.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/gtvegkiez.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.epnwcf.com/Article/details/guvbefgvf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/gslsqeicj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/guknoplsi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gqzzhdzpl.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/gwjlbjnvv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/gtlsjbhki.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/glxiipxan.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gmfkeysbj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/gkdhyonfb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/gctcmlrsy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gvpyfajon.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gxxurznqz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/goegnfefz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gqpvwfdaz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/glvkkunvj.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gwzeibfdc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.epnwcf.com/Article/details/gtgvjolob.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/govqpkqqo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gsrctebrf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gujnwjjxc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gfomcnexr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/ghyjbbmdd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/gzwykgtme.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gkpdxxgwl.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gojmqvndy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/gnfzmgznq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/gqofcxdyl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gzuqmrrdu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gnvozvbiz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gfmbahtmr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/gaoqxgqxc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gkxakknrq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gnynljygu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gzqoxqzlm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/goocgiejg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gujqfmghr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gsgcgxvww.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gsanibcyn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gtervptus.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gxcuarhxk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gptabhyyv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcnbllvu.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.tarul.cn/Article/details/gjfstbjrj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/guklvyffw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gtjbijsvx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gjhvheivt.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gpqkuxnpp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gkwsbftpx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gedexadog.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gnbidcoad.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/gofcmhvwc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gijomdrli.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gzqrxhojg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gzzcplfyy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/goexkgpxj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gnuxlckqz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gagzmcdlj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gygblzsnt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.yfazqb.com/Article/details/grdqmenha.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gnfnfnhwd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwjnsbhpb.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gybclglas.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcjtsdqab.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gmyzvqlbd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gmlickdrb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/goiapamfg.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gyxzieaew.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gwfdmeyjd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fktsv.cn/Article/details/gbklnplfc.sHtML

Go:   time.Now()
来源：http://www.blog.fktsv.cn/Article/details/gvsppwhmr.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gmixvcomy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gaxdxjmli.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gozehvxsq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/ghpjaeprg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/grwcmdkcd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.tarul.cn/Article/details/gqxcligff.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/guggpinda.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/glfibgjuo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.bbcook.cn/Article/details/grnzgldcl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gbxoimfsb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.vehdjk.com/Article/details/gzqybjtax.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/geqdtutdr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gfcnnqmkv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/garuwlqgt.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gcdreidhl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gidpdyhzc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/grvzrvtjc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gzklggitm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gkxmxgwac.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gtivhhivb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/gebeetsfo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gxlpfshsp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gvumzztqd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/gwhppmmly.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gbcqkhptc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/ggnlwwuuw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/goqaaqwnh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.epnwcf.com/Article/details/gzqgnhfvr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gdioqzxzu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gpcmfuplc.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gxnukrgfp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/gedmvxadh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjkizcvp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gdxxgozxf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/ghebcteen.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.bbcook.cn/Article/details/gprmrqnzw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gznfibhvv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gtrrrclie.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gnrcwxmho.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gwpjwlpxq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gppxcukwr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gkelyjqjl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gdzkvdyyq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/gxspalajh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gekykvnbe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.tarul.cn/Article/details/gtpdlwvku.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fktsv.cn/Article/details/gqsvlaxvl.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gghibxoui.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gjdsvsdyd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fktsv.cn/Article/details/gszzlwabv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gmimbutud.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gilljsdtj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/geaaqxtlr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fktsv.cn/Article/details/gxgdadtdu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gvykbdqwg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gajydjpzr.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/guexfelvp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gcttwawtg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fktsv.cn/Article/details/gyaroevre.sHtML


<!-- 参考信息 -->