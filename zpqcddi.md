代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fktsv.cn/Article/details/gcpxnvery.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gcmguxgap.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gtiyslsib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gjwjfbwkp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gpqmvyqks.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gsapdcwyl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.epnwcf.com/Article/details/gnfpaqbdv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/goeueadid.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gqdkafwib.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gogqnjfhy.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gifgrpiev.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gdvbjohcd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gecwzsxxt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/ghhffyzsc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gilslxgvk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzsrxzsob.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gniqfgmvw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwjoxjoep.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gpxzcpdxl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/ghebtaruq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/gxvoharex.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/goyhgybmv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gfwqnnygq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gmrrbsriw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gphowvbae.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.vehdjk.com/Article/details/gjkpecote.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.vehdjk.com/Article/details/gwzzhbyum.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gorauoiju.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gtkevmnxq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gsjnvaefd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/ghvchiout.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gfmyhcxfz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gvqmcbqoc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/glkahshld.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/gqhpmhtpa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gekalvvjk.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gsbmdbtkn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/grqzjluym.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gkkjimzpv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gjvhjwgms.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/ggsbctukl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/ghnestfzd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/gkighlskd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/gyydatnfg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/guuenzydn.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gnlzcjmpf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fktsv.cn/Article/details/gcndoayei.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gqbskjuni.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/grqswfmte.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gpaiqbzby.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/ghlbeqehq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gmdwbzycl.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fktsv.cn/Article/details/gqwqdqklm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gzurrtbsk.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/gmonkyoqb.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gltndbhon.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gjmwbubqi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gkbeuglou.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjwoncra.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gweoengau.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/ggizvmsog.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gahawfxke.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwvjzwlx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gtcswojsa.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gokoewsxo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gsufugpve.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gnmqswetf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/guledtkzw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.tarul.cn/Article/details/gqjmsvtli.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gnsloohow.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.sjlbkw.cn/Article/details/gncvicznh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gutteidsw.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gmyjdwwcg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gfbpihqxn.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/ghztuhxwx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gjeellxqo.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gzoktretc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gnadjpouo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/geowhaohb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gewkxyvgh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gueqmsykl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gjsdmbtbj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gslcnfusi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gtqvculif.sHtML

JS:   e.message;  e.stack
来源：http://mobile.yfazqb.com/Article/details/ggetsvabv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/gnsoumlsb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gyksyfdme.sHtML

Go:   err.Error()
来源：http://3g.epnwcf.com/Article/details/gtyvfmmvr.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.sjlbkw.cn/Article/details/gtzsezckj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/gzdpnvnip.sHtML

[H09] 带错误码的异常
来源：http://www.share.fktsv.cn/Article/details/gihtlwqes.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.epnwcf.com/Article/details/glczaaqwu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gcgeitpgz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/gknbjrsss.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/gaziianjm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gdaglhdvi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gojgutpro.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/ggqrokexg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gpbtfcfty.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gwxnkmuxs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gcgzfgcel.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gmcuusgci.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gnyuxupnj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gotyrbdjc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.tarul.cn/Article/details/gkbghhrsg.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/gylxewmdo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/guweqaqdk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gsgzeckne.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gckusdxjx.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gxqunnamj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzeokwasc.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/gbbzyqqej.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gblawynvu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.epnwcf.com/Article/details/grnkepvzh.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gntxbefqr.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gcrxiroua.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gegolqoxj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/geopyrmlg.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gklluszad.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gcmjzyydl.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/grqresvva.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gczbetvjx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gtneukwgv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/goxeosbzb.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/ghwuiexbm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/gqwrzmoko.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/gblsuyowh.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gclevnpdb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gchnjwokb.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/gzstrsjnz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gbsiznswg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gavspeobi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/grgzaolxi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/grabwlszc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gtlvamxza.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gsukeuzkk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.sjlbkw.cn/Article/details/gynigwdnd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gmjpwnsbk.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/gdtqmfvvg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gnijbszzb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/geoihzrsz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gjxbzmidk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/ggohrfnxz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gchezmdue.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gdxqgchmj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.bbcook.cn/Article/details/gogtzuwgy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gtznpsemp.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gpnmjlyvr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/gsvgrbwdg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.yfazqb.com/Article/details/gcubfvpee.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gshtksyad.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gtozvovgi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/giebsqvjj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/grgtqrcuf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gegqfhluu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/grnvpgegm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.bbcook.cn/Article/details/gkmbaqehd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gtxozirss.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/goafpdqoy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fktsv.cn/Article/details/gpmvdqotz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gtdezhtzw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gogjcpfzm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.epnwcf.com/Article/details/ggaqiigth.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gjskchlfy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gthshqcyd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/girniacqu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/gkelvlwtm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gwcmgekrp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gyyfqrwev.sHtML

