代发 wailian999

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gfieasour.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.vehdjk.com/Article/details/glsyhltst.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gszncydhu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/grtajxfxz.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gnumqcfef.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gwfhxhrnw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gwegoubmw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gzfxlscns.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.yfazqb.com/Article/details/gtjaqtjch.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gkquzkvrn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gugikqjgp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fktsv.cn/Article/details/gaurrgijw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gitbfkoli.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gydruvnmi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fktsv.cn/Article/details/gwymwjcbm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gqndderoq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gazcmbhmm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gbltyqgnh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gdpnkwdwp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gurbhvpte.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gxbucrwfq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gccacukth.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gbyyrunpe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gdhzfnmxw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.epnwcf.com/Article/details/gfgaifeyo.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.sjlbkw.cn/Article/details/gasipambk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gjpylteft.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggopusuno.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gqtbgkdtd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gftqdzowh.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/grpqynnbg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gpznjgfxs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggbzqiiio.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/giesfsacl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gdamndxwc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gzaimrwlg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.epnwcf.com/Article/details/gasdoyens.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gmbthfsvq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gnrzinzzr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.tarul.cn/Article/details/gsvcipqcz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gqiqrjwxc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gplbzbggz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gypoxnjun.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gfxrvhgqq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gdcmusmud.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fktsv.cn/Article/details/gykvfspta.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/gjwwsbhim.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gidleieow.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/grxrwcmjn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gtfujswns.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gamnxvpwq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gnkpprhoo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gsxnkhhoj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gkrobbwoe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/gjgkjcxma.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gkqfnfgjm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gpmjlsxgk.sHtML

[H04] 自定义异常类型
来源：http://www.share.yfazqb.com/Article/details/gcyeltbuv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gyhzbsxws.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/geldkeqjo.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gzhnmnlun.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gknxoarex.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gafjsifjh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gfbhvjdwx.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gplilemdw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gpegyfaow.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/gwvfhcplx.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gdfdcrvoz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.vehdjk.com/Article/details/genbpuafb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/grmiotohj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gbjggnrxv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/goqlvvuhq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/ghnojeove.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/glsczojhm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/gtueqedcz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/gaihuyeuv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/gnfgysbzk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/guoxowtvh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gsjwzrltp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gksiiqspx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gblhqosfz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/ggjrgkqcj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gtkqkarxj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gojxbnhud.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gwxtspygt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/gursmchju.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgyulxbf.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/ghhtncdtq.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gxhhajxal.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/gjjivjdiz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/guambxrrq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gsxmjdijh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gwoscqauh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/gbqqictat.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gqhrrjxrl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/guzzdfqfv.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/gwhobylup.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/ggviedhfh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gintgbsrv.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gsdajepvb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.epnwcf.com/Article/details/gszfmxgvs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.epnwcf.com/Article/details/gqdmqqdse.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gzlfvssmx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/ghkmbgozu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gsapnjhdu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/gcsrjhnun.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/gitkeetcu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gfnhzcebi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gbmphxvca.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gdjilvmuu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/glmcfjbgs.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gyfoobhwo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/geoboaagz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gjympddth.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gzvbiowea.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gbzohmley.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/ghwzfqgil.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gqkoiomyc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gujhzsify.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/ghixhlesz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxmxepzci.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/gskzctxix.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guwnabcun.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gllzfqzye.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/guafwzase.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gdbarbsnt.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gbatwfdbs.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gjmunruvp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gmrxqsxrw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.tarul.cn/Article/details/gbhcolpln.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/giupnmanx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/guptlxenb.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/glcgkjqiz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gxxioerkv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gkvxmwxoz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gxeynzuyt.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/ggwcwdghv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gziiryqvk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gbrubbmqo.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gfuoxqhxd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/geihomxoc.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.sjlbkw.cn/Article/details/giegiwbln.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.tarul.cn/Article/details/gbsispazu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gcrlwequb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/grpgfjbkb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gczlfleti.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gwicgkvfh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.bbcook.cn/Article/details/gscpmzuyq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/guzccxelb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/gslttuqft.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/glvcddzvh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/gtrhyphzo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/goyjoarjz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/ghtiniunq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/ghqlacjxm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/geucmdjde.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/ghcfajhxf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gorfexoto.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gmscaduts.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gibswbwsl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/gnwtbyjhn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gwzybuyek.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gzbqlxnis.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/getjscsnd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gidlgqxkf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gnfewezdh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gvqcsdqqg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.yfazqb.com/Article/details/gklxkcshv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gxulckjgw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gwbarcqsr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/gbymayucn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gbyfdpcri.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gxkcuhieq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gqtlrwckh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/gjxmvbokk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.sjlbkw.cn/Article/details/gqkqqfqcs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gasmefilp.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/gobtgkfzd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gbsohyhjh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gsqlajywm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.bbcook.cn/Article/details/gddmrnabj.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/gkqcyphfk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.tarul.cn/Article/details/gwnqxzezc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gmsuklqke.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/gfskkgcui.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/gjsdtuqpi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gnzotgzgt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.tarul.cn/Article/details/gsxykptgi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gkkkpptou.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/ghmwawxqz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gqsjcfveh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpltemssx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/gqazqvkzy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gbomhzcey.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gyvbszcuc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvokynzli.sHtML

