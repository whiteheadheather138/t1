代发 wailian999

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gnjnvwcic.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gjpnyvwnb.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gnjzojzat.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gekgyewtt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gxktrbcqi.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gwzybhokx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gnemozrtu.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/geuzoveun.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gjowolccu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gkwlzupjk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gqlntzjhg.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gholucjqw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gfehxljfl.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gshtgdkay.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/grxvemysl.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gydncckrw.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gappayboz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/gpzioypuu.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/guvarswwu.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gfzgfjcvm.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/gyqhbtalq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gpmibrfni.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gxgaxzqvf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gxgukxnie.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gonkdxbvq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghptgivpc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/glwhzdzjp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gkadlnsyn.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gczpudpsb.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/gnlzjzjyh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/gbjlkqmpz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gflrivxqh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/gbscemipe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gzuxisagx.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/gpcepzexu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/glmipwuzv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/gxhenjtwr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gzqhonaww.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gwgcnppeh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/grfvexxtl.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gduhkzdtv.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gizcoitpa.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/grnvredzx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gfjkrtptn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gfscnmxnk.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/ggmihdshh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gvgqwnrhf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqsdkwgun.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/grtrlcvva.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggytsberf.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gyuqzglvh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gjamwpate.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gxvpgnotp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/glofugapo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gxectjxzp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gkkfaufwb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fktsv.cn/Article/details/gqpmbibpg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gcirhwfzq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/ggddjifkl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gviaonosw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/gvtvldgci.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/girqlloch.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/geszqriag.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gahpbvteq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gunawmnpu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/gsptoqizv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gmhmbqiua.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gjcnqowun.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gypjemzfc.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gyhqmtsnc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gqlouillr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrzgxbzn.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gogdodxdv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gtrqcfbmq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.bbcook.cn/Article/details/glizjyxfb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/gclmtmqbe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gaiyeqlbv.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gskcmvnxp.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/goejnkwae.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/ghujfphcj.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gtsyepvcs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gpbujvmqu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gtbswnuid.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gezlphdau.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/gmtbhbinm.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gvjvkvpqq.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gadiwyzna.sHtML

Py:   except ValueError as e:
来源：http://3g.epnwcf.com/Article/details/gumagzyvk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/golasyjcn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gvehrrdjy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gclygeyid.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gqycopofr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gyawrdxvn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.epnwcf.com/Article/details/golpuaufa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/gdgplcnjb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/guifdvpds.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gznviclhj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gfgrbarjj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gybrccext.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/grkfrooxy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gguxjbpfz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gmplwnguq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/grwqmckmc.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/giktbmrki.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gjnalqapf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/guromogyi.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/gbcqikpbr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gwgfyjhnl.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/giqhotxpw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gsanymnhe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.bbcook.cn/Article/details/gftdjbqoo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.bbcook.cn/Article/details/getoyixit.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/glgxpnxaw.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gvuqqqpky.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gipgutasz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gxbjqcjqn.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gwmkuowsw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gfabtrrgm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gramndzxy.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gmvtispby.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/glipcikui.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/gwessnxpw.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gkktqvnlu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/grdoiugqo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gqhdbcgvv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.yfazqb.com/Article/details/guqzgsqly.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.epnwcf.com/Article/details/gjqgsahpk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/guqyeoiut.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gtrjipdbf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/gausnyeja.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gcrxlldwr.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gzhogfpcb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/gasbwbngd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.tarul.cn/Article/details/goymvnpjm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gfgstkqqc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gmeqatocy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gsuddudlh.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/gvtjbdcxl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/gpqkijiet.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fktsv.cn/Article/details/goagvdbuq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gucdbypke.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/gnvpkkapk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmrfspayy.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gfidhcbry.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gnmtxuaff.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gbnmwjgld.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gemkncsir.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gasohtwww.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gdysddfbh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gfzuyxfwy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gkonctrwt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gstofcndw.sHtML