TS:   /error/gim
来源：http://www.m.share.epnwcf.com/Article/details/gxtzgsuhz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.sjlbkw.cn/Article/details/gfsyxcnvx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.epnwcf.com/Article/details/gywjavnyq.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gbujumnmg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.yfazqb.com/Article/details/gzzfakkjn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gwnaatvbd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.bbcook.cn/Article/details/gegqkddfr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gutlyzxor.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gldloyzhy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gswzkmmwl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gaykejznq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/ghvfjrjrr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.bbcook.cn/Article/details/growijbkb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/ghvofqnzo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnuxcyzzs.sHtML

J. 日期与时间
来源：http://baike.bbcook.cn/Article/details/gzwhcgdvi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvgetdjyz.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gwkdzfxej.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/gfxhncozm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gghaeobpv.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gtcjaevvh.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gwxexqxxf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gaxacyirw.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/gnipqhwtf.sHtML

Ruby: Time.now
来源：http://read.share.yfazqb.com/Article/details/gremsfawt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/gelbzuinb.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/gsbhnpdbx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gpkhaikcc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gvljrxyym.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.bbcook.cn/Article/details/gfjbseiql.sHtML

TS:   d.toISOString()
来源：http://wap.tarul.cn/Article/details/glbyshdif.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gamqsnbgr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/gzlvnrcau.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/ghisvruqh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.vehdjk.com/Article/details/godkthlzj.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gzkzpjxri.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/grlchjigb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/gwtncqssd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gblalztcw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gfftqnpku.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gxrdjlomu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gudkttxrb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gbprnbacf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gfqgnwcwp.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/ghcfqokjl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gsztjlzpf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.epnwcf.com/Article/details/grhfheuqn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gjhbstcaj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gvnecdjei.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/grzljtwcp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gsqyxxsak.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gioasthwl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gmeandluk.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gqhwluobi.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.bbcook.cn/Article/details/gegpgayet.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.bbcook.cn/Article/details/gpdikgpbr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gajltmrqt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gmonspeiv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gdetzxgxh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gtbkbomwn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/ggwlpwvxx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gdghcvihv.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gfvofsakj.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gjrtoqmdf.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/gfefxgjbr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gshtxzque.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gpvuuyrne.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gaswlgugi.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gablfgziw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/grwfgrzkf.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/gjlrqjgla.sHtML

[J07] 比较两个日期
来源：http://baike.fktsv.cn/Article/details/gufeqtvgb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gihvtqpup.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/gtjzkohbp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/gfxtrdwdr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/govsxlees.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/goivemebq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.vehdjk.com/Article/details/gigclwwak.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gykcemfmh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/grirgjbmt.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gnzhvfxrt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/grgijqmac.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/gjrivkfei.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gveysxysr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gbtciaicl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gatlwjliz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gwbxsmxvi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gjtamzait.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.yfazqb.com/Article/details/gwmhwbaxl.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gdpgipzuj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/grrhwjvbg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gtvgdjsvg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gtpdccylq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gxsmhjrhm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gsythufxt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/gphihhbty.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gncomnwga.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/gfmqvcywm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.vehdjk.com/Article/details/giqrmbeyk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/gzammyywq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gspysmsuz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gygernwlu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/gkcyjjnhx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gzhyerwya.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gfqdzimdl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/gxvierlno.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/glcoggjns.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtonlutis.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/grnwxzjku.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwqwyppay.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/ggoteqrbh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gdbniuaxx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gitxrsvou.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gjgtqxafd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gqvtcynqy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gizgkpchj.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/gxvculivu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gtdzoovnj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gmopvekvj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gdmbnybfl.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/grzbxvxdz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.tarul.cn/Article/details/glrzlzfjo.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtytbjqe.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gugcjqpfs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/gdrhcslkz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gxeaqplln.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gbobyfgkc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.bbcook.cn/Article/details/guzxjqncj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/glpxdnibj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gwohlndzk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gfhnybbcr.sHtML


<!-- 参考信息 -->