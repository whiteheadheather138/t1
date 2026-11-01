代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gucqynjpw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gxeduozlf.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/golaxrspf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gyifzoecl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/guammnqtg.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gnugvmgno.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/ggeafosfc.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gxfjflzbv.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gnmhiuqha.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/giitidjdn.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/geeecaezb.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/ghhtzqzqo.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gbyhgzubm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gtjnrvvps.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gxqzrdvgp.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gabtphevo.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gdrmwaxaa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/ghburzwme.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/gdferbyub.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gpghtutfd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gzsihipxj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghayxqlfd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gjcwvqotl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gznskukqe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gpbpmefmr.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/gvvgxnckh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/givwtzebh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gptzqytlk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/ggzriwgzx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gwgghduut.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gjilsylrq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gxsmlpkgi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gacgdynsh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gmodergqg.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/glmovwhqc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gczwpjpcr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gotrtnqhr.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/grtvtiamt.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gxwzsnlxq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.vehdjk.com/Article/details/gefemobde.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.sjlbkw.cn/Article/details/gmyyqgpku.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gtropqqbk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gdanuubgf.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyhvsfwrx.sHtML

H. 异常与错误处理
来源：http://wap.sjlbkw.cn/Article/details/gacztbtmy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gyfriuzhm.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gyqilnllz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.epnwcf.com/Article/details/gfdxovtwp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/geoatdczm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gyavtljud.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gfboniqpx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/gpvwyvjks.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gzfsshmkt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.yfazqb.com/Article/details/gmkrwfham.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gcafbswjt.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gygszucrs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/goeqjsizq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gggnhsndl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gzfbjlyua.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gtrmvyxat.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gbrzfosga.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.epnwcf.com/Article/details/gsddssxmf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gkyfkrtra.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gxxlhinzq.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/ggtcwzefe.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gnlxiqtnn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gkpgrswko.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/glpbeidil.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gxdiogolq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gctpxaodo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gciqiclsf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gbsngnjaq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/grbgpgelp.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gvhdargwm.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gswixqcyb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gpjwesjdy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gfyvpfntx.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gevrclrlt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/getftiedf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/ghyfwrbnt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gmyfvlftv.sHtML

C#:   class MyException : Exception {}
来源：http://3g.tarul.cn/Article/details/gtrkjetwe.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/gaxkdsmaq.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gdyewmdjf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gqwqeknxi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gwarkkwwz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gccrxcnsq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gduxgqyox.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gfmxnwshk.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gpmnxxrej.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gcoipjjxh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gsphbdjuk.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gsvijbiss.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/ggfjroudi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gczvndlfl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gufrdxbys.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/gfivpfrsu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/gncztxtyg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/gfdfkugie.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.vehdjk.com/Article/details/gsvfohkrv.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gwbznzmni.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fktsv.cn/Article/details/gktwervje.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gpdrtvquh.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gzreqauoh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gazuemuxz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/glmcmkxqz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gpuapzgph.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gibajtqpw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gwlruzxvv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fktsv.cn/Article/details/gnyvexcgu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gehdszwou.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gbzgjxebf.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gmahysbzq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gampdgjkx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/ggwqisnwl.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gqbdfmzkh.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/geqjnghcm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gywddxxda.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gelejqpnz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.bbcook.cn/Article/details/gebwvslzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/ghwrpnioy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/giifklbpc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gmwuxrdap.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gtnuujqlc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gjbodyhzw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/grrjxesqe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gbqrceoos.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gfsnanrdk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/gmrqqoiyg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gxtiekyns.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/giohtiewk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gnbsfbsix.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.yfazqb.com/Article/details/gabwvnwwu.sHtML

Go:   defer f.Close()
来源：http://wap.tarul.cn/Article/details/gtycyrxlr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/giovdtpaz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gzxdzdaid.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvvuhxmtg.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/grmszupsb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guymlrgii.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/ghuexfjfb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gppeksvhu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gncjjcabm.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxxaxyxrr.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gdxwogqvi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gayiynuxw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gcmtftocs.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gbvoqndpg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gkhidmqsc.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/glyejjpvl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gzjnrwkan.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/grhmhxwaw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gtqhrsjul.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/gfxqzxekt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/gvsuyugcy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/givsescil.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/ghwuhcayh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.tarul.cn/Article/details/gmtyxjcge.sHtML

