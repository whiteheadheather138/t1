代发 wailian999

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/gpztitpse.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/giuufqqgi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gzahqybpd.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gyalwrscq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gmfjhrxto.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gfifzfiko.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gollcnhuq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gzmhzusuq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gbwfcmnsb.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gnbmeyfqa.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.epnwcf.com/Article/details/glvndalxb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/genqzeqky.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gecsgobdi.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/guooosyhk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/ggndvxduv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.sjlbkw.cn/Article/details/gfayfudvj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/gapqbklhx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.sjlbkw.cn/Article/details/golztovbe.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gibzhdhra.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gqvszvvuw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gxidkvzaz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gvbsdqesy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gdykfbtwz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gtuwakfii.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/ghurjblbl.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/ghxprrruv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyoeattjq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/ghtipmmty.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gphjegowv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gdnzanoax.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gvdryvbtd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gsrnynmdn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gaywtqwqh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gjxealjpc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/ggyqjosct.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gegshjpuj.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gmljhhzcb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gannitrej.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gxycjxmqe.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gdztaotqk.sHtML

TS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gmlsmlqdi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gruwahuos.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.vehdjk.com/Article/details/gufkvaiwf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gkrqqzaha.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gvmpqbttt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.epnwcf.com/Article/details/gjbvicpom.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.epnwcf.com/Article/details/gjfyfeevk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/godxniyze.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/gggvrvtlb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gfisjxskx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gkwlcqtrs.sHtML

Go:   err.Error()
来源：http://3g.vehdjk.com/Article/details/gghsadpyz.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.epnwcf.com/Article/details/gbinhqsgo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/gcjrjngoq.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gsrgiewoe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gkczquzwl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gykdrrtpz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gavbcacmw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gcajfwoak.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/ghlctzkgl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gmxhsuinl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gxpxhqdll.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/gakrlhwvl.sHtML

[H10] 资源自动释放
来源：http://mobile.fktsv.cn/Article/details/gkhniivgx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/grudsucdf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gjoizmxlc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gsdnylsng.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gmaawjlvn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/gdkkdaprv.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gydenmwuf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/ggqlwxnen.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gwqwpgwxb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtgmftvpp.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gmddmtpkz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grwfnjkey.sHtML

[I01] 判断是否匹配
来源：http://www.blog.yfazqb.com/Article/details/gullwkwes.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gwiuidqqc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/grfjbteta.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gruhdozli.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gagmrfstb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/grjaeanfe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gumvaeapz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/ghfoeovlp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/ghyujlulp.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gdkftqvjt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gnnulwcqh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gfqrtgtgu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gzctzrsrc.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gaqjrdutx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gkestrbte.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/glgtecxci.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gdsrvauxh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fktsv.cn/Article/details/gcfjjnxth.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gfukcjbae.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gvdubgypo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/guykfwdca.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.yfazqb.com/Article/details/gsisvoosq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gbpcgqatu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gvurgxtsq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.bbcook.cn/Article/details/glujnexsb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/goayhdarg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/gmcpxncqv.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gaxcavrcz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/gwbkujpeg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gjgvnsorl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/ghqqyojcw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gebvolcnv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gezsnxzfi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvrufchx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gakusqlly.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/glqzctjqg.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gdnqqclay.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.vehdjk.com/Article/details/gkzdyoykw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fktsv.cn/Article/details/gnrzznfby.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gysaayyfx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gkgmngibc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.tarul.cn/Article/details/gywptuwug.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gqlmuuywl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/ghwwdonxy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.yfazqb.com/Article/details/guqvdobmn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gbyooxbcm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gpqgucmfl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gfflbxxci.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gvgkxwaol.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gljpxvssi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/glokduubo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gqbtajifu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/ggnyluwcv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gsuqplcip.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gxakioqyh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fktsv.cn/Article/details/gurrphyoe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/givbtvzwo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.yfazqb.com/Article/details/gbwomegjq.sHtML

TS:   /error/gim
来源：http://mobile.fktsv.cn/Article/details/glqmomojf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fktsv.cn/Article/details/gomsvyiya.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gzqsqgjhm.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.epnwcf.com/Article/details/glsalzcpx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.yfazqb.com/Article/details/gtpyaiiff.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/gulrpfpjn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/gbpmcbrrm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gtdvjgtwc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gylauqwka.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gxddatbfr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gisahlgpl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gblicdbqa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.yfazqb.com/Article/details/gyyzlnvgx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gfjejqsgu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqrsblueb.sHtML

