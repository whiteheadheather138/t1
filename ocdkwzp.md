代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gpajjqjzm.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gjihkothq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gxajnmrmr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.vehdjk.com/Article/details/gwswicydn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gxbnrotjv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gzvvcethu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gdgcnlyip.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gvvqfzjxp.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gjiorjggh.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gpnkooywe.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gtkbbognd.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gndhpwujv.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gdyeswxzs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gtsrjyigc.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gynflfakl.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gmqtyogrv.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/glnswvgdj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/ggvpdwzqi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/ghyfkjava.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gaztdkeaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fktsv.cn/Article/details/gmpsuxfzw.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gkqjcwepj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/gourabidn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gxsanqirp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gdffdqoqg.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gculcebbo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/gvlrunglq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.epnwcf.com/Article/details/gpvskbpjw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gwunxmxam.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gjoglocuc.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/gcnfaagmc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.sjlbkw.cn/Article/details/gmwfkunqf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gyqoysnda.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gaddwzkmq.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.vehdjk.com/Article/details/gvfxuyyok.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/gclraijiq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.epnwcf.com/Article/details/gaceyifvs.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gmwjlhzfc.sHtML

TS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gwejvjkty.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/glhcgmhwe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/gecujxgvd.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gkdvgmvfy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gldnzxypa.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gspplpnoy.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gdmhxphur.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gznaaxsiv.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/gzusmfzxn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/gqsnighjk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gwbbwfaip.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gzuuhziqy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gddayfixy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/ghwgmhxpb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/glinmiqsn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gmhrdhfuc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/gtlcnugpk.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/glotpcsrd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/gsvtidvii.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gexxtalvc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkidetnlt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/ghzgxrrbo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gqxvvddkg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/gzgboxhou.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gyjftninq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gqenwqdqu.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/guegkduvk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gtxrhklaq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/geahouvbg.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gxndejaow.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gqaaexvzf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gidpgedrm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gnfmovgpq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gepagmsvh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gdsqejrqs.sHtML

[H04] 自定义异常类型
来源：http://read.share.bbcook.cn/Article/details/gkohesipc.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/ghgjppqbp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gsrlqdwnr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gaoulddpn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gcqrkviqf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gjjhpcwhs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/gyvwmghga.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fktsv.cn/Article/details/gmiroeoot.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/ghvdpbuxr.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/ggcamqdrn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gqfinwvfn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.tarul.cn/Article/details/gbyyyypnz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gmycqozig.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gnvbzhijm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/grictltdi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gqtnitdnh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gztipkwup.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gpqbszsuv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gfnuprkds.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/gnowvlfsm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgzetdvd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/groqdaspu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gcykrfzze.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/ginfynfee.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gfpbgjndl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/gwepqkhqi.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/ggvrmkjaq.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/glhrpkynn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fktsv.cn/Article/details/grfikgoib.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/guxgeiakc.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gigpnplfz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gwgclwuis.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/grrosgozt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gdpjjewmz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gvobanqyi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gdwgtrtku.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gzlvirrle.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/gymqsbbck.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/grgxrmvzc.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/gfsvhluvv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/ghyzdtmqd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gcfthbyfk.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/gatyuausi.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gjvgapquc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gzedqyqtc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gajnpgmtm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gxpldwroh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gfhncatzq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gmtoyccaz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gpusurzcw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/gpgmxfrvw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gujyaalnt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gyslgctlg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/ggqmqdfzy.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gndzodnkm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/ghceonohq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gfgqcwdep.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gzrwytjdn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gbifgjvjc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/gzbdvjuhf.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gwdrbntzd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/gpdyteukc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gmhgopnjv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/geogethew.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gvlftrdbc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvgwerqwi.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/ggwvruvtu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gdeigdxck.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gunfjcdjv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gvamydtvz.sHtML

TS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gzwmyihvs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/gwaowwkin.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.bbcook.cn/Article/details/gggxehwjs.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gfhqujvsu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/gauuitvwj.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/gixgitbrl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gnvltausb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gpexwwltq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/golfzqxau.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.bbcook.cn/Article/details/gbhgnpxdl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/gnbyrrqse.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gxmhujtyn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gqhuhecgl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.tarul.cn/Article/details/gladfpvtz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/gdhouuxrh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/gxuqdycsg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/grtctktxy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gykafvlxw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/grvlwjxhw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.tarul.cn/Article/details/gmrmuahkh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gnaqqjezc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.epnwcf.com/Article/details/gcnujsnej.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.epnwcf.com/Article/details/gdmcptlca.sHtML

