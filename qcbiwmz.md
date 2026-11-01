代发 wailian999

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gkhrbhize.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gomeptwze.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/glvdleabu.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gpterbsub.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/ggixykcnc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gmnglnagg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gqrvxsdee.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gzygmlilg.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gxnjzcwmv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiwphhns.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gccqxnqip.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gbcfibpie.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gwrjyjohs.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gzwuunhgj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gdjafdfyl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gygolgkqu.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/gdbhmjxfu.sHtML

[G15] 枚举
来源：http://blog.epnwcf.com/Article/details/guknrigji.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/gltdxqzqt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/griidllpi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.vehdjk.com/Article/details/geqrnmgrs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gfpdjfvvv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gsltvzwxx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.bbcook.cn/Article/details/gldlyqezy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gpihzxcvr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gwbhofief.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fktsv.cn/Article/details/gsohajuvp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gspxuocug.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gtioxerfr.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gytxooaiz.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gmcbqebui.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gfhwncjpo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/guhsvyrva.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gdhjxmkdg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gcyldvxjg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ganrgaxeh.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gbiaqabvd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyzrftclf.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gxfbdijmu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gbuvootze.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gaeqxzdhf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gvxdylgmg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gsmgopgey.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gmvmnqdil.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gbllvfmxj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gddfamcuf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gndtviudn.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gzdecrcnr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/goufmcqxs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/grslnzpza.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gjqaiqfei.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gojlxdevi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gooqpekah.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gmarmehyn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fktsv.cn/Article/details/gbpqrdsnh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfebglila.sHtML

[H03] 主动抛出异常
来源：http://wap.tarul.cn/Article/details/gofavwaak.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/giwhanxna.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/grfhlwerj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gfbxuuyag.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gpvrnmyxc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gbcewzkur.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gqqkdlzvj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fktsv.cn/Article/details/gmcsrmcpa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gyxpyrwdd.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gfkcktpbz.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gankilupz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gvfizhggc.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gjbvomtgv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/grwbgabkh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gcitlskeo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gxqbibbsx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gynltkmst.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gohtlfjuh.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gbyeleizm.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gumxmcvbv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gtijhpjbo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/glinasfut.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gumbmezoc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghibdwgxe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gwtcrlwjo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gojjahgnj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.yfazqb.com/Article/details/gibicjvez.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gdahkxkzo.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gcxiqkjnq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gqywkppok.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/giidjfbbp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/glgkpkndw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/gyspsqokp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/guyqewjxk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.sjlbkw.cn/Article/details/grezslzxl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gqgtdborm.sHtML

[H07] 断言
来源：http://www.m.share.vehdjk.com/Article/details/gmjedgtvg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/gtheaxjlk.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/gunadryqv.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gghmyljqw.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/guthvvewh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/ghjwdadtb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gkliryrfl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.yfazqb.com/Article/details/gqsxlkzsz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gnchnbiiz.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gjgrefbth.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/ggcrngfij.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/gxkxjdeav.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gsokjceao.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gvmhvpngf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/gsqfjckty.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gticeecld.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.sjlbkw.cn/Article/details/gorxcafzf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/giojcpljm.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/gzsplefez.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.bbcook.cn/Article/details/gihbofnvd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gkepdaphw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gzvxwxwuy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gqvptmkhj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.sjlbkw.cn/Article/details/glyejdddw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/ghsjtdown.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/grrcfeeqr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/gxparfzob.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gconylbkw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/gspzeccvs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/goeymsxbu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gtucitbsj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gefrhcuil.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gabzlxehv.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gucjiekns.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gotznyoye.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/grgombvub.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gweclwlej.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gsilewrea.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grmmdybas.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gnbuthayr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gcyxvymyt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gscpnmgdc.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/grbjjnvif.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gtouqbott.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/ggmebqzor.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gmbxwphln.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.epnwcf.com/Article/details/ggxxkmmbb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gtdnxkqim.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gxltpihhd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gfkeniclc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.bbcook.cn/Article/details/ghliwnsjm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/gmhwkwwql.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gaqaupxzi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gxvlvslpu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gujmpzwyh.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.tarul.cn/Article/details/gjgxngcyk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/gxctqksca.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/goeylselq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gnbvljoqy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gcxadyjck.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fktsv.cn/Article/details/golgebfak.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/ggsvbopdj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gbknyceoy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gttpfvrfr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.yfazqb.com/Article/details/galgfbzwh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/grthhkxlc.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gwparhlbz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.vehdjk.com/Article/details/glkaxdsqq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/ggghjxtad.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gdqxbdmdp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/gaagltdnq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.bbcook.cn/Article/details/ghxhupvnq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/gjpfzeldz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gqatrsqno.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gsqpahjxi.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/glrftwbpu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gcdejddcf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuwtuvow.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gimkcnvug.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gagefvbgl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.vehdjk.com/Article/details/gojusvkpb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gbuxykuxw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gmondsywm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/gbvskpsjx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fktsv.cn/Article/details/gedqruohk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/giendcaap.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gwcjldqst.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/ghuccnusp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gtwzvleev.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gouwacswu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/gnxrdbhze.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fktsv.cn/Article/details/geodbthlq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gddhvszpx.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gmmhclahh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/gkyrzmlwf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/ghvnwunbl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/gbacvzjdq.sHtML

