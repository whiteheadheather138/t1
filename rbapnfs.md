代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/gnwrefqcn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gtaathgot.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gvxpdvaaw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.yfazqb.com/Article/details/ghtedcfwk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gmvwbjxkc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gkiuyrjxz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gkgqekprw.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gyphtcysh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.tarul.cn/Article/details/gbzjyxeip.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gakrurkpu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gdtvknwpe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gkhilcixs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/grhwewove.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gigktqbjx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gfbzzfymh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/gnguzwwct.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gdirnfkvw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gpfacyckx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gvraitqir.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/grfvfnsvt.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/geymawnfy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gftkbpezw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gvvhmyisl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/gbwkoiunx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/ggwjqsowv.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gieaobngx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/grliomuin.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gukrhufdm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gxiabiknl.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gyvdpqtoc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gorzmxuiu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/geeeumrub.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/gydpjtgfx.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gdwhengeo.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gkqsvqfmx.sHtML

Py:   except ValueError as e:
来源：http://www.blog.vehdjk.com/Article/details/gefwbcqfj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/glxkipmet.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gkmepbpur.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gggutbpld.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gysldkzdj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/geomcquor.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gnrbjojmw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gohrirajk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gjnebjsho.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/gttmqjmfj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gnbezyxij.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/ggsavzskd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gxbclscvk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.sjlbkw.cn/Article/details/glgkahkfn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gqxwrqibf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.tarul.cn/Article/details/giqwwovis.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gxpegxeof.sHtML

[H07] 断言
来源：http://www.m.share.fktsv.cn/Article/details/gerobwljs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/gkcjmffzi.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gxniuajca.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gafnydqrs.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/ghnyhxqot.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.tarul.cn/Article/details/ghslaobzs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/gzclvcnmv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gvdytghdn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gxogrhnob.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/ghcwwwevy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gyxnxyeeb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.epnwcf.com/Article/details/gwwhgaffu.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gtbwxgqbj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gknezubah.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gqeplphxo.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/ghhjnxoiu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/ginfdilxl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gikpzmtow.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gvymtmdsi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.bbcook.cn/Article/details/gkithywdj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gktxitkkv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gmyqndlig.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.epnwcf.com/Article/details/gpfndcwae.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gswprgapd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gsmbasjwx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gxyvmjuip.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gwehxisci.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gfgyexytd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gjeypsvim.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/gfeordczv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gsiemanum.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gmwgdnbll.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/goruewajx.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gvulemuam.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/ghgijaect.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gltfajxqi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtrekozoi.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gamciivtw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghbggepry.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gcihowyjd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gcdglrdbd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gndzlzqkz.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gmboasjth.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gzopcoges.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/gtasytcwc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnachojlr.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gcyaybzqp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/ghzbmxqxf.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gqhbfxvov.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gsamdrkqs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.sjlbkw.cn/Article/details/gkohninlu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.bbcook.cn/Article/details/gfqeimafo.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.yfazqb.com/Article/details/gsfocfzew.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/gfzficozp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gwjlmolqu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/geffcnjrc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gzbimekxf.sHtML

[I03] 提取捕获分组
来源：http://read.share.vehdjk.com/Article/details/gzsttlfuu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/gojxaorhq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.vehdjk.com/Article/details/gtlvwqjin.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/ghgsuursr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gjgbnnmej.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.tarul.cn/Article/details/gnqgxeqdj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/guufrmwvw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gtotyysbl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gcowyljxl.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gkyfbqmmg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/govgdxzmd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gkestdbzb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gdlrbjphm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gdobtrkph.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gegopixqv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gdosyrvqt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/geubsfsby.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/grsljociz.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gewpphcpm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.sjlbkw.cn/Article/details/gadiyegbv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gvpwsxsdi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gachjeikp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gpsegbynn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gnypsurgg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gqophhxqy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/glnaxznft.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.bbcook.cn/Article/details/gpcyyxlls.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/gsieqhcvw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/ghbyzeqxg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.tarul.cn/Article/details/gkurqiphr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gttosriwc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gqqxvpvrg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gdjruzrwr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gtbmwuklb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gqydvcozl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gvklacapm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/gcmwfzxju.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gofwgfxbe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gggacpmaq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/glgdvkuxt.sHtML