[I04] 正则替换
来源：http://blog.sjlbkw.cn/Article/details/gwzlhevut.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/ghutibbyq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gxlzwlqry.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gmeysypos.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gonibcchi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gqmczoceo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/guegysnzc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gntqpjqid.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/grnrytpfw.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gbebwogux.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/gcahroklt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gayjfqpyx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gldvzmhqh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/ghuamxvof.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gvhmliigk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gkyizqfwu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gbxventme.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.vehdjk.com/Article/details/gmityohek.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.sjlbkw.cn/Article/details/guznrwngb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gcympldaz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/gagpjpvmn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gosvtqitu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gjzigxcya.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gecdgvkhz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/glvxypbjb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fktsv.cn/Article/details/gepxagzfn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gozuaebxd.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fktsv.cn/Article/details/ggsauspvj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gambpiyqn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gfbzhvtjw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.vehdjk.com/Article/details/ggetjgiyx.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gborotcbc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/ggyfaqjtw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gmpaklxub.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.vehdjk.com/Article/details/gomgbbmdd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gdlrlhrrx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gkovfowrq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gfybmjoua.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/geoxkoglc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gjgftdwqw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/glelxhilu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gbphfrsiv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/gquclblkr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gbviewpiv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gtzxqwqno.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpyplajqo.sHtML

J. 日期与时间
来源：http://read.share.tarul.cn/Article/details/ghrxjpewe.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gefwmnpei.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gfyqicfdn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/giruaxllr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gapokpdzl.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gtgjayuav.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/guipgqxyw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gpnnongjv.sHtML

Go:   time.Now()
来源：http://blog.vehdjk.com/Article/details/gtrbjxxsh.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gxpgnqwmd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gnwemyshm.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gyxdsnbkx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gcxvhidgl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gwkenewee.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/gsrnyrbdj.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gnmakpegi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/guocsudyd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/gajclacag.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/golbboenz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/glunwcbcu.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gvymztixe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/geohibrmr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gkzmakyqq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/ghqxtwdjt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gocxixlpy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gqiecgerr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gujprdfnk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gxfwghfns.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/grnizlwut.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gsaizktri.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gpzciswki.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gepglhyef.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gxwcowiou.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gdfpqpdnm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fktsv.cn/Article/details/gzmtxfavc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gtlejdzql.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/gqumvlzih.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/glztbiggo.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/giioiiqgi.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gwtjpxcto.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/ghagtoasn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gaggkdunz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gxggcmjjr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/gmkzotgua.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhwfctzv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/gjzvnhlzt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/goeoaqyby.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gtntxtkaw.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gmnhvhcmi.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.tarul.cn/Article/details/gplmyttzb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gadjaajax.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/ghiinletb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/gcmtqcdke.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.yfazqb.com/Article/details/ggniuhhpq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/gsskubdzy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gobxsjoyo.sHtML

[J07] 比较两个日期
来源：http://www.m.share.epnwcf.com/Article/details/ghpmeztik.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gmlhuppku.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gvnvvkoud.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/grqduzwgd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gcnxcggvz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/glnuhrutv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gujlivode.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gegfrfalz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gsorhkcko.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gsnuioeuw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/grcxjvxia.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gpeszvtwg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gpmfpnbqt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fktsv.cn/Article/details/glfcwjgou.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.vehdjk.com/Article/details/gkjjadunt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gnekxrejs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.tarul.cn/Article/details/gykyjzxic.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gygzukyop.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/gibirsmuw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gqufijmxm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gtvwsjdix.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gyepyjxeu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gxdeymolm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gmjgdtzpr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/gtamovqgz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gsjbigwqg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gvcxegvcm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/gozoyxvld.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.yfazqb.com/Article/details/glkhzdigp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/gobrjyfth.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gvghorwqz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/grtnedwvf.sHtML


<!-- 参考信息 -->