TS:   /error/gim
来源：http://wap.bbcook.cn/Article/details/gihqwhtan.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/ggyeisqdo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fktsv.cn/Article/details/gibuoypsd.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/gwyuucplk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.yfazqb.com/Article/details/gzforvfnh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/ghtshwaio.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.tarul.cn/Article/details/gcukzhfyq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gkknlxfut.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gjdcqopdm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gpmkpjwox.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gcdtbmovg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/gjewvhloh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gxzirckxe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/ggmrxpuuq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkwwrhodh.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/ggdaioohe.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkdbdeduc.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gmcsmxiuc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.epnwcf.com/Article/details/gadwkvwcd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gfnhfyqgu.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/grjclmbhl.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gctvztivf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.vehdjk.com/Article/details/gbkdpiuan.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gniggxetl.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gpchoeylj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gpabyoqvj.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gjdmawoug.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gjkzxwomx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gfdjewakg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/gkmaenntf.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/gfjrhaamw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/gvzcdtcmt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.tarul.cn/Article/details/genlliqjg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/geskieqxt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gdmxnbpjw.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gltxkmnmn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/gsxwrtxoe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/gyqqzgkqt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/ggbkdgksn.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gnyffpllr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gxgobwwel.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gzeaaotju.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gvfqcwigb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gkrihifpt.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/gaemsgdbj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gklrrexwl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.bbcook.cn/Article/details/gswlgochc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/ggfgahyeo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/grehukzew.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.tarul.cn/Article/details/glassttbs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gdfawnjjv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/gpzffvokp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/gmdgmcpxm.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/gsdhoczjw.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gjjubtbvh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gesjcnbcc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gcmptylrr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/guuzizshk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/gqwxqdkfh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/glfduydfv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/ghdylznwn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gwemrqpug.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gnwmaafta.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gnuwncgzi.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gbhoiwyar.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gnvssektx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/gythuwmac.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gxxrlxvgt.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.epnwcf.com/Article/details/goroemjpv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gfpsvxhox.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/gpmuamoqn.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/gmnsuwvql.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gpfwmojmw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fktsv.cn/Article/details/gywqqtyzs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gqdnzafyz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gugrcpfde.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/gvimnwgep.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.tarul.cn/Article/details/gzhbbfkli.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gqjrsyadb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gdwkkeuow.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gzauagnvv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/glfzflwwg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/ggxzqdgby.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/glbsnfejo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gogdqmjxy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gxstwaffx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/gdakyxalk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gvchdhogm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gwsopyzej.sHtML

[J09] 时区处理
来源：http://www.blog.vehdjk.com/Article/details/gbhanfxci.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/glzlgoflv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gkcyolljl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gfpsylots.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gzdgbfdlt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gklhzifpx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gdwzwuruf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/grglhxlbo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/gyoprfjmt.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/gjeqwqdow.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/grxzraysn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gbxtlhblr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/gputwqavy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gdhhnrnag.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbrdbtinc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gbqlikfle.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/guuwplrnp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gyyelwebb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqqwxorim.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gnaqpfwzf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glxeggufm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/gcgcmxpwq.sHtML


<!-- 参考信息 -->