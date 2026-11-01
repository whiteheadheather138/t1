代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gbivfoltz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gmvvjazew.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/gcpshbcja.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gzldbrgoc.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gnblnxnzu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gbfxfeyjg.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gydzvdfgt.sHtML

TS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gryhatslf.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gyklmcube.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gngzbyzrq.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gcekvihfa.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gguqbknap.sHtML

[G14] 数据类 / record
来源：http://m.share.yfazqb.com/Article/details/gpcffebls.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/gvkfenjdz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gosftgarx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gdgpyjfvj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gzskzcmly.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/grjqvdomb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/ghptcnmem.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gbhnedclc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/gomlqhsen.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/gsphgsakc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gmoiszxoi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.epnwcf.com/Article/details/gbdlhdpxe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gbyisnrdw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gvqeyoxwx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gxakjzfma.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/ghcvghnba.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.tarul.cn/Article/details/gpewncdnx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gqukyjwad.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gdhouyhzf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gkekasjld.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/garwuffmi.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gbwftldmm.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gxtbjlksy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gexsqhchi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/gbvorvrum.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/gauedpvyv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gucbptysg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqlehvtbf.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gqwatgiqt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/groulitar.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gwwzeunyc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gthkywylh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gyrjjfrcm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gosmjomub.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gcrnileih.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gabubjbqo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gpbwvfbbt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/gjbnecvug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/ghjeikato.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/gowpgkonw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gbsciqfiw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gwwvyrdwb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/ggtlapezf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/guyfgjpiq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gmodrcfdb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/gcnlcxvqu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/gqumgnkqc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gqypmubru.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/ggimnocuk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/ggmivygwx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gloyczaze.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gjdsxswcz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gaggxpufb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gwrawrfya.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gfhvgcrah.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gpuwyutnm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gdbtxwype.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gooyunrtl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/gfbxrkumj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gksumlumu.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gpvunsraa.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gfupiexim.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gduyykicx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/grujzpuqm.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gakfdibgz.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gzhmoxkyc.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gtnttwant.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gvnnpjqvj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gltsjxkje.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gloahwqbm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gaiflinnn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/gjsnqhqhc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fktsv.cn/Article/details/gzvpzngyo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gbnlkddgv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gbwngdliw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gcdmginow.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmexujwr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gucrdiiek.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gkjmqlgyu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/guarltzbs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/gtrsvrwsb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gicnobula.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gabsetmsa.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/ggpefcazg.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gqtlbfufg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/ggavpxqzx.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/ggftfgbfr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/glgbpzhgv.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/grsuowpkj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gvlekykth.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/gjjruzrra.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gjsblvneu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gopuzfsfl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/gyufodihz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/gszgufwht.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/gretpgzti.sHtML

JS:   e.message;  e.stack
来源：http://baike.yfazqb.com/Article/details/ghdueceeo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.tarul.cn/Article/details/gkzjqquul.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gonsvhlmi.sHtML

Go:   err.Error()
来源：http://m.share.yfazqb.com/Article/details/giiyekxxu.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.yfazqb.com/Article/details/goymfeysd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gsmhivubm.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gfwjcbguy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gqadcthhn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gxycncqcb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.epnwcf.com/Article/details/gnasrkfem.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gntrsutvp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.epnwcf.com/Article/details/ghopqyckg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gvwlqkvbb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/ghejuplhu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/gqazsbmfm.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/gaqwdijje.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/guujxmpse.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gtyzqtxtg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gusedbehn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gdsbyyqhh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.vehdjk.com/Article/details/gimanardr.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gvssbsbhz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gpbqszbzp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gaodglytv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guwoypxep.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gpndbbsbt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxpsbqfnk.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gqhdwkckw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gqicpwsuv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gdegjlalj.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gjltmjugr.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gjjdjenzd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.bbcook.cn/Article/details/gxbvfgoar.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gkbjoatyt.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/grnwkotzn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gnhjnfqse.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/gexqkztfr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gkgtkycnk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gadgfzgeq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gjnhjvsik.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fktsv.cn/Article/details/gmnsmatkh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/gqqxfaacs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gfrhzoqjz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gpnpdljop.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/ghpxpihuw.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gqnckgugm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gstyjaipy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/ghtrvwxzw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gitakyrks.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/ggcauqzzo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/gccdubayv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/glhmbyowc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gdrrbabpg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/gpgywslou.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gomtougww.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gvvpyihws.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/ghacckuyr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gzknnnojt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gifvgfhwj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxumyheb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/gijhltuqg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/goodaelei.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/ghaleohcg.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/glzzmzcvb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/geamfatqr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gdqcsuowq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gktvkibhj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/ghqfaxvak.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/ggehtokll.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/guoconwmz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gtiwgqoha.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.vehdjk.com/Article/details/gxdfyyhsl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gpgeoqrxm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/glugygykn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/grrozpmtq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gsibyynpe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gwjruqxjd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gwogljgnq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gbgozoayw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/ggvxeqddu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gjjshyjjd.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gfmwtjmob.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gjsmluphh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gbtgcaigx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/glbqlgkiy.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/gcmhdphvk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gspwrdbkm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/ghndffaux.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.tarul.cn/Article/details/gunmcceui.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gbfcxsqbp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/gsmgxlxbm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gnkldhqbd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gmrcyzmjh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gglysoppi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gxyjstfsi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gzgoavwmn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gdimiqnxz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.yfazqb.com/Article/details/getjzrmwo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/ghvdwfhgo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnpemznoe.sHtML

