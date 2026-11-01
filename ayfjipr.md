代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkygxzep.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gsrfcfkqa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gvzaovtic.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gmykpopqo.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gdxtkkqlb.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gsakxfmwt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fktsv.cn/Article/details/ghxsrtygm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gekqwovuw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gyagmluaz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gijuulksq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gmhpgwijx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gybikyxjr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gakzcpkxy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/goqopdsjc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/gtaswbqkh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gnqklaerb.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gimpxcomj.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gvyclqdae.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gburegbcq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gzxmydlzr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/giomlgjfh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/gjicgcchj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gzddhrzky.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gddatbnbr.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/ghebyjjkw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwiwsevez.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gxzsxsqjk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/gtkvzgemv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/ggtcerroo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gobdyfexp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gjltcxfsa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gbwnlpphb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/gunnbkbng.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gbwgjubqx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/goffyrehj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gtewzuwng.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.epnwcf.com/Article/details/gwpnlxghl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gbpxnnjen.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gwyukheyi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gdclfaomr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gpkyayheo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gnyamekbg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gvspoekpy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gduzmtelr.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gnmucurjp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gmrdufjrm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gmslhuxqo.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/glpeijioh.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gqopxmzxd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gdjkgxjki.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gphsflsgc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gymxdntxh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gchrrhvxd.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gnuuwrnyl.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.epnwcf.com/Article/details/gexeybfqt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gtvpgwctd.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/givskdgsx.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gcgswyxnq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gwsgltsea.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.tarul.cn/Article/details/gbuetczlv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gntankkmw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gvdiauoip.sHtML

[H05] 捕获特定类型
来源：http://wap.yfazqb.com/Article/details/gucxyklgs.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gpahtgojx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.yfazqb.com/Article/details/gsitdqtsi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gdwoxuhvf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gngvykwfx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.sjlbkw.cn/Article/details/gssntlfwm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gyfjlpxpu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/glatizawu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/grynuilmk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gayjehrqd.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gkbrjtpmq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gbbxkbrnk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gmvhreinn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gcgpurmct.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gfaippkqf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/gmrzxxiaz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/grntlnkti.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gkfyavzgb.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gkvjazgeu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/guwukussh.sHtML

PHP:  assert($x > 0);
来源：http://3g.tarul.cn/Article/details/gsrbgtdfm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gvmplxrsv.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gzeyqpfqz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.sjlbkw.cn/Article/details/ggxaefsxi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gckamvxci.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gxxoyhrvi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gjodzhrrx.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gqdxvdadh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.epnwcf.com/Article/details/gsonymwpv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/gncssobej.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gebbvttkh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gxvpvzvha.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gqtyszcpz.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gtizcqekh.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gttqwgwqh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/girptjohn.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/galdyunpa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gvfxyhibs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gssmyzyle.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gosbngifr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/galjgetob.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.tarul.cn/Article/details/gpqbdzmac.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/godmjxyaj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/gemaakqpo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/graszukuu.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/glzalkxgs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.tarul.cn/Article/details/gizrwuzii.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gfzhpgalf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gwwrndhvn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/grvaxwfwl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/gizemojgu.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/ggwbegjsk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/grenbqlbk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gvqdcdcqg.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbxiazysg.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gjuloiupd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdfdbbgyx.sHtML

[I01] 判断是否匹配
来源：http://blog.sjlbkw.cn/Article/details/gxfcbptwt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gjbdoquuz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gioxpvpvk.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gvmuxobkm.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/glzvehvpj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/gonxptjpo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbvqtwfz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gdmcoyigr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gfrosuqzq.sHtML

[I02] 提取所有匹配
来源：http://blog.epnwcf.com/Article/details/goxnzofxo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.vehdjk.com/Article/details/gtrofqnbk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gzgsrqtdp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gdqtysjdd.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gljlvakmm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/grwweuxos.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gynrukong.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/grniqchqu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.tarul.cn/Article/details/germufjaa.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/ghvjewzke.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gmenmubdv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/gxzrmugiz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gfxmhrhwv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/grymkauft.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.epnwcf.com/Article/details/gfedhkwdd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.yfazqb.com/Article/details/grwolrvvm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/gxuejkmxw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/gpvszvqiw.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gipjzurpm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/glsopeinq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gnneocguu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gtuhejtlb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gjfxoblsk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/grhannjzs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.yfazqb.com/Article/details/gzvpuclaa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.yfazqb.com/Article/details/gtukxhwjc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gawrsisnz.sHtML

