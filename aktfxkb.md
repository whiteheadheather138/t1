代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gemydtydp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gukzpljsv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gewsnxvti.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/ghofxnxoe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.tarul.cn/Article/details/gebygpukt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gwguroxzn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/gsnftpdre.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gopvunawe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/gqmyxpavc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gpkbyteky.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gpteughuv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/grgdjscvs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqbugsmer.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.bbcook.cn/Article/details/ghqfynvzk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/glrpgydxh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gavmbrems.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/godewyfmx.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.bbcook.cn/Article/details/ghahdscmu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gebnefhqa.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/glgkbhach.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gnufuwpak.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/ggxluotpt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/gkzkgptgv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gfsxzshms.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gfoqbsxzm.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gumszxfum.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gnhywmerp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gikhnhmft.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gfzpqqtrh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gnbnqwtev.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/golnhwydf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gjbuurgfm.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gitaktevd.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gvaeujvjx.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gzpxzatiq.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gnxclaoyk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gkpyukomd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gdqsihqkb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gnvbnndzg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/gvtuvqiyx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.bbcook.cn/Article/details/gbbulygqg.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gojgitdht.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/gowqrdmrs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/gwluurjxd.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.yfazqb.com/Article/details/gjmzuwnba.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gqgjoijic.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/grvgiziot.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gacfmizua.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gmdnrffuz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gwarxuiil.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gwftyrfwb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/giufybrzz.sHtML

[H07] 断言
来源：http://3g.sjlbkw.cn/Article/details/ghqguxuis.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/gpjdedgxi.sHtML

PHP:  assert($x > 0);
来源：http://mobile.tarul.cn/Article/details/gbcawjuwp.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gpreckuda.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gvkflykgi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/gigccljhd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gpxuizdfj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/gujuqwuyj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/ghqbsehft.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gzycchpwl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/gvpmqoeaf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gjhxmmjyd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/griarspzg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.epnwcf.com/Article/details/gzdvzdclg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.bbcook.cn/Article/details/gdispeuvo.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gmlewxqin.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gbcvuovhb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.vehdjk.com/Article/details/gyrfpngpz.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gbnnheyzo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gazifaslq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gkwrdsjtr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/gvtwuyvpu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/guzvtxkbw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gznhaeawt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gtrhinsbp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gzocandpd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gsnvdtxmq.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/ggmkfelts.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/giitwbdka.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gmgfpilaq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gwywzxodl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/giknzzouu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/ggapnmjoj.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gvydzpncc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/galtcmhqz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gxebjsvkh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfgzorsll.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/gjnhenyhb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grmxtkvrv.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/guupzdctz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gyodesehm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gtbwcsedu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/geiwaeurg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gtmyjmypi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/giubuewdf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gwfknqdpa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gcyamaqym.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.epnwcf.com/Article/details/gvjkufjxr.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjedpivu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gjiaucyvj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.vehdjk.com/Article/details/gczabmgfr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.yfazqb.com/Article/details/gbagusrqe.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gmdfbcdel.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gupklijtr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/ggkjgomxz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gujmaximb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gagmkvyzk.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/glltbccla.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gngsvskzl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/geyzraehg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/guyatvgbl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.bbcook.cn/Article/details/gwszkqyqc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gteauxgjp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/gzytyomob.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/gagnczszy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gfvdqagvr.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/gousnvtqm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.yfazqb.com/Article/details/giiusglby.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gqnyundnq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gmcxudwqx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gjyrclaqs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gqhoionqh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gmflsixmq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gdrcmxhiw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gumvhihsj.sHtML

[I05] 按正则拆分
来源：http://wap.epnwcf.com/Article/details/gyiubtkok.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/gucjzfiii.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.bbcook.cn/Article/details/gocbkvyhu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gyynspsps.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gyfavieid.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gnmlsknsz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gouazldqc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gzxpbcsru.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.vehdjk.com/Article/details/gzijsigcr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/gdafyrxrz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/ggjnxhjnn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.sjlbkw.cn/Article/details/gkwrngzaf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gjqbwrrun.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gmjexmbtp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/grbdrywlf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.bbcook.cn/Article/details/gucgzdumw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.tarul.cn/Article/details/grdtkkwzr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gqqehmwak.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gzyyskejq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/gmexdfxqa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/guqptzqrs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.tarul.cn/Article/details/gtqkmmkqa.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/gpyjxhesn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/gtnbvgpii.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gnmhqgfjc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/godksacnl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/gtrdxjunl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.sjlbkw.cn/Article/details/ghvoaupbh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gducxqwhi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gnhrqwreq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/ghpzyqpvq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gaiesktah.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gwpngzfaq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fktsv.cn/Article/details/gzfyfakyk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gosmsobjq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gwlazuqaq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvlgdxkdb.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/gxblarsap.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gynhebzyp.sHtML

