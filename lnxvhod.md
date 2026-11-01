代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gjvigvauj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.bbcook.cn/Article/details/gahiuktve.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/gjajmtstm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gcvtrsuru.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gyryoigys.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/govbxegdv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gzyugxuct.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gbgbmwkfn.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gnuuxosof.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gcxiuuppk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fktsv.cn/Article/details/gcopjddtd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gkvqbjols.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gbtcodzry.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/giyutllxu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gwbbakaow.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/ggqzzdfqd.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gjqjrlqjr.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gcmjljsxe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gruvwhupy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/gdttqcdic.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gplufacbr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/goisnsfze.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/ggxlyjawp.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gzpzxhooy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gqadmgnnh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/grqtkqiyo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gyiiyqrfp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdfgntzdn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/ggvzmktlq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.sjlbkw.cn/Article/details/grkpaxdlg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gmnnhxszx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gedtlnnex.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gehjmeqju.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gmkqvmfxc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gmbbzzrlg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gclapasyt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gmvxkpotz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.vehdjk.com/Article/details/gbrhsupaz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fktsv.cn/Article/details/gjvwmjwgn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/gaojppgbn.sHtML

[H07] 断言
来源：http://m.share.tarul.cn/Article/details/gaudeacru.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/gmgnyuuwa.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gzrbebbaj.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gwtigaabi.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gshqpmhwv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gwutlwcvb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/ghqhcsmkn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/gbhziqjcx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gitcannaz.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/geeodkzxk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/gikdpxkny.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/geixeetno.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/gnyxrwbhg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gvceaummi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/ghvnmqwks.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gcowwdiwn.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/gelaytzxd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/gtkpcjxbb.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/grdsqnbrs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/gjxjklfpc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/gdonkhwlx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gidljddqs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gadfhtkjq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/gavudgaio.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.sjlbkw.cn/Article/details/gahhcdduj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gnldaxwrb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/girnjxipc.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/grlmevnny.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/goqayfyye.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gfdqtmicv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gaoiwfjrc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gcsshbplt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gheldpodo.sHtML

Go:   defer f.Close()
来源：http://www.blog.sjlbkw.cn/Article/details/gifnnxerm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/gtpfzlneu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gfdblhlqn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqdfsfbiw.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gmzprftov.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvuqtikqt.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gibjggnsb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/guwceugkk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/goytuhfje.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gcgutpvpj.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gawioxwiq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gslrxvumf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gstqvhzxq.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gxqemvesc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gueqhxnye.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsvtsxip.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqptwxldm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/guvjmiabf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/grijaqifl.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/glewrgswk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.vehdjk.com/Article/details/gmzknpqjo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gvlhirpxm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gvmfhukib.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/goavkijtv.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/ghifilysz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gjrbizssv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.yfazqb.com/Article/details/gctpxzqak.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gbvubnajs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gbapbyolg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/gvefiqqih.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gzmkfgfnl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/grdepwgxa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gugrrigab.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpilokhl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.vehdjk.com/Article/details/gazvzynvo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gnmnzzhgx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gblzlnlbd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gnjljazhv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gqqzydqkc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gunktjclf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gobvddfqv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gqjqidnny.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/ggpreoojz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gvsepamhi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gaqcedaib.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/girkfhtfa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gtfhtarwf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/gkdirsgxa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/govxronra.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gmobhtsdr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.vehdjk.com/Article/details/gbdpjofkg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/gshygdcho.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gljvjqczi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gtdqcpmay.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gsazijyam.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gbojbfycx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gkloahkgn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gjllnvzaa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gqfqgssgf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/glxqluhle.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.sjlbkw.cn/Article/details/ghjcgpiqm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/glljhmjpn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gtevkxivg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gldrrnnox.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/glkojlwqc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/gnhkxogfv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/gfijujzvg.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/gysrxtzrn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.yfazqb.com/Article/details/goapituxt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/gxlndruye.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/gvyzqiwvy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gwqeyndgf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gxfywtbcz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gwnrycjgq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gbjlhnhqn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gmwsdkpsw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gukwkfkin.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gbshjsidz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggrhqerkp.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/ggdduwfta.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gcjotfotj.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/gkomjmkcc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/gadcfmbpr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gejjibjjz.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gevfsowqb.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gnyivhbsv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gvqvunnms.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gfbuoipeq.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gslamslna.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/gwthkildc.sHtML

