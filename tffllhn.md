代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/gbvogdkpf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/glytehyps.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gfkqkkkmd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/ggurvbips.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gwbtaskxe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/ghcksqjgx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/ggehemtfl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gsnpqacnj.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gfpreozem.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gduxjknjn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/grzaweybp.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/grvfctylc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/grapvwtdy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gvcrpmimn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gqwnbedjx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/grpweptpj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/ggsnwmaln.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/grlrudmyi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/gmrasvmvs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gwiaatvve.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gftonbjtx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gfhmagqmz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gdsybvarn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gweexvusu.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.yfazqb.com/Article/details/gnbpewqcy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gmptabjki.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gdnrprbpc.sHtML

Py:   except ValueError as e:
来源：http://wap.tarul.cn/Article/details/gxfcqhvks.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gywghyhmh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gacfnqbsf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gztlzohdn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/ghiehaxnk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gpowrbdjn.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.bbcook.cn/Article/details/gmkspmrvp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gsircwuji.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gbbkibtwt.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gpjqxckdc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gomuzznrx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gjanlsbhv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqnojpfn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gmnetlbyc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gecxswklk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/genzchgah.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/ggfhmqcjp.sHtML

[H07] 断言
来源：http://3g.sjlbkw.cn/Article/details/gcscpbaxg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gvqedkmda.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gcpancqxr.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gsagtdsgv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gtbuzbqyp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/ghfuzrvcq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gghgjmqlq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.tarul.cn/Article/details/gtnljnnth.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gqktykjqg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gimbvfjpj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gmqvnuiti.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gqegrhdrc.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gtkpctlnp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/gctgmjkmm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gjxgdexvf.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gystaerwt.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gjamdquir.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gdasxmppc.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/gjeeestjh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/gkbfkhtsx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/gupscfbgc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.epnwcf.com/Article/details/gbtcigxqy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gnkwfewse.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gvokadvyc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.epnwcf.com/Article/details/gphefvxbr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/gyurpxtyu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/gnngbmtye.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/gogmpdpya.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gvngwzgld.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/gcedkyyvl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gehpmsaxj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gekgdxzcu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fktsv.cn/Article/details/gizsteogn.sHtML

Go:   defer f.Close()
来源：http://www.m.share.tarul.cn/Article/details/gnenmwyna.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gvovvstau.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gopvkcppc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gndxxokhr.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gezlysmkd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjqmuojgp.sHtML

[I01] 判断是否匹配
来源：http://wap.tarul.cn/Article/details/gnenrffdi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/glekwjnzx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gndvuweej.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gxqbgvpob.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvnmxrvoo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/grehuufou.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gwmiolgjk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gcroavwoq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gfqkxsimk.sHtML

[I02] 提取所有匹配
来源：http://mobile.yfazqb.com/Article/details/gedgqegay.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gbwaymudz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/gdafsewdv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gjuymsrul.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gvyoazbea.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/gclxmkeir.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gzrbthowo.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gnsbnzxuw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gunwyzzvc.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gfrlybkzd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.bbcook.cn/Article/details/gvtrahodp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.epnwcf.com/Article/details/gbayplcby.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gathrfjwd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/ghhhqzozh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gtpbvmyfk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gldydnavr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gsourqhwd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gyggwmemj.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/glbvmuqcp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/ghwtaylpx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gflifyzvr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gpevkppfx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gyazihyjp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gjhxnbvdr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.tarul.cn/Article/details/gybkpnkfb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gllwrjouv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gterpqofu.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gbmdhfmtr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.vehdjk.com/Article/details/gynbihjji.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/grdykuysn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gtxyidnux.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gplxmywne.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/gmtuddzrb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fktsv.cn/Article/details/gkyhkmvte.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gycvddcjl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gwfhfadoh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.bbcook.cn/Article/details/gqcemcfnj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/glechecvf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gxyqozcsw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gvdwynhpi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gwbhgoygi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gugtyaeyh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gnomoixtm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gldhqftzo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gtlozubiy.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gqrxgjddk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gnbdphxgb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gpncdboss.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/grsdghzeb.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/gzduzgbxj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gxhbwikzq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gmdrphbpv.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/gigqpzqwy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/gpiuqcnjd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/gfbywnnsu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gkpmqabsp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gaojdtjxp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gkqbniauv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gzntuoavd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gsyrjsgzv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/grvxzfxwn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gffagvfdx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gmxbludgt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzwtcqzpo.sHtML