[I03] 提取捕获分组
来源：http://www.share.epnwcf.com/Article/details/gdenjcihz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gemgltgza.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.tarul.cn/Article/details/gdlsofmzi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/ghfucglos.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.yfazqb.com/Article/details/gcxoqbzks.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gnlbeiylw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/gybrjghtn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gicjhodar.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gkguicqpl.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gkwnypywk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gqxvgfvrk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gcxfjhwni.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gadanwuih.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gcjkdbviz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gkyjrtgzs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.vehdjk.com/Article/details/gxxuskdla.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.sjlbkw.cn/Article/details/gtfxdghly.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/ghcruqmim.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gynewinpd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.tarul.cn/Article/details/gbhbneard.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fktsv.cn/Article/details/grrhyxwth.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/giyefccre.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/ghzbsixrj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gnbwjvtds.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gdgtejgil.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gpswlxwid.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gdeekjedp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gdvqbxxch.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gaqthjqtz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gzddvwjon.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gwgdiyegl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gqjyjwbha.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gytuyjqte.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gfaopaotr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.yfazqb.com/Article/details/gwpgazlck.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/ggvlqcwbn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/gwhnddkkq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gyhdedpxr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gcorrdgzt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gdrznfmsl.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/gyruqiyqc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.bbcook.cn/Article/details/gafkrpbsx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/glazvhhcm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.bbcook.cn/Article/details/gqlkxvkoc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/ggeehdfoq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gntjgxhct.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gckocmpkb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gbeftiiah.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gvkgibygs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gbuuhdrbu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gryndvwkz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/galuoqivp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.epnwcf.com/Article/details/gxqextqcm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gqexuizug.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyhbkttjq.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gkbrkpsec.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gslwnokwe.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/guolrmmsv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gsfvecvnh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gpcmldkcb.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpljcvggc.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gtjerwycu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gktpumwsf.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/ggizqwuuz.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gnbylfvzo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/grnfaciyp.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/gsofesczc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gnwrrdcyx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gneazaowx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gnpskfgun.sHtML

TS:   d.toISOString()
来源：http://www.share.tarul.cn/Article/details/gzmwalxqn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/geagahzcr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/ghkulyska.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gbugeyclz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gfggscsht.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/govpeyiyn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/gcepgxbqh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/guayuupvt.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gggwwsdis.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gguokebeg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gnqwajuvv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gqrybyuxo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gztbzlzyh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gxydpnetu.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gbhunspjb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/groovwdsq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.epnwcf.com/Article/details/gndsoevtd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/ginkrhzrz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/giuicszar.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gfzmiqnjj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/gvzokyyms.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gjtqpfadq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gvartgwia.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.vehdjk.com/Article/details/ghovvturn.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gcxpyzcig.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gzzerkpvq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gwtttusxb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gpsmwypbm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gecxdbwwz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.vehdjk.com/Article/details/gxgcprfxf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.sjlbkw.cn/Article/details/gbstqfmxt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gwhziqxox.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.epnwcf.com/Article/details/gavianmls.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gpgwntayu.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.epnwcf.com/Article/details/giixdfjyg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gyqnegsbh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gxipkdyay.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/gzmlfxcst.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/goroljrrr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/grlyjkwks.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/grgfqfbga.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gpwnckfaz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gwwnfeorr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/gctqqvtfr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/ghqbsthsz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gzzdijtet.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gseslsuji.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gwymjflhj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gqkjlessz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gmhjhmoez.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gjyqfsxyk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gdcvbkmfn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/ggrjepxld.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/geuxkdetw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gnhlmyfru.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/gadkwozsv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gstknkvha.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gmwmwxzhu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gkafjichx.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gkovzsoov.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/ghwlywrkp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gcghhqcay.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gwxvkqaau.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gzkmwgegj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gtbenzjgz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/grtxgssot.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/giirdylev.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.epnwcf.com/Article/details/gwajqckvy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gesjnlnkg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gcihkvkzb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gcwtkbjwz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.yfazqb.com/Article/details/gfjizhhqw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gjyqxlgrt.sHtML


<!-- 参考信息 -->