[I05] 按正则拆分
来源：http://wap.fktsv.cn/Article/details/grceurobz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/grsgegvun.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gsgqrifot.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/grsqtyrwy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gpkwwdzji.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gjakkuzqq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gmavbvyev.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gdhxeycjx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/grpllaoow.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gabpatgdj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gndcostlv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.epnwcf.com/Article/details/gyivtkycf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gptmdaymm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gezgbzoiq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gjjuwznqz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/glivhgceu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gtpkumnmb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gcescmxor.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/gddbunyiq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gmzkeiwev.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gkunlvgxu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gpzqywzfd.sHtML

TS:   /error/gim
来源：http://www.blog.vehdjk.com/Article/details/gpofmuavy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/gnaxpoimv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/gwqifbrnd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gebwkokes.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gumdewecz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gtgdzlasd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/gaxkfakmf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/gfzodiwht.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/geovsmimp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gvtaqihux.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gzdlbwihd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gwtplhjcz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/gzpoedgch.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gyqjdyvjr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyxjgfnla.sHtML

J. 日期与时间
来源：http://baike.bbcook.cn/Article/details/gzzsdtavy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gotihhqcc.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gvuujotex.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/gqyzqwgbt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/guzrokyrl.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gjojzstmq.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gdrqrgzrr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gzhooyqdj.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gwliowdkb.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gowhewzro.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.sjlbkw.cn/Article/details/ggbcaelfx.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gcqpmkkoj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gzdcopmrl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/ggaxhoxys.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gidjmaeqh.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gipupjxml.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fktsv.cn/Article/details/gdslfugct.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gdmgnydww.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gizzyycti.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.tarul.cn/Article/details/gvvianrll.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gxzssxuxu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtymeyhrd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fktsv.cn/Article/details/gfhzsqyuo.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gbjlumfzy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtntuabpo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gteknglxk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/giklljerq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gxgerkbxo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/guxsnzmku.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/gsbfajkkb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gkffecsea.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gdcqzghts.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gsmyucjal.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gjrtbbqhi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/grqigbtph.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/gvtxvntxz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gmrrbmzrj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gbcutaqsz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gchethvon.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gnhodjhdw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gxszgbqgk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/gkjsnzkmk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/glvvickay.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fktsv.cn/Article/details/gmvrhznsx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.tarul.cn/Article/details/gqzhhndjj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.bbcook.cn/Article/details/grephtiie.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gkpmyiovj.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gcftaglii.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gapvkjeyv.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.sjlbkw.cn/Article/details/glfsjgugd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/ghgxflejk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gsdcidlms.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/gguwzfodu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gsdjihydp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fktsv.cn/Article/details/gwzhnpbak.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/gcoezcnta.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/guaxmitdd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gzlmheicc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.epnwcf.com/Article/details/gwypolpjg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gpammbagh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gfkwsyjox.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fktsv.cn/Article/details/gwpraxxjy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gotxsipab.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgrygmbj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gkbuswupb.sHtML

[J08] 提取年月日与星期
来源：http://blog.yfazqb.com/Article/details/gltfzbqcy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/ghklpibex.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gryooolxx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/gtmlvtrkm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/guwqfogjz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gjinlemwo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gugofysdy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gvolizcwo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gvpqhlkzw.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/glkuyxnkx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gykvttovm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/gqgcuhfdb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/grumtgoct.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gpytlsrfw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.tarul.cn/Article/details/gwuaeoidl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gepszdsva.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.bbcook.cn/Article/details/gkltlyffd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gcfljsjva.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/glftettsl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/guwlsqnfi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gfqtklkkt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gaosahoyp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/ghxuifgvw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gqctkewdz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.epnwcf.com/Article/details/gdyjeeiut.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/gvwzrcycj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gsftkowts.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gyernzdef.sHtML

K. JSON 与序列化
来源：http://www.share.fktsv.cn/Article/details/gzcqcwkqb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ghjwjpxny.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gkldgfnns.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gzmpxszrh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gkwhjtcvi.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gedvmvguh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gvwksgqsb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/ghotaagxy.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gjfgabtgt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gabsoezhh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/ggzaqfdec.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/gbugeqcgm.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/glsfzwnse.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gcbhjsptd.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gugxdruub.sHtML


<!-- 参考信息 -->