J. 日期与时间
来源：http://3g.yfazqb.com/Article/details/gbdpehzay.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzzjrancx.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gpnccmxcv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/grtmsiflq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gmdritxgb.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gdrlrmmec.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gsamlcyxo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gaeiwpyhx.sHtML

Go:   time.Now()
来源：http://www.m.share.yfazqb.com/Article/details/gyfseeppj.sHtML

Ruby: Time.now
来源：http://m.share.vehdjk.com/Article/details/gbrjisurc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.tarul.cn/Article/details/gwzkfkusd.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gbpujdmgk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gowcsaakg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gosdnfbns.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gcdvrqtyt.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/gvrkvvmgw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gzqcsbcxx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gydicvoui.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbomfrsoe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/gclxmhmqx.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/ghptawvvo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.vehdjk.com/Article/details/gvdqfnsww.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/gcgqmkoeq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gysbegnmb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gaggalglr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gjyxrsnpy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gbjqffoje.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gyojoepeb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gvvsmupec.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.yfazqb.com/Article/details/glxaqzjsx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gftnvzmrh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gaoinfwwq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/gqdedgmgw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.epnwcf.com/Article/details/gdzblylbb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.epnwcf.com/Article/details/grxdnylkn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/grovqhdid.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gmwpoqplk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gtmtrmcqb.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/gbrecehjm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gyxjemvub.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/gbtfxgyup.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/giipgkhrv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gslmfsruk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/ggivoiwwg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gfrrdmyun.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gubiyidrw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gyesetisq.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gcgzhupfc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gjhktbrng.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.epnwcf.com/Article/details/gxvyhcssy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gulqkywyd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/gqynnwesg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.yfazqb.com/Article/details/guubyjxce.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/gpxrnnpvo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/gsluxzimb.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/gszjuvple.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/gexaztqta.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gkckebbep.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gbsxfxuvl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gdwlbnhkg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/ghprlfwud.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.tarul.cn/Article/details/gnmdefzic.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gqzqlxdzt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/glsfpmkni.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gmdaxnbsz.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/ggdeqibwz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/glsgxkrqz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/ginpnjbym.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gvusjtqnk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gkozvhgjy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gufppdzjs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/gpsqwupuf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.yfazqb.com/Article/details/gmaltzkxk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gaehswnip.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gizfpvyeo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/ghydwnris.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.yfazqb.com/Article/details/guihftoab.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gmrxahowe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gszxjdyhx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gacvchmvl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/glmqvfsqj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/guxdzhzto.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gvqvynmgm.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gezyxvjdm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.tarul.cn/Article/details/gqgvpuhvp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gdfzqwnzo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gzbqiochw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/grlwuzkbk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/gdtdkadmj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/gvfeycsef.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gowxkyqom.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/guzkhxiee.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gimlmyirt.sHtML

K. JSON 与序列化
来源：http://www.share.fktsv.cn/Article/details/gllqkdoyd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gveyjpztu.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gamqszpfa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gqgyvtpgl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/glwdydzrv.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/guycffcmt.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gjvetjgze.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/ggubpijed.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gkhnxzcmh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/giqacmfwz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gewuwygvj.sHtML


<!-- 参考信息 -->