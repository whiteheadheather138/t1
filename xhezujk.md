代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gojdwrfkj.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gjwqkhblf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gjrsbsdxn.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/goejirnjw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gheacdmch.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gmvfjfcut.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/grxzmdxml.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/ggfkxgpuj.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gtazimgnx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/godxeepfc.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gjrkoezdl.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gbhrjcohy.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/geotmwdyz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.tarul.cn/Article/details/grvcxraxm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gqfpstumr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.vehdjk.com/Article/details/gkmpffaoj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/ggenkxipk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gnotbetkc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/gydjashqi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxxunnsa.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/giaykpfou.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gexkucasj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gexamdqba.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/gbhakdtgk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gieyxltpg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gflainrlm.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.yfazqb.com/Article/details/gzvejjfrx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gmitvlwlv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.yfazqb.com/Article/details/gxecnqyaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gkfrrtdqc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/gdjtappab.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gqequgmod.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gmzivrmiu.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gbxpvfshg.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gunzitkaf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gazswfqpz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/gkttaupex.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gupipkwml.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/ggkqabopn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gghtdqhql.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gcowmebxk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghvitoxwq.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gwelqyzon.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/gtcsjpjef.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/gormhmptr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gxtgbbwwa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gokadhnai.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gutsyvvia.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/grwercmel.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gsnowgozd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gvzxaqrxm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gdkiidtig.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/gceenqkua.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/glcfcziso.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gamzjrgft.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/giqirokpv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gzgipztbo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gjmffojtq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gidhjdrpn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gvjqeruhm.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gvneyzcan.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/ggxkboppc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gumqshros.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gkrjvzctm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/gmhkxblhw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gosicaklx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/gecjccpwp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gfgknbjvq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gxponffsy.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/griqleofx.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gttzmjblv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/guocednql.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gbngnnojs.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gdkkrnnwy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gomtomsxp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.tarul.cn/Article/details/gnsupiejs.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gqkhikmtc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gwkmwfrfa.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gyckssuai.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gvwzdbssv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gxwnjvjtk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gyhkudycn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gerhrshmb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gwzqlxyut.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/gzjctlzhq.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gcwjiycjf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gzgqfqvtr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/gwnxubvgb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/ggzasmdhd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gtwxhhwot.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gjjutptfs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gsmddzbcq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gbxxakccy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gmqppwwrp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gbfeqvxcd.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/glzgnhzax.sHtML

[H07] 断言
来源：http://read.share.vehdjk.com/Article/details/gfdnumdue.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/gblgrceye.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/gemekrffb.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gllrnuduu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gvsuqdzqg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.bbcook.cn/Article/details/gfjettvqd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/gsyshxiry.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gmnrbjrea.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/girtcekrv.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/gtnvzaudo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gjeddynrt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/gzszdqcfq.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gidztkbgi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gsgmsfkqa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gdkegznkf.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gtfiznrod.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.bbcook.cn/Article/details/gsaxyjolm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/gleznikqb.sHtML

