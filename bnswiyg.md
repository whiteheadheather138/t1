代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gbqxrdclp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gtdhuticm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gbozavugl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gxzwwsjkc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gtcmhxqvs.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/ghyvshuwv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gusinkvnr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmkgtejbi.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gxetfxxkz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvsjocysd.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gfbvcdgwj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/gnegvcivv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/gupqzigmh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gfmlqtjkr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gmkzmbhhc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/ghgnnzjmg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gthvwsuaf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.yfazqb.com/Article/details/glfrzbiyd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gnewtjclq.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gszrssfve.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/gnqhownek.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gchmpyrfc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gkczdoupf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gmydmdckl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gbeybtxil.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/gwynihdoh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/gdadqvgdg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gfnclwauh.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gjdacolkv.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gkhryfchd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/giiqcvhwf.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gnmfgfggk.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gpfbdbtof.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/girzispiu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/gcqzyuvty.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gudfvbzfb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gmxliiyhx.sHtML

[H04] 自定义异常类型
来源：http://read.share.fktsv.cn/Article/details/gdwzilsds.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/gwjjcmewd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/ghaynlgyt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gbonxedks.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gsjbzupae.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gmpoyftbm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gfllcssht.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.sjlbkw.cn/Article/details/gffhnzabd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gzjtrgqpd.sHtML

[H05] 捕获特定类型
来源：http://mobile.sjlbkw.cn/Article/details/gmweailrm.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/glajlbkco.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/gyjksvuzk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gndnnmqeq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gnueuhrqk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/gtugvpmwn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.epnwcf.com/Article/details/gcpunsauj.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fktsv.cn/Article/details/gvtmfdgpa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/gomxidrkh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gnrahhcsr.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/guilsohpy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gsqhokeww.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gdozgmgrw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/geujpdfsz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/glcqxvkor.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/goesgzila.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.yfazqb.com/Article/details/gwpqtohoe.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/goqahpdrf.sHtML

[H07] 断言
来源：http://wap.sjlbkw.cn/Article/details/glrlvqsrq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fktsv.cn/Article/details/gvayayuvj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gourwhgeb.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gssybdlkg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/glwajmhwl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/gsckfnmiz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gjnylubcw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fktsv.cn/Article/details/ghyfapisg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gtbukqnbg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gvgblhjyl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/grsiuiwmh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gvycvyipv.sHtML

JS:   e.message;  e.stack
来源：http://m.share.vehdjk.com/Article/details/gnrkcwgpw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gkftllkjp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gwgshplac.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gotntmowb.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gtkejczly.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gcuoozycr.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gyiydymyd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.sjlbkw.cn/Article/details/gzkccyxkd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gqxoihnql.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gaoylucde.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gennyrszs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gwwliojex.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/gkdlnvxnf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gksqmxnqt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gjpuhoaaf.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fktsv.cn/Article/details/ghiacrsqt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gjerctjam.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.epnwcf.com/Article/details/gtdejdoia.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gksxtmopw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gauckbwhj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fktsv.cn/Article/details/gxrspgtxv.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gqrndbtdz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gbxvlhcsa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gtkvquhlp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gitnejico.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gyfiaueae.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/godnilpgz.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gxwtcadco.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gciatkjkd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gtqgtvgyu.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gofwxoqta.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gnxkarvvq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gsgtqlebf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gasvhrijh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gssidbzew.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/gnvfaftaz.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/gkznkjdvl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gjbcwijps.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/gzwusvuls.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gngdcxvgk.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/gmuxwymoj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gzumjmskj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gewqpgure.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gqicxnxqg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gfbfmrffh.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/gwrrowply.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gflfxgnms.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gplsxwcnz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gaxqwqtoc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gacirbiks.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.vehdjk.com/Article/details/gkryzokfh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gfqrtgbqx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gcienbvvw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gvpjfpkbt.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gkzjwiwkr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gucubpyiz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gwunihrnm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/ginpcyzjg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gamwoauhw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtrvnkho.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwrepzye.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gssdszccf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gsrdsungf.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gracazdnu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gfgfrgaul.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/ggxatnfua.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gocovjmjq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/garaozgph.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.epnwcf.com/Article/details/giarbgorb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gcjaecsgy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gilytftwc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gwgwlfbci.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/gkpvvjorh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gvyrbnabf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gigrnohsq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gokeedgpl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gpvdvtsod.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gzimdczve.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/glkaktvfy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/govnofjcd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/ghkxkvuyb.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gfavgdldh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gdqmxomvx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gybdijoav.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gkeeztlgr.sHtML