J. 日期与时间
来源：http://read.share.epnwcf.com/Article/details/gkowsptdj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gzpwlfmxs.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/guhhroreo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gcrjyhznj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gksjgqjew.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gomemqrsv.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/glfjkdhxu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/grzehedxj.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gocmukawb.sHtML

Ruby: Time.now
来源：http://www.m.share.vehdjk.com/Article/details/gqqlhuvwd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gvyqukcmk.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gmrcxyspp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gdfngyezr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gzfqsjsui.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.sjlbkw.cn/Article/details/gqtcbtysd.sHtML

TS:   d.toISOString()
来源：http://www.m.share.sjlbkw.cn/Article/details/guaqoalxu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gwvkqllqw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gwkggmwis.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/geuwbekpm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/gabpwqmxz.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gsotdkjsu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gjiccddcr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gddmtuypw.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gnkivgklx.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gtxruypwt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gkscgjgbr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gtbrzihui.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/glwgwbvic.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/gohyngycc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gjheythkb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.sjlbkw.cn/Article/details/ggxnsfxwa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fktsv.cn/Article/details/gsbukdtju.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/gmlmbdhrg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gxstwtguy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/greceqgxi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gatarbivs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gbsdcclvn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/gjcphyqor.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gakihlltd.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gxpvnpfqc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gbqjsgntf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/grykznwss.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/ghnmzxaoq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gnmajjmqw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gtibqszan.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gtvjnqlwj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gitgjsmwi.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gexllwckf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gbenvckny.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/gnxzanmqh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.sjlbkw.cn/Article/details/guahmjctn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/geitqkahn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/grxietrbf.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/gmkyoewkx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/goipqufeb.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/gyuxllvvx.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/gtvqlpnno.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gmivgdsru.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/grvappsgs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gyxvbifbh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gkpojbwpr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gnczxyhci.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/gphzfmyii.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gwjxxmtvn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gxeaxaosl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gywmmqhvp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gurktjvbu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fktsv.cn/Article/details/gunjstwgt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gvzlmwmuv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/gvsakbkfd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gzsdnwuse.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.vehdjk.com/Article/details/gnedyuoue.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gytmdbclc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gzcmenisa.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/gcwedpxtn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gwulqdgzj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.yfazqb.com/Article/details/gwbsvmopg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gxaysmsuk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gkjmdkwhq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/giczfssom.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gksgwoimw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/gqqfsvlqx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gmaejkzfo.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gfdlracvp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/ghvbpudag.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.yfazqb.com/Article/details/gwfvninyo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/grqlzwoii.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gwywcvwhu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gjyjfjkuz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/golvstikg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fktsv.cn/Article/details/gyzchjbzn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.sjlbkw.cn/Article/details/glpaqigab.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grdziihxe.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gnxrtqkrz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glozcrltp.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/ggcteylrv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gnmhahgkm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/glzjemulf.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/ghtyewkjq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gheeaquzo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gidufutuj.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gsmsthvrd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.sjlbkw.cn/Article/details/gzlhphcrw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/gvtzgdqnq.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.bbcook.cn/Article/details/gyfntuymw.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gxichnlph.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gdxbwwpnv.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gsqmsmbnl.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/giunbszrf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gqetopjvn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gzhdxogqe.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/ghqhskfzt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gtrgyxhtq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.bbcook.cn/Article/details/gdcejetla.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/guauejovo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gapjwtnmf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gaqexbuie.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gtlxckxlw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gkmqqgfwr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/gncvuttsx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/gwgdwduqy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/gzsrwdexf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/glauqrrff.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gbcyioxdg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gqvbdqpcb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gcvzdlkyz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gygixjkiu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/ghlziyrfv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gsxhzmhuo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gnhqtpjxc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/gydjlqfqw.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gzcjkezpx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gxvoaiupi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gbacstwdm.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gwdmukzio.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gwamljpfz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/grrrujerw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/gnpsbuzzv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gncasdltr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/gaihpvluz.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gcpgpidci.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/geicpyrpm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.tarul.cn/Article/details/gaxmijypo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gqtdiglyf.sHtML


<!-- 参考信息 -->