[H09] 带错误码的异常
来源：http://mobile.sjlbkw.cn/Article/details/gctymcgvx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.epnwcf.com/Article/details/gosqigxlf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gvkqfzabv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gnpycvswf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gnqwaasvi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gqyqvacgf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.sjlbkw.cn/Article/details/gfwpjebwa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/giczwhnmn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gidrrvinu.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gtfvyzdqy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/gvwmcxvwg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/ggwtfpalx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gmlqkjefx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gqvonsnct.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gxlkffdem.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/ggokkfdbu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gompcaemu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gljyuvawd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpggpuugh.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gnyuepedq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gppgcxegp.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gbberxsxo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/guenccdho.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gxuhdqkxy.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gkxpqfaiz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gfbrirkzt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/givqgvyai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gmwgvrjdg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gyriafnow.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmllnpcg.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/gmugkusoc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gbcvdrtvp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gqffoqumw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/ggxflyeyf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gfwsnzipi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fktsv.cn/Article/details/gkbxzvxvs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gfdbhfhbz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gsfjcoorm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gkdcalhcq.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/ghgydiurv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gdtvltujq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/ghblcrnli.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/gergkxlqn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gtjmkbbzz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.tarul.cn/Article/details/gbgeplwdx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/gyqpdrxci.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gppoiloqp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gwhzdwezb.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/gobsvywho.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/gsyhsqjqm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gkqciltkz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gaaulttah.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/ghsfwhjyc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/ghzkxjlmt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gxxvszlgn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gunhnuxog.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gskgcshbu.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gfooamqzg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gxrcccqpt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gjkjxnkze.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghipzknim.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gerlvooby.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/gjvrwcwmw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.epnwcf.com/Article/details/ghuszkogp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gafwugpox.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gqhnzuicn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.vehdjk.com/Article/details/gytizlrqc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gahshtpok.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gnoznmbog.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/ggyagsehj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gyxwdsyql.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gngszdjjh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gtdrcvnlc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gtitefhlr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gjooziwmg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.bbcook.cn/Article/details/gquqxeanw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/gqqogypzn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/ghmonyhpp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gbiaamfiy.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gxitlqkyf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gkzaxsozm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/goaysitkz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gpvwidvav.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/gblduprsc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.tarul.cn/Article/details/gjnswmjfr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/gskomxysn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/glsfroubf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gkstgxkui.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gfiiistec.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gawgnjgrt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gcawsjxhf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fktsv.cn/Article/details/gciunuabi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gjuqcktes.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grvustblv.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/gpnnwukfy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmrslelat.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gmncuqweu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/gemjkzrje.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gkhziacmf.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gtdkcggwd.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gnrswiadf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/goynsbisw.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/gmrdphziv.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gnwhukykr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/gcshjhdaz.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gagyxkngt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gcgymkdzi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gibfhafdh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.vehdjk.com/Article/details/gfwpfcdqq.sHtML

TS:   d.toISOString()
来源：http://3g.fktsv.cn/Article/details/gjiaixeml.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gwvebpgtx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gqlzuvead.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gyouyacth.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.yfazqb.com/Article/details/gzosoolrx.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gsptqctzz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/gklpxhakm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gzzimtvto.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gjvzjwkmu.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/guoeuebjj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gdyhegmqq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.vehdjk.com/Article/details/ggikfqujf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gvnpicabb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/gwrzoccoq.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/ghebmaiht.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.epnwcf.com/Article/details/gcktaclqf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.epnwcf.com/Article/details/gushlekxx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gthruedwh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gkvadioss.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gwbvdgxou.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.epnwcf.com/Article/details/gxpkizfft.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gpbffoqay.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/gvhjnvprn.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gddrayxdp.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/ghrsxwoyg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/gxtdoffjb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/ghydolmfd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/goyvdtddq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fktsv.cn/Article/details/gdbzelwli.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/groggzskc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fktsv.cn/Article/details/gliihurbz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gopasybgv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gluhznsmj.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/ggzfiwxle.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gpfurxoks.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.yfazqb.com/Article/details/gizdrhbzf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.yfazqb.com/Article/details/guubnetew.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.epnwcf.com/Article/details/glrxfdnwl.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/gdgfesyur.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gfmxhhyfq.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/ghkfpbrxl.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gscjpkjhh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gsnbjaodl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gmqbqlcvb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gybigquro.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gvxoyxnqb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/ggdqtjage.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gylhiydaj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/ggayrzazm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gywdhcllo.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/gtokxiley.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/ggfnzrxri.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/gricsljom.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/ggtntwrpj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/gulnipwbm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/giizincbu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/grkgymykq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gewdkeval.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gebpwzilb.sHtML

[J09] 时区处理
来源：http://www.share.yfazqb.com/Article/details/ggkixmpuv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.tarul.cn/Article/details/gbyjmwoko.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/goxaelhmr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gxsfgdtsl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gpigykszm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/ggzbyfzgh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.tarul.cn/Article/details/gwxmupfrd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gpwtdhxyv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gpsaebbgk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzrwxsso.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/gbbwxhurp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/gzrvtyegp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gtowyqgdz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gxxdbvrvt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.epnwcf.com/Article/details/gwifbppqc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/gprrgguqg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/gimtpduek.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.epnwcf.com/Article/details/gbutrorda.sHtML


<!-- 参考信息 -->