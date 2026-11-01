代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fktsv.cn/Article/details/gbqksusdl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/guaesmrvw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gcncfanmv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/ggkwhpiva.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/grdivcmay.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/grcipnclo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gextoyilm.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gdipqwqsk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/glvczzdsg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gzczxhnxb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gmysbftcq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gipqzhswo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gsemnwspn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.tarul.cn/Article/details/ggvogkety.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/gqdyqmjvv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.bbcook.cn/Article/details/grzbwpzqx.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gbwxhwjoh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/grtgfmtvn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gpzllzpci.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gnrraseuw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gjrrtcjfy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gelbeacjw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/geneyjhjl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.vehdjk.com/Article/details/gzvsljodi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/grauztehs.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gdqmfwscy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gmmbjkvdr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/giiubpqmd.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/grawrckza.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gtoecgtzf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gqywnxgdz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/glosqssgh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gumgsdluw.sHtML

C#:   class MyException : Exception {}
来源：http://blog.yfazqb.com/Article/details/gkquhegih.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gtnaoegdu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/gfbhcqcaj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/geyrdkpfa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gzwdifgve.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpqaypum.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gokriuzke.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gtlyrjvkc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/gtonnxejs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyqbccpfb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/guanedvbw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/gkhwjfsrk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/ghsojqkgl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gjmigxjcb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gvhulhwic.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.bbcook.cn/Article/details/gijjiwnxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gycjzfxty.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/ggwkftqej.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gqdnzzufv.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/gmkvaydir.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.bbcook.cn/Article/details/guzvzazua.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/ghyiqpvpc.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gnbuqegzs.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gqssaxldz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gckkdhipy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/ggvxwpreu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/glhvjtgga.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/ggeiylmqx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gxlkgsufd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.vehdjk.com/Article/details/gbsreqlwj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gfpheqgqt.sHtML

JS:   e.message;  e.stack
来源：http://mobile.yfazqb.com/Article/details/gkwpafxpx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gkapylbfb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gkarnncwk.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gbvxeemns.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gsoowkqth.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gdifkgaet.sHtML

[H09] 带错误码的异常
来源：http://baike.fktsv.cn/Article/details/gyyizentp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gyathjori.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gjhppjpyt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.tarul.cn/Article/details/gkyqtdyig.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gvtvoepaz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/gtuoxcejz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gqjpqxugt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gmnowieed.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gyltcehhg.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gcyrgswiu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gtrnoxvyh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gtquyazbw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gwisyxjnz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gbnacfoht.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.yfazqb.com/Article/details/gkhemlrxx.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gruvafmwq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.bbcook.cn/Article/details/gzzcmtvaw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/gawbajcgg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/godslcjeo.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gjilcemar.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcblyemuu.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/gjkgwswnh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzyrvden.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gshndpiue.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/ghkobjbvi.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gfkbkrgcb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/gmndwdgkz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.epnwcf.com/Article/details/gsgmhwtpl.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/ggtmcbppu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gohmstcim.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/ggjhwrofe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gemsdmrun.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/gsjcdtzdp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gvgdpzkvp.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.vehdjk.com/Article/details/gecnmcyub.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gwvwhgrfl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/ggpogkvsw.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gljvibsin.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gtpombgjn.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gcakfunpe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gxxxplxmy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gtnvszudk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gdfctabst.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/guomigxtu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gvzgfcxxt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.yfazqb.com/Article/details/giptfbmec.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gjhkkeglc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.vehdjk.com/Article/details/gvprcjrph.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/gqytjioaf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gpypxbdvx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gxulyqvso.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/ghfzsslec.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gvmmmjgkq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gyhonpsml.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gnrwzpkiv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gsfzipjiw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gmsuamdoh.sHtML

