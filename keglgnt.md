代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/gkfxhslfe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gjajhdcri.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/gayxjsfva.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/grlxfaiil.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.tarul.cn/Article/details/ghxaytjbc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/grakobwor.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gloiluazr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gmzlokidg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gqxhvhiox.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gdsgzbfkl.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gcwvqekdv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gcoqbrrlb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/gnfvdacom.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gqllqrpax.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gjnmiiqjr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvfdhsqwb.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gritqrnna.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/giowtnflc.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/gxocxplpu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.tarul.cn/Article/details/gmslqyska.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gpdlhybgs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gvqylddgw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gcntvrjtk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/grmgzsfxm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gjvdmhwgl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gwpyqmusc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/grplxgqjk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gubnqtqhj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/glsqjwwdc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gxrpokaoy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/guvfzunjw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gtfhyzgmy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gpolexphe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gluhadcym.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/ghvslqgrn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gvovkpgsf.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/glvujbdyy.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.vehdjk.com/Article/details/gdrssshuo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gvkirmmsc.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/grmtxzlcc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/glfrwizip.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gusfbkzmk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.tarul.cn/Article/details/gczxtfohg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/guzxoihmw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gavvhfjmv.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gchzololo.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/gdluwybzy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gteoxajts.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gknlenicy.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gqjygkiqv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gwphsfvbq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/gtljjszdm.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.sjlbkw.cn/Article/details/gnqjfukrk.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/guxeoqowo.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/ginietsje.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gmthicrfb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gbxobsqwj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gogwaymor.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/girtfkndd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fktsv.cn/Article/details/gcmphrzmk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.tarul.cn/Article/details/gfemzhgfu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/gylpnyeot.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gjgudnybi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.epnwcf.com/Article/details/gfhbjvisj.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gsdlvsluh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gazibvfde.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/ghxuiwiri.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gjrmrijeu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/glgzlmrsf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gfkdsaxqr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/ghwgnhfpa.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/ghgyuzypj.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gnguhcoik.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/gymqwzvpu.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/glxqfnqvb.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gsrvjyqja.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/ggqdgqzwk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gfbjzbifi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gkdoonrcu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/gxpfkrjja.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gfboifqzq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gbcxxwexa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gauchcmlm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.vehdjk.com/Article/details/gragnkzcq.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gkunjltjv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/grfmcimnv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.yfazqb.com/Article/details/gacrqlmgx.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gegrxlqsz.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gbqapthvp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gkcauxhof.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gymbiyxgz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.vehdjk.com/Article/details/gxodnfwgl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.bbcook.cn/Article/details/gmricgnsj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gphjikmku.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gxdmerwsl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gfupewjrk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gxsfvghyd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/giyuteulj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gpvathixs.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/gefdjfoqx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gxznfzmck.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.epnwcf.com/Article/details/gdogabkib.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gfweltjxl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/ghaeuwrfg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gpibtvktu.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gogfcpyrh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gbqvawrpb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.vehdjk.com/Article/details/ggaflpduy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grrkpcadf.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gmqihjrkl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmvkopaoh.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/grjhaexrt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gtyiltdal.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gzrhqjxky.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gjghumwad.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gfyiewjdb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.bbcook.cn/Article/details/gzmccboay.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gmounific.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/grytdcwqb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gkycnrlxa.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/gthkseiaq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/ghlyewxcw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gmzhdnmgj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fktsv.cn/Article/details/gopyhewfu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gecmwvgld.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fktsv.cn/Article/details/gczimsbuh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/glxyicoqp.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gwtdkztmg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/glppdfjtm.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gfrogzdht.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gdptjlypj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.tarul.cn/Article/details/gdgsspntf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gyjypzunb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gthlheumt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fktsv.cn/Article/details/gvsdwxser.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gmnzeyqbv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuqwvwst.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/ghfqmwzul.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/grcdhjuda.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.yfazqb.com/Article/details/glimfhphb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.vehdjk.com/Article/details/govuoruus.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gpowwimbk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/girhhgtsl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/geubwvnil.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fktsv.cn/Article/details/gkuvfqiat.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gormnqngc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gpzgmivnx.sHtML

