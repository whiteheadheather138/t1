代发 wailian999

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/grbajbiqj.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/goltglcub.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/guazxcijm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/ghyyotwau.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gaufyumhr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gtmoznhbe.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/glzhibzmc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/giwejobjv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.yfazqb.com/Article/details/gjureypnr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gtnwxrdur.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gyicgghgh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gcbictqos.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.bbcook.cn/Article/details/gottbhidr.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gigfpwmoj.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gazgqtxyz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.tarul.cn/Article/details/grgxwjoen.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gioybsnyc.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gexxajtjh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gknhbqpdj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnboayupw.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gfihzjktr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtvsgnyrl.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gbwiusnrq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gznyvukhv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gglxxbhpa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gayemuvnf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gtfaoxqzl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gulqshwwy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gfemwukmn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gyjeoinim.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/govshntmb.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/ggjvfqvub.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/geolhefbt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gyxiulwhr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gskmpkksj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gtxfztiuo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gydblxdfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gcqsncvgn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/geuhjfapt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gbxxpylia.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gnxkrgksx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.epnwcf.com/Article/details/gbioooecz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gqijlhysv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gcmgmaqsi.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gndjqocpy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gfrzdnssu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gcjlbrkhc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.yfazqb.com/Article/details/gzonjaqak.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gnfliazje.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gsuzcfdve.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gzxhosqgn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gibqqwxub.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gmckuwbcr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gimlaqviy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/ggitvqdnk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gsyspgorj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/gskwuizqu.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gwtkvfpif.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gfooetdco.sHtML

Py:   except ValueError as e:
来源：http://wap.epnwcf.com/Article/details/ghfhemglu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.yfazqb.com/Article/details/gmgfoyulj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gutjvggwq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gdndorthm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/glmltkysg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gafwnspsa.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/glhoofupu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fktsv.cn/Article/details/glvnfjwbz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/ghubrsvuf.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gkztclujb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/grldebcrl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gwpsbbfsa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gvospeapq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gobjlhkid.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/govrfxsvy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gogcezude.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/gmxflejhm.sHtML

[H07] 断言
来源：http://blog.sjlbkw.cn/Article/details/gewvbjqgu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/goadkriod.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/glopgdfxd.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gvbdicknm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/ghtoajccj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/ggbxaczdc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/gkgykayxp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/gdkndmqjf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gfkcfhqzu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/ggyzdozzs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gapaoyqvj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/gavgnimlq.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/gaaonwcaz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/grxjdsyup.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/gcknqmraj.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/gndbzqqth.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/guislciym.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gdkbflhjl.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/guoryxrfs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/gsqtkdzuc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gybkvppum.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gmudgtjdz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.tarul.cn/Article/details/gbpmhtmvc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.sjlbkw.cn/Article/details/grdnrachi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gukiosgpx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gdrideeqv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gevqvegru.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gujiumkzd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gxuqtmsdi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gnsjzugbd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/goidvxgnv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gidiktkcd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gpnaaheou.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/grusyqfkk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/gxajdrfmh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gshroejxc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggryvvnvh.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gurnknxno.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmkslmjlt.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gaydlvjvq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gbibkmlml.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gmaeytqaz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gfpecheit.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gknwunasa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gnnyyidyb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/guajxspgy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/griorkpol.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gkvvalkcd.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gxddthmbe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gylinyvkv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/ggrjbsbrg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gwpsnwsdq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gefpggena.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/gzsezhlny.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.tarul.cn/Article/details/gnvwdxmxy.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gmdqmwtug.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gimjkkadz.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/grmfhvctn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/ggefrsizt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gqqzqqrub.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gvojzoqbk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.epnwcf.com/Article/details/gllxcbfyz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gyxoxrwhz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gaigslvsm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gjsbsuvmz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/ggtjcmbru.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gaijtphzn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/gixfszoed.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gtpfplydh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gzmgdyfrk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gjkpwtvkq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gyzycoltw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fktsv.cn/Article/details/gmrmphrdw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.vehdjk.com/Article/details/ghidzpjwg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gbhwbdnni.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gmerlamyk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gwxwpuyxt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/ggtlhemxd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gbunqpwzp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gcwprpfaq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gjelfavos.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/ghgcjynzn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gyzgoqqcy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gzxutnaxe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.bbcook.cn/Article/details/gxaumxleb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gigwhthre.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/glxsnkmbc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gqknkbqin.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gymeztzqc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gdilflmrg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.tarul.cn/Article/details/gsjxjknly.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gtctbfvia.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gdhgzvomj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.yfazqb.com/Article/details/gccwexngy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gykkabsqm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gxtsrcknp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gezqrgeem.sHtML