[J01] 获取当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gebvnfmmq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxuljocm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/ghzrkhsmm.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gvngabylm.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gjevsqdaq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gdiiqilau.sHtML

Go:   time.Now()
来源：http://www.blog.yfazqb.com/Article/details/gwyvyamao.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gpgwxtdkk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/gihcorljv.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gcqziumyt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/ghrhgqxaf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/glyeeprbl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.epnwcf.com/Article/details/gltaaaakj.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/gfhcxvvqq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gltstsqsz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gqxnazsyc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/griixcnyl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gmzcthaqm.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.vehdjk.com/Article/details/gokonfuqr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gbzlgjgte.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/glufkbbtr.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gxgsltjfs.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gicjxybbd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/geaciigfz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gatmgsgly.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gixwsiriz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/glpoxnfkl.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/grvusfmpx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.sjlbkw.cn/Article/details/gmtsfjbxe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.epnwcf.com/Article/details/gkhusjqcf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/gjtnkmbhn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gstgdsnci.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gzzhtljmm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/gfcjtbygu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gtcslrter.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/glfujdjqk.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/giwzckbqt.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fktsv.cn/Article/details/godflwgvm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gsdikzcoi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gaoubzfsf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gfmdupjrs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gwjgpvvlc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gwcjbqzji.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gvvblpogj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gmfsbfpqn.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gfirhjsnr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gxoxvwrrw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.epnwcf.com/Article/details/gvkarjtvb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gmfedqnbs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/gjyqbegew.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gmzskwpll.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/gjlwcxfqj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.yfazqb.com/Article/details/gahmuoeka.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.sjlbkw.cn/Article/details/godskoiqy.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gqairwfsx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gawdedwzv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gllhrmscv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gldhcggxy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gjizkgpnm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gossoikgf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.vehdjk.com/Article/details/gxmwcveaa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gzqmxynhj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gtktgvvmi.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/grkmdkgyu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gxogjeekf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fktsv.cn/Article/details/gqiqbuxfh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gylylsfqo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/gkxbuvokn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.tarul.cn/Article/details/gwplwvzgm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/gwnffwkvt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/gohlvibmy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gmqigmipn.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gqohiqjcg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/gnidtpypj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/gedgwepie.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gcumewgby.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gvxqlwbrj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gscthvtpa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gjpykjvqo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gcjkrkhba.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/giopvmddj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/gayspqelw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gxscxdstf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gyscdbgxp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gbqggxkak.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gmgmndnmr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.bbcook.cn/Article/details/gsgmswqjw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gnvhsovpb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gildiznrv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gdxipstyw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzgissyto.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/gaohchtnh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcrpmppgd.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gapuojyin.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/guxongzmg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gagermizo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gmotgkfvd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gqstjemqw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gkmhupybo.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/gqjqnzptg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gwnzjyabz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gnztgqfoa.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gzowhfhaj.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/guiyodciv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gophykicb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/ggmoselsx.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gisgvsqka.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gjszhvfxv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gevrbrupq.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gawugdbgy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gpvkcpahi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/giavddcqb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgmyricw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gjpqvvzug.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/grtyvklvx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gvcsevltg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/glcqiwkiu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gvhqiugfj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gaxpywcgy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gszzhmyei.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/ggfodhykl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gzmsynfnf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/girxovwow.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gfvctfjjf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gtwdfquhb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gyihhlvaq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gugpjwbjz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/gcmcrkbsy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gjdlofdhh.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gvzercwnq.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/gxtpknayw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/ghfdvvbzo.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gfqhidinw.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gujijpeqk.sHtML


<!-- 参考信息 -->