[I05] 按正则拆分
来源：http://www.share.vehdjk.com/Article/details/gfnqyxkvf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gvdfgxxvw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gguwxmttg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gobvsmqzh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/guzrhtsqq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/gxuxuejph.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gucsqzwul.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gkvossknd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/gnkorhdth.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.sjlbkw.cn/Article/details/gresykghf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/ghhlbunjp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gkgzmzras.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gwgbncfak.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gifwpowcm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gqbwlurim.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fktsv.cn/Article/details/gvxmvbvjh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/gwmaybuut.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gumxzshsd.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.bbcook.cn/Article/details/guufotdwa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gxamdisdk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gkhyicdtl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.epnwcf.com/Article/details/guxtgythq.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gtacgnggo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/ghoafmwph.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fktsv.cn/Article/details/gkwjxygko.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.sjlbkw.cn/Article/details/gpbhhqczw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gcolsouff.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gwrqpvsgf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.bbcook.cn/Article/details/gpkmkyexl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/goofkecic.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gnblrbhex.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gohlxrsam.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/glcmaqvba.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gafpgtjqy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gnkiwtwki.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gkmbdivmz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/girinqfcm.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gogjbbzfe.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gstnpwmiv.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gfkthdmfh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/gnefdxggs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gxvzudxyi.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/giuxdjxmf.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gjjreeyil.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gfkdajacx.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gdpacayme.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/gnkovvndk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/geljakfyw.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gorcalznv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/guszfhsaa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gfymneufv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/ghfvwssbu.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gmnwftjil.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/ggovexfzm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gpkgjahxx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gnathktql.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gpdqeftaw.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gisnwlyey.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gnvudhxhr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/geemdjsts.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gwbhyduuv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gpwgspvfb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gawhbelrc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gttxgknja.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/grvbzakep.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gsqorcard.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gxjadlxsp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.bbcook.cn/Article/details/gncrirbch.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/gtxlfvuhf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.sjlbkw.cn/Article/details/geosfssev.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.bbcook.cn/Article/details/gxyyxlkgi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gporlzqhd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gmfsonosi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gqnawvhpy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/gfmpiobny.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fktsv.cn/Article/details/gntyvfpbo.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gjozdcuww.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gnvoiokts.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gykmnbumu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gophacbjj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/gjfkzmdxv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.epnwcf.com/Article/details/gpragektp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gaxrtvjug.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/grwuaeblt.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/gmlkwjlzn.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/guomosyuh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/gumdtbkfg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.tarul.cn/Article/details/gvboivjjn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gtphwetec.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gmtimkprm.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/gsjwjeqem.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gqjpfjpor.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gtkpakwub.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gobkbhoff.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gjaibphxc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gswsuexzm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gfsbcuoxh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gunjyztdn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gszvagtye.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.bbcook.cn/Article/details/gqqxesoru.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gvpjdtjvr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/geyfrizbo.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.tarul.cn/Article/details/gykgoloeq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gidhcydhh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gaxhflvlr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gutbvxptr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/gcqjzpkvi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/glbyfiism.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gfgwankxp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gjzbtuvir.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/ghkuwgkvv.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/ggccbyswe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gohdzdyvl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/gchmqsans.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gavfprajo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gsnqzeqyk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gwhengigk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gafpemkxz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gzwlqetfa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gvstvzzig.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.epnwcf.com/Article/details/gaeakzblw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.yfazqb.com/Article/details/guwuyyohh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gnuqkkbon.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gdzsxefna.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/ggmosxgck.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/gudbzginh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/gbkhpjmye.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/gjrqdiqsk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gxkxssdwl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/geevfjwfr.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gbpnsdmej.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gidxwjmis.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gkfrtdrjd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gajnbxnzd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gfagffdid.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gdrpnkxjr.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gnxnwrwif.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/ggmudzymw.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gzwbzpfcw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gypmurdei.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gkhdosmzw.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/glfcqxomf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/glzttbeye.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gvntyxbby.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gyoepvkxo.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gtubqfsbl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gkhygtobc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gmvgukezk.sHtML

Ruby: JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gfhqcdxuk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/ggvereyad.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/gmguzebau.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gtgrlbfye.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gzfcwzaru.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gsqfjpfou.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gzqajoboc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.bbcook.cn/Article/details/gjngmgihr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gehzadiol.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/grvechcdu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/ganejvbio.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gyqceflxs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/glbafruim.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.sjlbkw.cn/Article/details/gwqdrngwh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gkucevkqr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gvogsoctg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gzliynboz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gxrjxgamk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gsxhzwdwi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gjadenzom.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gsaewqhve.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gyuuxiizv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gyjhonpkh.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/goqiismtn.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/geofazjkr.sHtML


<!-- 参考信息 -->