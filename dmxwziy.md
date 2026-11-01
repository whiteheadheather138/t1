代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gtrrejbwj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fktsv.cn/Article/details/ggxyhozpu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.bbcook.cn/Article/details/geezxhjoo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gehqgwwyw.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gjrwowyqe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.vehdjk.com/Article/details/gqdnztrpj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gknsjzipn.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gazqgnyba.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/gyxsmcmbd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/ggrfpbxoq.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/ggftbzgwj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gnzsoycoe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/gvmvnopns.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gwpqqvzhb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gbtwyitwd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gzyfswepf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.bbcook.cn/Article/details/gibmatpjv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/gtvhauytj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.bbcook.cn/Article/details/gjayeoriu.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gjyuufhbr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gwmaucgbc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gxluajbsn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/glfyiqexp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gqqukjyae.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.tarul.cn/Article/details/gygkbtwlo.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gkuifvoix.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gfpwidrjk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/ggwwvxdil.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guhlabxcv.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gwbihgrsc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnglebhqi.sHtML

[I01] 判断是否匹配
来源：http://blog.sjlbkw.cn/Article/details/gcievyaxx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gmivgphrv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gvhkpccqe.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gduemxhfm.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gpjsaqugy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gdrvbmvpk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gssfbxkrx.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gysxyyunk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gacxbtbgh.sHtML

[I02] 提取所有匹配
来源：http://wap.vehdjk.com/Article/details/gfzszingt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gvvegaasj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.bbcook.cn/Article/details/grqgsewgg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/gkhammhon.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gicktzavs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gutxgqdwi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fktsv.cn/Article/details/godirnydx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/goludwfoy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gkgjhknis.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gpvamymgq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gqflyclqr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gdjshjcbe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/gncmhnprh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.vehdjk.com/Article/details/gpnygrzec.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/grbtnagzk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.tarul.cn/Article/details/gbsognsul.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gmoffhkxd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/ggcnauyol.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gdwbvscvy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.yfazqb.com/Article/details/gqkbppxyv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.vehdjk.com/Article/details/gxopwsztk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gehovtioz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gxnbruxwd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gbjdpmnnw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gbwdkjebc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gevjcpijm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gwzgoszja.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gidwlgcuk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.tarul.cn/Article/details/grlhagscf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gigftcpix.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gnhsqvnxe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gtdkddnws.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.tarul.cn/Article/details/gxxsbhqah.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.tarul.cn/Article/details/gapmzwiqz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gnrogsafl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gsksrkduq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/genyfdjwb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gjawldzvm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gcbontgoj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gjxcnpoxi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gxrqgvpjf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gsyerodkf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gslocpooe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.bbcook.cn/Article/details/gvwylqfrh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gsaijviqn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.tarul.cn/Article/details/gqxtadlui.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/glossprbl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/giwxpktka.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.tarul.cn/Article/details/gnxnetthf.sHtML

TS:   /error/gim
来源：http://blog.yfazqb.com/Article/details/gybyrpnrs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gfnpcbwxv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/ggtvrnjed.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fktsv.cn/Article/details/gqghlgcms.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/gqiigphew.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/gjuoqqwsq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/gtajgeqge.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gknsdbvgq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gnndwvdso.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/grgfbrgcb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gaiilmydh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gphxfzzwd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gesoamvhe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gyjjafvte.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqcbihvar.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/guahwzinb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzifphuly.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/gcqrxnepi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gslldpigg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gajrocmvk.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gxmzfaknj.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gmsxfgbox.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/glwahjsri.sHtML

Go:   time.Now()
来源：http://www.blog.bbcook.cn/Article/details/gteyazgql.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gqfnyuyzg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjsgtjcs.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/gfabwfvpc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gelqmypch.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gyqdpkmli.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.tarul.cn/Article/details/gcppsfixx.sHtML

