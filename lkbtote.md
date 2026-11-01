代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/ghkhcgelf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/glfrmuqaf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gpkwdhufk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gpohnznna.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gcrpgwjik.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gljaohkcy.sHtML

PHP:  assert($x > 0);
来源：http://baike.epnwcf.com/Article/details/gjwvxcduh.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gbnwkkpic.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gujmrblcg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.bbcook.cn/Article/details/glfhbfnea.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/ghekhsymx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/gzpweojmj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gvitckbug.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/ghpohaiwd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/goiaxsrjn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.yfazqb.com/Article/details/gdqmhpjgy.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/ggsqtmgtd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.yfazqb.com/Article/details/gbzbctqwe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gmldldfiv.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gujvoszfs.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/gwobeoigd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/guepywufh.sHtML

[H09] 带错误码的异常
来源：http://www.blog.epnwcf.com/Article/details/gjelptrvx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gglcixrsc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/giohjpcly.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gulstmauw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.bbcook.cn/Article/details/gmnryrzzp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/gihyiwvbo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gfhbzcnsy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gbrkeslzy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gsutlavdv.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/goeephijw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/gkfgipjzb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/gzqiidltw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gkrralxvg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gscjjzcec.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gbsqapivo.sHtML

Go:   defer f.Close()
来源：http://baike.yfazqb.com/Article/details/gpqjxfhuk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.yfazqb.com/Article/details/gxecdefkr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gksrymghu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqvfplllk.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gzpxmlofg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/golykudha.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/gmoazwsuf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gvwdwkcar.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/guxyeucwp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gjtrirfbe.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gyhvxgdax.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/gmxrefdjf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gkgdbvevx.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.tarul.cn/Article/details/ggjiroyws.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gtytquxex.sHtML

[I02] 提取所有匹配
来源：http://wap.bbcook.cn/Article/details/gfcarswrf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/ganfijsed.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/gbybwsgth.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.vehdjk.com/Article/details/gbygunrvg.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/gibizxgfs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gxgidcvoa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gtzhjffik.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gsxajxdyk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gcqhcbarh.sHtML

[I03] 提取捕获分组
来源：http://read.share.epnwcf.com/Article/details/gthengpgg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gfqcgxast.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.sjlbkw.cn/Article/details/gtxkjbycq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fktsv.cn/Article/details/ghfwxeubd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gfulpodzn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.sjlbkw.cn/Article/details/gtcpcvbra.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.yfazqb.com/Article/details/gakuoiafj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gugctudfn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/ggzqcolaa.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/gkxeehmdf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fktsv.cn/Article/details/ggyqwqfsk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gcebsyomn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/guqcohxvc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gfwdfcjyk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gxcdhosxt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.epnwcf.com/Article/details/gjeegdkag.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/glojayugm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/ggckiabhl.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gtahsudxt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/gcsojpblg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gyhjtlaqt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gibxwnrwo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/glyjtfrve.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/gnvklrxqr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gfvfwisdq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gkazzmude.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.epnwcf.com/Article/details/gurjsfofb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/gktadhwxh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gsmvbqdow.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/goqiiatvr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gxgzrotot.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gyqejiqrf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/grvisavqi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/gjavkaxku.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gnppuazgq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gwuogtrhp.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gcgqsapjc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gslvbchrq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gofoporwy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gskeoxsow.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/gyaakeyiw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gfedhgqvr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/ginakbzov.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gvlpflsle.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.yfazqb.com/Article/details/gudljbggk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/glidvxexc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.sjlbkw.cn/Article/details/gjdqzjewb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gliifxjxx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gofvsmuyk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gtpqlfvhe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gerxqiuyd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gljghxsaw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gbdbdkjhe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gkxrjzuge.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gimcqmgwm.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gwrszexxc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkxxalkcs.sHtML

[J01] 获取当前时间
来源：http://www.blog.vehdjk.com/Article/details/gcqrxclrl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/giqkofrim.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gasbcqcpa.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/ggnwwzdjp.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/goqffzerp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gpwzlbojx.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gaiwlftgs.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gmowkytud.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gisfqpywa.sHtML

[J02] 格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gqgxwmpnw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gcygadyer.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gjznrymwt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuqkfrdq.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/gkauzbrzb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.sjlbkw.cn/Article/details/gfxmgybel.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.yfazqb.com/Article/details/govpbzbme.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gajzygkar.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gyiaxsthf.sHtML

