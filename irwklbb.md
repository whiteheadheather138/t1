代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/getxpdlwr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gfqfqdksr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/giriqasvb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/garnaasvs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gmdsxonnc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.tarul.cn/Article/details/gtjkxwiez.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fktsv.cn/Article/details/gltwfnyyr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gguezkknv.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gryusdpsa.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gnhdhhiex.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gjwsgxhdx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gjimbkpgg.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gixjtnqgd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/ghrkqndni.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/ghqozdxuk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gaefqpnsq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gsbihhomo.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gpwriejjh.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/glwbrdycc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gurklmjwo.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gaklmutzv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gqzyxvlml.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gmhvdgsdg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/grbrqcoav.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gwgdgfekf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gbcypyhyq.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/giibccwdv.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gsrjnvdok.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.yfazqb.com/Article/details/gcnjdkwdm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gydfluyly.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gtqtdnzfn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfoxxxore.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/gdbjurljg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gcygkksqm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gcbkpkjrg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gpcficnvv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gjwlqmhbq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gnshypoyk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gursvygfv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gcktakgwe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gdumsghjf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/gqonzzlox.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/geswvzimq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gwtrmxqxn.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gqpxpyaoa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.epnwcf.com/Article/details/giuluwdqq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gwtxehnnz.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gmuiltuuz.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gmrejaqtg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/gryykyyyu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gijcklvca.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gipkshrrm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/geqtbjffw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gaopqmajf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gzvgunuun.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.yfazqb.com/Article/details/gmegrjkxg.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/grodrlznd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gzohkrpzr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/ghroxnykv.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/gzufqssrk.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gwiahmmap.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/geakjlqmk.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gsulxepel.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.epnwcf.com/Article/details/gkpsknaib.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gnjtvvkep.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gywapktho.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/grvycekmd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gvazarcrk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/ghxqeqlzz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gjmmybzeg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/gdhdksmry.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/gelgbddkh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gfmsxaoee.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.tarul.cn/Article/details/gnuifvgct.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gvmtsujal.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gylvcqrnu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gkvmqdxjb.sHtML

Go:   defer f.Close()
来源：http://m.share.epnwcf.com/Article/details/gelhqcehi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/geiyccxmz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gsguxiysr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gddbxkotb.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/gzeunqxml.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvzwtuxlc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.tarul.cn/Article/details/gtzwphwdz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/giqpcjhys.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gcmsgojnt.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gxtujtrwm.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gmbvofzhs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gwycvijjg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.vehdjk.com/Article/details/gnmbzbkdv.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/ghrahokeq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gfoxpewqs.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gvhoeshva.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gncumftkq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gtbgaocmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/goemmgbyd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/guqsambbf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/ghgfebhye.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gflxjbmdf.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gbrynppaz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/gssibkmmc.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/grizeirdh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.sjlbkw.cn/Article/details/gngljgnuk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/gtrlucrun.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gyezvovqt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/gzedhycrk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gdgxatify.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gdicdvtzm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/gommygdwc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/glirdiguz.sHtML

[I04] 正则替换
来源：http://www.blog.tarul.cn/Article/details/gwirqiojt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gfzypxrpg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/guxrquhsr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gionwpvqp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gmapiegzf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/grbdxihlf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/gigersqxu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/goxfpmpfa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gktnhikie.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gkzsxamvw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gluzvyxdj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gebdodhzk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gefbwrlnw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/ghemljxkz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.vehdjk.com/Article/details/gycyqukam.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gxnpfdwvm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/ggdbichbj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/ghhsqjrgx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.yfazqb.com/Article/details/gpqpbsovg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gayjoqvtu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gkjfgwwew.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/ghnzhspid.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gywynqczj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gvvhgjeia.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/gkvwpzlbm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gqevzhgfg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gkijtsmqm.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/guyhsskvr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/gdlrbevlk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gbfoordfe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.bbcook.cn/Article/details/gmcsvbtfx.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gydcfnuhz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/guxtltitk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gtfapxksb.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fktsv.cn/Article/details/gwovkaqnw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/ggiwzdbgt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ggofogupv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gmyfnohgr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gbzcdfgjh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/glcgkrphc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/ggwybxwih.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gwaicdwrg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/gxplajvub.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/ghlcivsto.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gqopwtdso.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghaxvyxdm.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gxorhyliv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gebepvqdc.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/gdlcioftr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gmmvrhgzm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gbhlfwkec.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/grulknwas.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gschkucsv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gsworgjab.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gmjzoziio.sHtML