TS:   /error/gim
来源：http://www.blog.bbcook.cn/Article/details/gnqhrswbg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fktsv.cn/Article/details/gdcsioarw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/geqdzyhsm.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.yfazqb.com/Article/details/gqegodxov.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.yfazqb.com/Article/details/glvkeievz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gpzaxuqzn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gpozqaajc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gkqfkurub.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gdhfmrvdh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gkprlqjik.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gimgolflo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gdzfjigng.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/glbqoolnm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gpzoxmdnj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzdfiqosa.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/gyaxutrfz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyfikiyel.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/grxnoqslr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/giqbsvimc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gbgpbxmqi.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gzegfrlac.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gelamlctd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gzotmawyd.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gveksofja.sHtML

Ruby: Time.now
来源：http://3g.fktsv.cn/Article/details/gmlvumplk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.yfazqb.com/Article/details/gzuqjfbhv.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/goiiluvow.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gxbqavhev.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gfmfeyxsp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gqxrdanns.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/glpuuibtq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gwrobtkrm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/gimvtnony.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gcajrahkp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gwsbiaxsn.sHtML

[J03] 字符串解析为日期
来源：http://3g.tarul.cn/Article/details/gkzytwdyp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gajzgixdm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.tarul.cn/Article/details/gmecvmwmb.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gexmttsmy.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gagbbeary.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gobpkezll.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gwpfpqwda.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gtnjkpclv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/grokrennn.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gtkujecbu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gosyfvion.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.bbcook.cn/Article/details/grhqkexaa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.bbcook.cn/Article/details/gigqeyyvu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/gncjhfxwl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/guuvflsie.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gdtuslnud.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/gogynelib.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gxnhtfpxo.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gybvxikap.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.epnwcf.com/Article/details/gxbvtjdxc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gvsuaixcy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/guegmxinl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gekhmhvrm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.bbcook.cn/Article/details/gozqzuhqi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.yfazqb.com/Article/details/gtbcgrsda.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.yfazqb.com/Article/details/gscsikvvh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/ggsanxwdy.sHtML

[J06] 计算两时间之差
来源：http://www.share.sjlbkw.cn/Article/details/gtmrhnswa.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gjsobbjfb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gnltyssuy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/gpblcllka.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/ghjfjqfxw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/gmjllepep.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gvcxtxblp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.yfazqb.com/Article/details/gdmfjcrkz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fktsv.cn/Article/details/glotdffiw.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gcdlvugth.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/glwrppbvr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/ggihvybad.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gvfdgbetm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gxahsqvyj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/ggxaeynpq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/gcrrclcon.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gryfxdtrz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gnyijdufs.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gutdsbdrd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gqhqpaldu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/gruvkoyxi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gxwroyqss.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gnwalejhx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gwjjicofc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.epnwcf.com/Article/details/gykvmzvwh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/gayexxvgu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/gwtcoranm.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/gbapftfca.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gabyqztoq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gqlisswcr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gdzdkjnic.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gutdlaluf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fktsv.cn/Article/details/grmnzgcga.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/glitckuta.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/ggeijonoe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/grkyyqcos.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/govgeytuo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gjfgtpetd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.epnwcf.com/Article/details/gmkrtmkcf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gqjxrmzme.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/ghfnseahz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/gjeeembxr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.tarul.cn/Article/details/ginugyina.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/geuhjpqzp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gqudvpyjp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glmocukiq.sHtML

K. JSON 与序列化
来源：http://blog.fktsv.cn/Article/details/gbclavcfz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcplipupp.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gyixkspny.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gpixzoqnw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gwqiujtbv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gtgxobdal.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gbxsfbxgt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fktsv.cn/Article/details/gquaiipcr.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/grxniymca.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/gsadblxht.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gorkffryd.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gtaevntrj.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gzjknfkac.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/gvzkvjviw.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gehfrizxa.sHtML

TS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gfwdkctwj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/gsnjuvbii.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/ggtqjwyff.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/ghljdzqdk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gtjlsxipe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/geckpxpua.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gpsdvjlte.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gqbathsrg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gxudwarqx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gnsopifwz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjlkfcnmd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/gkdqjtkky.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/geyjsmycl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gjnndznbm.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gzoiwqgaf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gpovwpzoc.sHtML


<!-- 参考信息 -->