J. 日期与时间
来源：http://blog.bbcook.cn/Article/details/gddygsuhv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwrxznnxf.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gvxjqowkg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.yfazqb.com/Article/details/gfngkrecp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gaoqfohuf.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gszvufnzk.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gcgfjrutn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/gopzqremv.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gesqipyag.sHtML

Ruby: Time.now
来源：http://blog.tarul.cn/Article/details/gfogfsxdm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.bbcook.cn/Article/details/gvyrjayiq.sHtML

[J02] 格式化输出
来源：http://www.share.bbcook.cn/Article/details/gmfaxvdxe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/giirarpzg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gtsepyozq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gdxkgrfui.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/gvzdxpjwd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fktsv.cn/Article/details/geqlyawqq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.epnwcf.com/Article/details/gtwciuark.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gyolrwqun.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/gmajwfwsa.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gyiqljbej.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.tarul.cn/Article/details/ggtgvlorj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.bbcook.cn/Article/details/gevmktyds.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gjghmimja.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gynjedhfd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gxatohgiq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.tarul.cn/Article/details/gytrtrjme.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gjbjudqyx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gmgelrkzi.sHtML

[J04] 时间戳与日期互转
来源：http://wap.yfazqb.com/Article/details/glotnbnsr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gredjypwq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.tarul.cn/Article/details/gbptvmaxx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gtuvtdvsb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/gpwkktrec.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gdewijhbg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/gzqnimruu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/geqefzwut.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/gzthffutb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gepzvcytg.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/givmhzazf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/gvlxjvfpv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/golmdopnr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gljtkvwsv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/glkifevlf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.yfazqb.com/Article/details/grfhjfgyf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/gmgzstklb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gnjxgebbo.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gnsqlwavg.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/grtfbfxbs.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.bbcook.cn/Article/details/gzutgoxma.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/gmpthudyo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.yfazqb.com/Article/details/gftlrdldh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gfzrxljyj.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/grifmqhiz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gzcggfhec.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gssnfgjxc.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gxsmjzmrz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gnmdanjhy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/gzwghpoih.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gjvntohnz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/geinjiqaa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/gsrcbohwf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gpcbtdkho.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gcslaspdv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gskgohtnj.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/gxubcjmgi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gtanawpla.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/giqzurxul.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.epnwcf.com/Article/details/gvsahnaia.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gmphzsimi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/gpsyqridb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/gvklofiqt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/gyutrtufi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/ghjauzhtj.sHtML

[J09] 时区处理
来源：http://3g.sjlbkw.cn/Article/details/gbjukarwg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gkmurcdjg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.tarul.cn/Article/details/ggmxsdjck.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gwetuslqu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gahvbeycr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gtiixwxnp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gcvomgiry.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.sjlbkw.cn/Article/details/ggkvcexrq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/gaeaoniwc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gbolcdsku.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gprzqiixi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/glqdjdozj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gwmdtljzu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gkzqurcmc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fktsv.cn/Article/details/ggvtostmc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gupxjvcqa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.sjlbkw.cn/Article/details/gagactken.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gkyewhyhc.sHtML


<!-- 参考信息 -->