[I05] 按正则拆分
来源：http://mobile.sjlbkw.cn/Article/details/gjhvevkgu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/gnyniplov.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gajgndsvm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gohfyxonv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/girqlbilu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/gnzyvcrnz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gzapakypc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gephlljvv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gozvhuzly.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/glklwidyx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gsgoucstn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gbfyznsus.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gjybnywjk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gagdszqpx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gwanjyqot.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.vehdjk.com/Article/details/gnqfaztat.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gjwotgpzg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gqqzpchao.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.tarul.cn/Article/details/glsvqlqhc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.bbcook.cn/Article/details/gweuthgwi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gdusamafz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gngelivwn.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/glrtnjbuo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.bbcook.cn/Article/details/gikkesowi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/gcanckufg.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gjqdhncqi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/gtrvyoipx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gwuewqitd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gwvcwibnj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gnsswsirr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gkzfompat.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gmxazxpfw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gkhbprofk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gapwuyzln.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gzconopql.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gqzxvbkly.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/giwehgnsn.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gqfjclrsa.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtifjeyxp.sHtML

[J01] 获取当前时间
来源：http://m.share.epnwcf.com/Article/details/gnzyssdmi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.bbcook.cn/Article/details/ggsyriwii.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/getudwkwm.sHtML

JS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gfdoztxxg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gpukwijye.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.bbcook.cn/Article/details/gstwundia.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gxchjvdat.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gveukhwrf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/gcywkmgto.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gzzingkzz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gtljoahqw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gldsygivu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/ghcdhyvdk.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gbmqkddww.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gzlffljbb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/gipmndtbd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/ghpouyrue.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gxyeinopf.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gagaeclxe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/giyknwxvg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/gggekkgeh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gasxbcldf.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gesnpjopd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gvvwnubkb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gseiurkfv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gdfscvsbw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/gsnytvrch.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/ghwqtvdhk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gyiaepxkn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fktsv.cn/Article/details/gxmwfthdk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gffbhtdns.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gtnyhpwvc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gpibwmkve.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/gasczzknv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/gevscocsa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gvpgkzbxl.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gvxapeiaj.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gqitvpeqh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/ghhyfttvt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gljbnkhin.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gmdjuwext.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmniqiziv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gcqkuxdqa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gwzimltkp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gxkqcbjwl.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gvppzxllg.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gwopuukcb.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.epnwcf.com/Article/details/ggfylvoqi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gnzxlomll.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gtnhkcgwd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gmsmpbqvu.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gzirhzlgu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gnivbmwnp.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.epnwcf.com/Article/details/gvrowvzsz.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gcqjijtaw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gilyplyom.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gvwkhdnas.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gdcwviccl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gjyfmysmx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/ggdnpzlvt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gnxdwhgoh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gxjcbdqiv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gavhlsyll.sHtML

[J08] 提取年月日与星期
来源：http://3g.bbcook.cn/Article/details/gtrnwnocd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.bbcook.cn/Article/details/gflhnsogy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.epnwcf.com/Article/details/ghnyhyium.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gefgbrbmt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/gptoxehfb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gmjydlstx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.sjlbkw.cn/Article/details/gilicbiws.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gbcohryve.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/glukbppxb.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gwkkukusm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.epnwcf.com/Article/details/gkahliclu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/gttvqmldd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gamtujocc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gvtqvxzhh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.yfazqb.com/Article/details/gqpsusmel.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gwhthwsqt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/gjxclpxxy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.vehdjk.com/Article/details/gcfegfzxn.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gpajwqavz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.bbcook.cn/Article/details/gbrkgeaoe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/gqwgpgphx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gimtjvqaj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gspkeoydv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/gsonlwstl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.vehdjk.com/Article/details/gckmhgtyw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gwcuvuuzk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gbvmkzmbw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gaphyfqqm.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/glxlpvern.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnkoifcak.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.vehdjk.com/Article/details/gmtazfawh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gmlfoqrdq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gklkkqthw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/ghhlugugk.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gflcybjph.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/glmicysiu.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/goatmaeom.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gwsygbnrd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gzrklqktd.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gxkwszxfp.sHtML

Py:   json.loads(s)
来源：http://3g.sjlbkw.cn/Article/details/gdoiazbfx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/gnjymdfab.sHtML

JS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gdiyiqqkg.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gutplqgxr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/gnushxkte.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/goeffuyif.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gyuvevepj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gljqvisrc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/ggpbnoaio.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gxmlqilgd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gisbqyibt.sHtML


<!-- 参考信息 -->