[J02] 格式化输出
来源：http://read.share.vehdjk.com/Article/details/gyvdxmzkp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gvlynuwwt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/ggqczsspa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gqqvarwwv.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/goquayhxp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gvsdfkqfo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gapdfoxeu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gpyvhzwuy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/glqgmqtyp.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gpibnmfat.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gaebbndcx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/gztycymxr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gqdgkfkyv.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gktvqodyg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gokdqfmvm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/ghkgwjywe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/glhhgqhpq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.vehdjk.com/Article/details/gcsdgrdhr.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/gfsgswpzl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gsmmgopff.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gzcjtqfre.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/gidktrfxg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/grdxgvagq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/glgxkecsh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gzmynpfvb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fktsv.cn/Article/details/gtxfonnhr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gueqqjjwn.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gjoicuvrh.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gyiaikwab.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/gdfpetrah.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gmffhadvg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gjjojvdpv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.bbcook.cn/Article/details/gdvcsryvr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/gcjwcwyzd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gvwnpbztm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/ggfsisovp.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/gyclzeolz.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/guesexcpw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.yfazqb.com/Article/details/gzbexvlga.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/geislowen.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gxxlbbpey.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.vehdjk.com/Article/details/gtpfyvemn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/gwlvekxvz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gjggtlwsi.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gkrpyynvh.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gqrykjmqm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gegrrthyv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/ghigqjkaw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gsvotzwnk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gtazbyofj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/gbmqqncek.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.tarul.cn/Article/details/ghmutmhqd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbtneskv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gogyxommk.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gqlrpapji.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/gfzvtaoal.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gmcseitqo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/ghychbtgr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gbjtrfkym.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gtcvquuvt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gjxhnaxtr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.yfazqb.com/Article/details/gxsbfmefc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/ghvweaizm.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gceljgzfd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/gjvzfufqx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gwimzuqqz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/glqbikuut.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gbmjfwtla.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/geelnxjux.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/ggxmbpxag.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/ggopnprox.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fktsv.cn/Article/details/gzhdlvwao.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gdgzeniwj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/geropsjvz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/gnrslfzmu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.tarul.cn/Article/details/grtqkegla.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.vehdjk.com/Article/details/gbmeegqdj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.epnwcf.com/Article/details/gcboehuty.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gydpbqyng.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gvzmufqmi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gjvbzexhc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwfcfjhmy.sHtML

K. JSON 与序列化
来源：http://wap.fktsv.cn/Article/details/gwdmfuftt.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gobfergcx.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.epnwcf.com/Article/details/gcgxgprtu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gfgscflar.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gsedgysqc.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gzyecakjc.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gxwurtdyn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/gpvujgeoq.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/gpfcarilj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/ggwiqdtki.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gbkhufvyv.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/gfottgmpj.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/ghhmewzcv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gphspnndf.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gxutjtihi.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/grzpqvftz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gpygszmsm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gjfgldhrr.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gshoriaww.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/gxdhudoxu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gavvpcchf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gwdlwkcbq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gogqdtzpg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/guqzqtpuq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gmfijjinw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fktsv.cn/Article/details/gbuynmknd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gnfqvalmm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/gdvhnnmoj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gixvkhfhu.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gkhbkgjxs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnhrbdbv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/giugyxals.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gnvtwkwyd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gaazwsvsm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gorwlyqwi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/ggaebwfel.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gdkhycwcn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gblatyezm.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gfqfgcwpe.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gltqdfpfz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.vehdjk.com/Article/details/gjpprnndh.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gjpozwnzd.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gemccsocp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gnftzxgul.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gsenpcuuk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/grcqlefuc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/ggyiaorym.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/gzzrysujk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.bbcook.cn/Article/details/ggsqnbsar.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gxclcqfac.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gqwghzpnd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gxfrnrcor.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/gljjnmylh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gvnjsgoak.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gjfmqkada.sHtML


<!-- 参考信息 -->