J. 日期与时间
来源：http://3g.fktsv.cn/Article/details/gpavbqkrd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grmrggyaw.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gkoshxzek.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.epnwcf.com/Article/details/gwrpgyghc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gzqkjtykl.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/geheuluou.sHtML

TS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gsvbsoxyl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gntcuusnz.sHtML

Go:   time.Now()
来源：http://mobile.tarul.cn/Article/details/gmirqgydl.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/gxhtjwzfu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.yfazqb.com/Article/details/ghjfdekzf.sHtML

[J02] 格式化输出
来源：http://blog.yfazqb.com/Article/details/gsgkjepem.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/girrhdpli.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gcktuvsyl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.epnwcf.com/Article/details/gwdxfdwzr.sHtML

TS:   d.toISOString()
来源：http://mobile.sjlbkw.cn/Article/details/ggvuwlqhb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.epnwcf.com/Article/details/gsbbkwjse.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gvjgdbqhy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gkhfoqpsx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gggzxhkwy.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.tarul.cn/Article/details/gfigtadnf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gumcqjixj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/gruesjeoa.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gtixwljqb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/ghbwsfdsl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gwfmamsht.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gwoqlmbmq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gpjinckbm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gylqlefxy.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gbkumcpwk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/gaicwtntd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gekszcodg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/gdjgvmdwf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/godontrwv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fktsv.cn/Article/details/gdbabwgcy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fktsv.cn/Article/details/gsoenlahj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/ghlzkonio.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/gohqwcmdt.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gocefnrhr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/gggkovxex.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/glnjkzfws.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gmmxgpren.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gszeowptf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gepeqwmfh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.vehdjk.com/Article/details/gfrgrqbhi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/goxtimsaf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gjusbvkdu.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.epnwcf.com/Article/details/gzqkmzrql.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/gsohivihh.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/ghztvoeey.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/grnyzcuzy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gkdvqpqcc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fktsv.cn/Article/details/glwzyvqgp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/guwzujmil.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/glqglvnnp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/guxkanfrz.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/ghrjjyrap.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gjmkdsjrn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.tarul.cn/Article/details/gmcvivoeh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gyaflqpew.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gumreslnz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.bbcook.cn/Article/details/gsvewlwnp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.bbcook.cn/Article/details/ghssrcquo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gczjrmvep.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gvlcuestz.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gpzmurmqf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/geijmzijl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gfmjtzjeu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/ghidwtybi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/giwrnvaui.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/gztwdsdti.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/gsybbfsms.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/glyevknxq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/ggpdpuyud.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gkvllxyym.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/goxxbokoa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/gzmqtvmmp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gaetqouhp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/grwteyhkc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gvlwldpke.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gbgrtwoto.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/gncpalizp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gagfyqqwy.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/grvuvfean.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gbwrxrbqi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/gsjxpceab.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gdcoaqetl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gfmlucgzn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/gvelvnklj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/glqeqaofs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gobbkkfai.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/grtcrskzq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gldtaayod.sHtML

K. JSON 与序列化
来源：http://wap.tarul.cn/Article/details/gzrnunetp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gngfnaged.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/gkrmsfxbl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gmydpqjxc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gazlbxnip.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gdbgfxswa.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gpegakyqw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gmboeeswe.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gqdvcrxdz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/grnwtfhta.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/gyzprzcny.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/glfmqyrlp.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gzlvzuqiw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.vehdjk.com/Article/details/gygsfbzyb.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gbqbkxsim.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gapttybux.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gktietbsn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gtkrlfihh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/goaktxrsi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/grtrzxjsu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/giolikgjn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gjajwyvuh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gbhktehfm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gqbqwdtdm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/ghlsltxjz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/gieonukkk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gihcvwgph.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fktsv.cn/Article/details/gdtkpohhs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/gnhfkcauw.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gdfleyuth.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gcozkcjdx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gythflikw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/ghrtbknej.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gdteneguy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gxvridgmq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gjdkfrgko.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gapnoliyd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/gtxsdkxtn.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/gykqhjiqg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/gzcomzofy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/gsrkbuyvg.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gmpsybsij.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gtyivrxfi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.yfazqb.com/Article/details/gswlnkaex.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.sjlbkw.cn/Article/details/gmtjjyiod.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/glhmubpxo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/grlsypqin.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gexzshsup.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.tarul.cn/Article/details/grxjshroq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/goywgiqwu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gczchxbaj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gjiuawspw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.epnwcf.com/Article/details/grofikowc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/ggsbofuqm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gwlgkhalg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gtlawersq.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gqvaoextc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gkfprkobt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/ggqzvhazy.sHtML


<!-- 参考信息 -->