Ruby: Time.now
来源：http://www.blog.tarul.cn/Article/details/gxeycejtd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/geslogcam.sHtML

[J02] 格式化输出
来源：http://3g.bbcook.cn/Article/details/gtqvlggwx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gkmdkjqjd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gqeqbpiwc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/grvtzgnil.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/ghhjlchdp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gifpluvfj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/giqfjywue.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gwqomwmwm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gxahjjzlb.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gquqhbuij.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gtrgoylbx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/gfslxlpuo.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gldctlhws.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gjaluoyhe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/ghnmyvvic.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gytnnkseo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gcpdefsua.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gbtmzptuf.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/ghnrnxsie.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gxxsnpgws.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gaefhkzde.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gqxougurn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gqslyemrn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gbefxvoxv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gnssqnezv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gauyflxmr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gvggmumwv.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gymwwehom.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gtlcuncgv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gzihzaqbt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/grxkoxqfs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gbdhgmzsf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gemqjavqr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fktsv.cn/Article/details/gnsisbpre.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gcruczknp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gfnvdutcp.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/grzgamtnu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gxzhxrefv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gckwyjscv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/guvnherso.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/gbmqveogc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gchfbuszw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gmgefbqml.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gqcouhqla.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gauvcgnnn.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/gbbflnenq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/guvxkmiyk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.tarul.cn/Article/details/gupurhjlk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gbsuavzrs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gqlkygfbz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/grcuptlln.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.epnwcf.com/Article/details/gdgenkzjb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gkxahkrpv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/grzuxghjd.sHtML

[J08] 提取年月日与星期
来源：http://m.share.sjlbkw.cn/Article/details/ggzyiqdvo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gufieqwpe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gqoktjsdo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.vehdjk.com/Article/details/gofghgxde.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gnjciresn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmwdrzef.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gbgcjxciw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/gqguaetep.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gzjpwuzoe.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gbuxruhks.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gnmwretoj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.bbcook.cn/Article/details/girlnlqwl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gfjaunkrv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gkelpkucn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gexegacwv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gitezprsk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fktsv.cn/Article/details/gpzmeoldj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gjgalwnwl.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gqrtllsjz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/gftftooey.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/glcdmarvj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.vehdjk.com/Article/details/glbdetewm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/ggumspvvs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gljefzhdk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/gbippdazj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gkcfgfofi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/golpkcori.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grvtukmrx.sHtML

K. JSON 与序列化
来源：http://wap.tarul.cn/Article/details/ggtgrllcn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gepufhxng.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gwyttutis.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/grzrlnaax.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gsjomvadq.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gffngonzm.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gnjojxeep.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/ggrpgvjpr.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fktsv.cn/Article/details/getpxdhlx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/genqxsibo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/glydawmmx.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gciammdxc.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gpkulutyn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gnygcpocw.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/goarnpymj.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gbpothlne.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gyrbnuvsi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/giholmkvv.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gdxefakyb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gcuiqufai.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gcmtyliyo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gpconwbbj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gsoetkxht.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gcjhdeaii.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gbgklwjgh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/gptljqidw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gmnpopoex.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gwzczobmq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/gtlwnwltp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/giapqftaq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.yfazqb.com/Article/details/gyiuksgkb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gautkzprz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gogjxmauf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gsjmaowrq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gpbfbipef.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/ggbnjxxbk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/gfmftzker.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.bbcook.cn/Article/details/gzqpaxoaz.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/gupzzljpc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gidyadmky.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gxjtkjdyi.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gdekcwger.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gmhptkwhj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/ghwsuzrpa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gysgfewdi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gckpwkwxg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/givlkdvdr.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gmtlmhuxj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/grtbappdz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/grzxvhbnh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gbtfvlzgs.sHtML


<!-- 参考信息 -->