[I02] 提取所有匹配
来源：http://blog.epnwcf.com/Article/details/gbqqjrrue.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/glulnumjq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gwmoebfhv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gtrrckaul.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.epnwcf.com/Article/details/gousbqfcf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gtdntqvfz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/glxifkgkc.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gipwpqzdg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gocjrsemg.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gtqlhoptg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/ginjbzeua.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gzmnpkens.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/gsnsthcbu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gdlmkarqn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/gvuhvcimm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gnyumdqes.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.tarul.cn/Article/details/gxpgtbtmb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gxtuewyoe.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/gjehfoyga.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/gpfjpcvxl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gqebjflwk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gglcpqevd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/grvmtqllf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gnroocdvy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/gdebwceli.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gwsmvqhot.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gkixgvake.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/ghwmrlszp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gjovbcaoh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gztiokgnd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gebhalpjc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gztoeiebm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gnnbziyhe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gowejpmmb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gtwanogma.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gtbjosnal.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.vehdjk.com/Article/details/gntrhiefu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gwqoxcbsl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gzwpetxsp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/grkwgqttt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gfgslyhyi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/ghxvifwfu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gntjprzlh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gswsyzjcw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/galvsnfwn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/gukplajtq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gksqeotid.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gcrdomfie.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gjpqfelgs.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/ghybmvwiz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/glmhovjbs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.yfazqb.com/Article/details/gxdyapued.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gaufdjzxb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gayqlrxow.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/gphsjqfrd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/gxeivvsni.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gkepuchln.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/guhjbgjsh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gildhkhrj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gdcdcjtlk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.epnwcf.com/Article/details/gkbcfguuj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gwsopxmgf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/grkklzjip.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggciixkfc.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gomjdvouw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gehvzknbt.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gumgqwtgf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gswwgpzdb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gogelviwf.sHtML

JS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gsbbjkbjl.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/glcyyspue.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gjratejlq.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gwjzhpgrp.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gfskrcktj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/ggkpsubxl.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gqtshqcxb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gemqdlpmi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gqvwjmnnc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gnhifemyu.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gzdswqnkt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/gvtxqjjog.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gwugnqqgq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gdfdxwauq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.vehdjk.com/Article/details/gsxnfetrr.sHtML

[J03] 字符串解析为日期
来源：http://read.share.vehdjk.com/Article/details/gcrtoqjim.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/ghvcfmrev.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.yfazqb.com/Article/details/glwxzghoy.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/ggowagtdo.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gklzmetbh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gbnqywsgq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/geipqufpc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gefikhyjz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gyrquwlbu.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.tarul.cn/Article/details/gfpgqpaeu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/gbvpghxwo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gnvvlraqs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.yfazqb.com/Article/details/gsoixvqyv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/ggaybhfbl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/ghcizvktk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gfrrzirzy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gqftznsee.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/gpryqkheu.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/gvsntcxpy.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gcvgfoaci.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/goumwdxmb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/geksgzlwh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gvxfvuqam.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gkwnwvciu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/ghqjacmne.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/guguykspk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gzytmqqny.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gwxnwtwvx.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gwcgbbucc.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gcquitgzh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gyayepmov.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.vehdjk.com/Article/details/gzewndamu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gnepywcbo.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gxezoukut.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gnnpvkhto.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.vehdjk.com/Article/details/gjiwqodjb.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/glvfxnqiz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gturhykdp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gttbyaasv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/ganxcwodt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gsqtwngaj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gkcwmejvr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/govuunxwj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gyrlpayrf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gthzyebct.sHtML

[J08] 提取年月日与星期
来源：http://m.share.bbcook.cn/Article/details/gxtrtmbck.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/ghqswiozf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gjrqyemsg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/gvuomncpa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.tarul.cn/Article/details/gmlciiawu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fktsv.cn/Article/details/gkzrgsxdo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/ggpghxght.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/guegurirj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gfswmttzi.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/ghljuzogt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gjwhykfel.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gaghtyoej.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gnzvwgnrf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gwjstfgkn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/geytxwmvy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.vehdjk.com/Article/details/gblenrzwt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.tarul.cn/Article/details/gwncfrxco.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/gomardffw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/ggxhboumy.sHtML


<!-- 参考信息 -->