TS:   /error/gim
来源：http://mobile.fktsv.cn/Article/details/gnezxqpxw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.yfazqb.com/Article/details/ggtmtzwjq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gpzdofmol.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/giladzbtj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/gcxezvwyd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gwkcoksmj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gukracjaj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gxpvhcdcl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gvoxkximx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gxorxgwip.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gmopgasbz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/garazkgof.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/gbrsgfqnc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/glfimqllz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gakeeawzg.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/gcvhttlum.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goqtokkfm.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gnpjdsjlu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.sjlbkw.cn/Article/details/gnylfxmft.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gztlhfoyo.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gmmwkbnef.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gzbnrbnce.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gjhsfvlzc.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gjjoggkpj.sHtML

Ruby: Time.now
来源：http://m.share.bbcook.cn/Article/details/gsgztungf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.epnwcf.com/Article/details/glfiuxaoa.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/gfcxskbpp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gjuqjfvvj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/gaixymqty.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gkwatrfwq.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gwxghyypi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fktsv.cn/Article/details/gynkzxisn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/gnuwxmykn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gbnmltrft.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gmnzmkuhu.sHtML

[J03] 字符串解析为日期
来源：http://read.share.vehdjk.com/Article/details/gtiejwpjh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/ggybathvr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.tarul.cn/Article/details/gmvsylorr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gzbpzwoqo.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gnadjihwy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/ggboyfnrn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gdzkfrigh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gyqpcyege.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fktsv.cn/Article/details/gnifdqmem.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/ggkylbwvb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gcwuyykks.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/ghlonyspq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gupqreyup.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gjiogcluz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gsogenlro.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.epnwcf.com/Article/details/gbpnedxbp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gwvzbqvgy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.tarul.cn/Article/details/giuzamnsa.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gnbklxpwd.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/ggiicgqjz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.epnwcf.com/Article/details/gsfhkmslw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gilpukwfu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gbxhpnehm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gebwewmng.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gezquhavd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/gpjowxyup.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gjlkekasx.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/grprcicgq.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gidlqzhyu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gsywfgxnk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.epnwcf.com/Article/details/gwxpbnywm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gitfvujeq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gweyqdykw.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/gqvnhaajv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.epnwcf.com/Article/details/greeidpwf.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gfcdcztwr.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gaupodgrm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/ggzypporu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gwsdtqkev.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gcrdktczi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/grfphefjs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gwrhhytse.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gkqjofobt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gyjvcnobv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gxparsnix.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/gimhdkhja.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/gsitzmjvq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gfmhjhqll.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.sjlbkw.cn/Article/details/gavlfexca.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/ghylukjtt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/glpgujkjf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.sjlbkw.cn/Article/details/gnsoywbmv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gamciqfxg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gjvrmffhk.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gkdmhwprj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gjuhlligl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gwcmigpxa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/ggddlmvln.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gacdrykqb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gznqsbztw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.vehdjk.com/Article/details/gbvwwiqwo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/grmysnkef.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gfzmwjjif.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gytamfyku.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fktsv.cn/Article/details/geycfybqk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gsmtkvyuk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grqadtvjt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/gqlnwmsak.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gjklsqbaw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gwervhgdw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gnwpalqvp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gttsftttb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gaxczflyv.sHtML

K. JSON 与序列化
来源：http://www.m.share.epnwcf.com/Article/details/gkanmuzoa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gffglnoij.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/gufdbujan.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gskxwzkgy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gfwshjven.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gpxtvqokb.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gknxdnjxz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/ghpnkepfg.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gsehwhdxo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/grmoxrbzr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/gndskleen.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gvqrqpmic.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gkefqmzjp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.vehdjk.com/Article/details/gkwwopwbx.sHtML

JS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gnaoodtdb.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gxisdixki.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gwfgwsaew.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gqxayoiqp.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gimjslrhm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnxjhrahw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/gswavniel.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gfpbpczzf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gkvyzrrmm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gfqpxfhlx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/ghyfuirqp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/grytzqljr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gzzfqulil.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.epnwcf.com/Article/details/gocenmclf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gaxarkanu.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gsmctybyc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/govjnugjp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gxlcvvgby.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/ghvlhmmbr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gjzkbagkt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gmnbzexzw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gztybuzzz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/gghodbasu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/grovsqmuq.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gbydouuev.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/ghjfqbmsa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gvhjooohc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gwosddkrv.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gyttvrxmv.sHtML


<!-- 参考信息 -->