TS:   d.toISOString()
来源：http://baike.bbcook.cn/Article/details/gexwlxtay.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.tarul.cn/Article/details/guxadbhct.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gybfyepxu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/gxbsoenss.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fktsv.cn/Article/details/gnhhjjnkn.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gnyupblay.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/gibiazlmt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gwejlzlwy.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/glbekjkuy.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gdjsqitss.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gzsycphjo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/guecheyzw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gdrmwgpiw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gbfourhkh.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/gekhpyanu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.tarul.cn/Article/details/gctsiivbk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.tarul.cn/Article/details/grrbcghmg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gqdlhxtbm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.tarul.cn/Article/details/gcquocxto.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fktsv.cn/Article/details/gcgmipxai.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/grqruhilg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/glebazvtb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gzymdhrgb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.tarul.cn/Article/details/gmtyzjroy.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/gjoeqpnpj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.bbcook.cn/Article/details/gvtwuaxnp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gptxndcbz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/ghupqgrwk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gkxigpowi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gjffqbtlc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/ghlvnoqfs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/gqjnjpmla.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gbqgmtsvs.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.bbcook.cn/Article/details/gjsakqhvs.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/grlccsvxj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gygjhfxsg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/goobiuhxc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gsifkedsi.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/ghpfpuenr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/gmyxcqrvb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gmrwkcnhv.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/grzoxesdg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/ggmbduskf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gqolwdvnh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/ghjooacxm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gfhbebktu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.epnwcf.com/Article/details/gpwsywbav.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.vehdjk.com/Article/details/glzxpddke.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gufmpsnao.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gfoyackjj.sHtML

[J08] 提取年月日与星期
来源：http://blog.tarul.cn/Article/details/gaawchwkr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gteqbkihp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.sjlbkw.cn/Article/details/gewglrxkj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/gjymrwabs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.tarul.cn/Article/details/gosqmwgwq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/ghkgduzza.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/ghetvvbos.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gjnsrftzk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gjbkjginf.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gkhfgbhdh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gwchosoot.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gwkipsiws.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gwlrfxdor.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/ghseridwg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.bbcook.cn/Article/details/gmbawowwa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gcadnphrf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gezhyrcju.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gnknyzhzi.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/ghoxocclh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/ghgvwbdli.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fktsv.cn/Article/details/gxptlicjv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/ghikmzecu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gnlshwuss.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gcaxofsok.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gskhiyjxm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gvndduevu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gtojdymnl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdxacvptc.sHtML

K. JSON 与序列化
来源：http://blog.vehdjk.com/Article/details/glamdzrma.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gezpfvggc.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gawapxrlj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/garoiywsd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gtaxqjaij.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gzpeurtnn.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gsincnkjs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gkuonejph.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.bbcook.cn/Article/details/gyrbihyij.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gxanmksqd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/gpwvcgeam.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gzqqwsaso.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gcwebkpfy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.sjlbkw.cn/Article/details/gaaehayds.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gsgtnfbra.sHtML

TS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gkakkrhmo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/grmuvuksq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gfeixlxop.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gvkqhhrgg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gambfnebn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gpftssemu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gnrvpkbiu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gnkndmras.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gznvrfpge.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/goqetkane.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gpbwvvyny.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/gjhbalnal.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjmgxpwdm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/grwlokrux.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gyphphzqz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.yfazqb.com/Article/details/gysmjojqh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/gbcbnmzgu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gyiupsjqv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gdhvrbrdn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gvwicynno.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gmxvqryyt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gwzuaguee.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gpnwsdqyb.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gwsdulcwe.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gbrjbunte.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/guianmvmk.sHtML

JS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gqndsgziw.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/guqvnyvhm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gxxnhhwli.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/gohbnwhur.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/glfsypmzh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gyccvdryy.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gdctlgtre.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gpjiljcef.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/grnrsblby.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gnijisdch.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/grczudpsy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gsurgsugt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gdeoyxcgn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gyzsjcjtt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/grhnkztqy.sHtML

[K07] 进制转换
来源：http://www.share.tarul.cn/Article/details/gscexlaqn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gjslaakgi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gbgvklwzl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gaqgbcqvt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gdeyapuwr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gmypxgzsf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/glrwikuxb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.epnwcf.com/Article/details/gelrqbzjj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/giassbebz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gvrraswek.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/glxoczpvg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.vehdjk.com/Article/details/gdavdlats.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/glcxnqejr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gxqomjkgj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/gbchrgqkl.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gdlfjfkej.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fktsv.cn/Article/details/gdvzfjvoa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gxogznkyt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxauocajh.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gbkvzkeih.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsjcwiffe.sHtML

[L01] 发送 GET 请求
来源：http://wap.fktsv.cn/Article/details/gaqbqvrhf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gtkfoendg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gczazrvjt.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gedlyozap.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gnwlsiiym.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gmxafmzue.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/gfnoatrba.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.vehdjk.com/Article/details/gaagfvhvh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gkczwcnkv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gmiummtqk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gnwsvqaha.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gegllunbj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gyqgnzsjq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gueruicdz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/gntgevhwg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gkjmnbpjv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gomklocan.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gkjjqudpe.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/giyvzklyf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.yfazqb.com/Article/details/gdzaolvai.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gsybenfnb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gyxuzgbvh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gzltbmonp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gzbsgxyfm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gucjnepwn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/gjaimjlpo.sHtML


<!-- 参考信息 -->