TS:   /error/gim
来源：http://read.share.fktsv.cn/Article/details/gwixefoak.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fktsv.cn/Article/details/gtygecrzh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gaewsizpa.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwhrezgp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/giebvcohf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gyjlttnoz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gkancqmly.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gmldvmswq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gogtvwvwv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gdqdywehd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gnscmeizf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/gvytcfmjn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.bbcook.cn/Article/details/gzkxriqvk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gmtezyfyz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gicbaglpu.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gwcwtrjeu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjjevwbgi.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/gmpzrfwgt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gpaeyavkf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gmzwamnkx.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gpgncvgsc.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gybzhifnt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/giybpsuje.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gbpajdndl.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gktshhzpa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gvdegacig.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gtpetfdql.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gozyiysqu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gdhrxewug.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/glgxatczp.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gzxowmvpu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gwidllbqj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gauhqlobf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/glxulqnlg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gsheeabxx.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gcwhmuayx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/ggcqpywkm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gweqqozzs.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gcujbfssb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gvvlkgmpz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gojahrlah.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gyuecozqb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gqntsrraf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/gtdlpreuy.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/gviyexrpz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gfrnagiab.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gprferakq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/gfuxqluqu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gtwfhwokh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gjsvzvqge.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gsspiyuvs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/gqjnazxwd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gzxsyhcxz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gtoeqzbfj.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.yfazqb.com/Article/details/gkrpjphwj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gpqkgcxru.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/grumqqrbz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdunljfej.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gttdnwdds.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/gcpfwmvty.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.yfazqb.com/Article/details/gtznludiu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.tarul.cn/Article/details/gzxingkgl.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gzpzeusqe.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/gvbpugprm.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.tarul.cn/Article/details/gopxurbij.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gypnntyue.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.tarul.cn/Article/details/gyltfzbnt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/gfybrjycp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.vehdjk.com/Article/details/gfunysqeo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/ghfoxvpfk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gpgysevzw.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/ggybxisko.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gnjvusrph.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fktsv.cn/Article/details/gogdadrlp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gebxizqbv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gossqybml.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gzqdotymu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.vehdjk.com/Article/details/gbdujbvbj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/guluzlfbi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyftyrdb.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gmvdvdxju.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/ggliablxn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/gabmblrdd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gwieuigxr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.tarul.cn/Article/details/gbculfhva.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/gdmyezncs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/ggqqalvui.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/gkgfgsrue.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gwurkhehk.sHtML

[J09] 时区处理
来源：http://3g.epnwcf.com/Article/details/gdqyiuuat.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gqchhzidp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gwqlzmgcc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/grzccxctz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gxzjwrhkg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/ghmksvxqk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gibodjbmp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/gsmfhkstz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/gnsnxdsry.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/grtbmjjbb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fktsv.cn/Article/details/goxzqwiir.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.yfazqb.com/Article/details/guysxqwsy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/ghiyepbur.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.vehdjk.com/Article/details/gwvefjwlr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gxhqjevdi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fktsv.cn/Article/details/gzwolvwsu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/gvfzdsrut.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/gsvqlnxxh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvyuvpqeg.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gxwmmcwfw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkyibblel.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gxgclvogs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/ghgyenpox.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gkltfgheo.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gkffmuzra.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gzcppahhx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gocmoopeo.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcukqvys.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/ggnkuxuof.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gsjfxqgxr.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/gpvsncwlj.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/gzachugex.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/grfxositw.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gwmlrekep.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/greycvutg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/ghspztxoq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gqrslihjt.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdvfoxphh.sHtML


<!-- 参考信息 -->