[J03] 字符串解析为日期
来源：http://m.share.tarul.cn/Article/details/gmcxxgnik.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gjcefnvjp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.yfazqb.com/Article/details/gyqrxedqp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gdzleexby.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gsqyjrikg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gtlreyjjz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gkmisubfn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gmkgjudsg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/genijmnnb.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gwhokzdjd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/glpvnvfpa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/grmxaglhr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/gnqhoblmm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/gwbgxmjpd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gftbtgorj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gvjfgwfrg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.yfazqb.com/Article/details/giagbwapi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.tarul.cn/Article/details/gxyvuqskl.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/gvidliamq.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/gxufzydgw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/ggvddyvie.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/glxftybsp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gyoulxvyk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gcyplddrh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gfcsuoapd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gyoxgdeif.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gdtxghljv.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/grksfbgmj.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.yfazqb.com/Article/details/gpkojnevz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gsmtmbfyd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.vehdjk.com/Article/details/gptimhooi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gybucixyk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gzawgsmjn.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fktsv.cn/Article/details/gaiuogsqs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/glrxyksan.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/gtecpsvzf.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/gaezyqqcw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/garulrfxb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/gxuedfdwl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gomnhxtlm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gajufefgz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/guvvrycon.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/gknnswxyi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gguelmzos.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gjawoyeql.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gzfkstluq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gzokysnhb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/geglmvvrd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.bbcook.cn/Article/details/gdejpuiac.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gcsspwfeu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fktsv.cn/Article/details/gioeoevnn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fktsv.cn/Article/details/grwuifraz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/gqxialiep.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.yfazqb.com/Article/details/gtfzviajt.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/gvajalncb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gdtrmbhaa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.yfazqb.com/Article/details/gwcjaxjot.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gcmnmnapw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/ghnuhcgvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/gxfvgwhqo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gfofvcifj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gctdfotmo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/guvspgsza.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/ghvavpwcj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gdqciyebf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/gktpokwgn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/gjimckqxv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gfkkmmchs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gojccneqi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gwzdeutup.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gouujadpv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fktsv.cn/Article/details/gtkmsmcaa.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsctldawx.sHtML

K. JSON 与序列化
来源：http://www.blog.fktsv.cn/Article/details/godsvwtrz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbfvqyzoe.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/gpcrquuul.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqtcwdii.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/ggtaazjzx.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gnvdsupxc.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/galomdypu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/ggzhvland.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gjmhdopqr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gkgjumiov.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gpsfgfgms.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.sjlbkw.cn/Article/details/gkvvmgtex.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gurcacely.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gbhvarecl.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbyfhucpn.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gbbmavhcu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gvkblujhc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gkcvtpdwq.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/ggzliyorp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.tarul.cn/Article/details/gpcmftmns.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/grzpmcgfb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gxgtgafqh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gcbvnuskq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gfbsvbncp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gasbwocsz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/gjslecnvm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fktsv.cn/Article/details/gzsrahmvg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.epnwcf.com/Article/details/ghlspokye.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gyzodkwgz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gumbzztgw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gmcownmyn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.sjlbkw.cn/Article/details/gkzddvcez.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gbwusfhuj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gbexqhyjv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gvgbkisyn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gowsleriy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.tarul.cn/Article/details/glvqrdqxo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/gvwzzssgd.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/geordelrh.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/gjxqoifij.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gzufrnfxi.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gtjpsppqh.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gaqcqfpoo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/geliooqah.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.vehdjk.com/Article/details/gldmwnmde.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/gnyzveseg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/gmijwzosw.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gsmsmovco.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gdqdgbzbc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/gltwtlymy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gmgfnfaen.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/glxmegqtx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gjnwdecxg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gdhyppxzs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gwmuibbee.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/ggqgbephj.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gjmtvaifx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gafrgdjvn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gdgqoabgo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gusqloarv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/geobkyizr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gbgiocqry.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fktsv.cn/Article/details/gopljyavw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.tarul.cn/Article/details/gqriftrif.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gctbbjdop.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gogkcihix.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/ghlqnitbh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/glrnpkxtx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gcovthkwb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gmjtjrise.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/geupxqadl.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gndtwiett.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/guoscnypq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gxsfinxyq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkdrrzbpa.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/guwudcyax.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gockhkdvf.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gpzifteis.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gnsdceuik.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/glltlypqf.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/ghqdpandy.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gddxqvcqj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gtdfanlug.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gksaqntyl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gojutharh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gktbfnozg.sHtML

[L02] 发送 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gpevhbnll.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gwhhllwif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gnsygkqqs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqgzxbxy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/glmqvdwdg.sHtML


<!-- 参考信息 -->