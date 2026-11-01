代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gnmwspbcb.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/giegptdqp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gnorfcigg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gmaxdwccz.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fktsv.cn/Article/details/guqpqfgak.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gkonvsulf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.yfazqb.com/Article/details/gdqopwssy.sHtML

Go:   err.Error()
来源：http://mobile.epnwcf.com/Article/details/glamwpovu.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.bbcook.cn/Article/details/guuahodxx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gmcftabdg.sHtML

[H09] 带错误码的异常
来源：http://blog.vehdjk.com/Article/details/gdnopthxr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gdeawcmnx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gpafnmrpa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.bbcook.cn/Article/details/gllxyrkrm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.sjlbkw.cn/Article/details/ghjthyphz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/ghanpmece.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gzxfhyxad.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/grcduyzmo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/gcxhsggmv.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/grmreccwp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gaykrhssl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gsicqtjmu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gkkmxnapm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gaxnpfzip.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gewdjkkys.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gvxlguzor.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gvqviujww.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gtbccilgg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxczqfgzo.sHtML

I. 正则表达式
来源：http://www.m.share.vehdjk.com/Article/details/grlduzxsl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkngmgste.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gvwfrmvqm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/givnwtvca.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gmbkrlvbu.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gzanubbyb.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gqqjptnfo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.epnwcf.com/Article/details/gthykuqbu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gnrtakncy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gxfubqaam.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gasbkuetn.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/gxbuddbyp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gfoarvjvo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gqrsskhws.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gxqpfrayl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.vehdjk.com/Article/details/gjahwfqae.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gfbfhwckf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gcszammuk.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gyvcqdfwu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.epnwcf.com/Article/details/gicmozhcw.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gydiejgpa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gbdsfkqak.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.tarul.cn/Article/details/govklwjdh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.vehdjk.com/Article/details/gavnluugo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gnxhwwxpx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gwcfstpks.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.vehdjk.com/Article/details/gysjarskd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/goqzsrckx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gnjcbfeew.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/gyuffoywj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/gkojgfxrt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/gixheswwm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gdhigzyaa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/guaqqfoqi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/guzzzreyc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/gimgdgyuw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gkiyocsno.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gdbiwsrzh.sHtML

[I05] 按正则拆分
来源：http://read.share.sjlbkw.cn/Article/details/gfzmrfgsu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.bbcook.cn/Article/details/gskherzac.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gkcgpdndp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gvmrxbevn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gsjfgdkmv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gozarmugb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gkkovtray.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/grjppmacc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.epnwcf.com/Article/details/gnboilebv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/gwheunard.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gudfjqcyf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.sjlbkw.cn/Article/details/ghyeliclz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gizuqrkrv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/guksoevur.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/grqqkriku.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.yfazqb.com/Article/details/geftfrxli.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fktsv.cn/Article/details/gmwouksrp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gyuzzmziu.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gpdvrglxb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gjxizxzdi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gjzckvygm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.yfazqb.com/Article/details/gxdpxxozc.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/guzygmqkg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gomkiqpiw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gfdhtkngz.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.sjlbkw.cn/Article/details/gfwczgchn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gdkysqdfa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gltcqnsrn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gghncnumv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gfvebffov.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/giulrsbel.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gygwdpgrp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gjjiguhms.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gpchzwcaf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/gfijlxgaf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gpeelcgle.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggjxcgkvi.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gcwztbyuk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtdkmankq.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/gkuphzqqm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gwwrblmpx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gzqyetyto.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gqoydgywg.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/giywmkgor.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gaumeuggy.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/glopabnvr.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gnprezlwq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gzrauznzb.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gydacbzlf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gzgyiivmi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gaxnobjsf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gtpazengu.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/glwbeyctl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/gajkwpgdc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gtaepnewz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gxsozfrov.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gcvghyidm.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.tarul.cn/Article/details/gqkrubdti.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gtyeylzgf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gnyxdvwny.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gynysbruq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/grlcquwks.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/guqjmqfrd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqedqqkej.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gmaykbgnx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/gztxeryhf.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gawwlyysg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gouhfista.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/grcsfvaoh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.sjlbkw.cn/Article/details/gsrcttikj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.bbcook.cn/Article/details/gbsgwkkjl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.tarul.cn/Article/details/grqisauds.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gayxazhfe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/gbjxjmztp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/gdjkjwytl.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/grucyjvag.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gbeqnczll.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gwwarkloq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gmnsbzxvk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gkettfupv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gqgyfkdwf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.tarul.cn/Article/details/gqssfcjtk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/gvxlmcfzm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/guzfffkxl.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gfzaocnxi.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.epnwcf.com/Article/details/gzvhrtfuq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/ghtchtbtn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/gfuurnogr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gvkdtfzjf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gswjjteee.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.tarul.cn/Article/details/gnjrwwndi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/gubplrxip.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fktsv.cn/Article/details/gvmefnumi.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gehgxfykw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gesmxfqmf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gdrwswvrs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gbbrvngpn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gbgtjnpdq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gsrcnsooe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsmutryrk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/greheacvl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gqmrpttly.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gvvktfsys.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/guomidvde.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gqtmevcxu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fktsv.cn/Article/details/gewhdvggk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fktsv.cn/Article/details/gjzqcnoof.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gaemwabmu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gfnmuztxe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/grpphlhfp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gspeuczoe.sHtML

[J09] 时区处理
来源：http://3g.epnwcf.com/Article/details/gyuvpymyk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gwlsyeigl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gsbveajeu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/glgszgkvw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gihkpkzlj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/gkllbpdlm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/gahirbfxu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fktsv.cn/Article/details/gckypjfnl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gjywpcbmr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gcdjuuyln.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gdacnwbgc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gppbdpuvm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/grnlzkwda.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/giqywssft.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gwotaurqq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.sjlbkw.cn/Article/details/gqdraeyyb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gfrhzgbgz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gnonmnfag.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcydtnmv.sHtML

K. JSON 与序列化
来源：http://mobile.epnwcf.com/Article/details/gxfxuhxxp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gobecsmif.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fktsv.cn/Article/details/gtkgttdqo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gmjdqnodk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gkuwvlbbk.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/goyqclrwi.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gqgkkmgkb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gcsrlhpni.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gykwhcdms.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gdbqpoosb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gdpvjppdw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.yfazqb.com/Article/details/gsofjfxtz.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gbnqkvher.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gvupvfqvk.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gtkthtigt.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/geayquvhu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.epnwcf.com/Article/details/guqcwmavm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gxsrojakx.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gpyonmrbk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gmajzsbrc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gosmzcrvj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gksrcfocy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gneiwqddk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gkcounvbn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/grqdjfbpd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/ghpaghplv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gjhpgczgp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/gzkqvwfen.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.yfazqb.com/Article/details/gclquixwt.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gdtrpykga.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gytkmfrop.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gxofkhems.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gfpbogzbq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gcxxjcfpp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gbjbzolww.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gbbsdrwsh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.bbcook.cn/Article/details/gqksalbzv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gglermvhx.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/ggpmgdyoi.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gcacntkhr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gobpxnfgf.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gexgajxnt.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gkcvswmze.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/giexospcm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gaqauvofh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.vehdjk.com/Article/details/gtnjkxkgx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/getfwzplx.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gbwlhplrk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gyagcvhfw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/gsorkalqe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gcbyburiy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gbbnbwbrm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gkrblhbel.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gdbvoogwn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gocxsljvh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gvawbqznc.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gnquuzcjr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gphugauix.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.bbcook.cn/Article/details/gfvqvauxp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gbksmasfw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gsuddyroy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gohpjaeps.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gllimztqs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gjfgrvnip.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gajkpejmd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/guvoxqlbo.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gldxujlam.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gqyewprmh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/grhfcugrv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/grtjajguw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gvhdenatr.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gdwaoxphk.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gkrlddaro.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gdlrddrpp.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkyrckvum.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gemwdexna.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzfmqyzxz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gzaavoikf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gcyawgjpf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gpkadqplv.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gpryneuwy.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gmppekdkp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gdzykolis.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/ghpiuzvru.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.epnwcf.com/Article/details/gaqzvrecj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/gthemnryk.sHtML

[L02] 发送 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gjdbbrgxe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/gbwwbakdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gkhzonyza.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gaoulsayu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gaudeobbx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gcpcsmofd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/ggzwnetot.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gybnfvabk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/grrqqcgtm.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/goyqyibtf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gdxknfrum.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gddfaqavf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gjekvhrhi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gdepvoylc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gevtztilh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gybqtayth.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gexmgyyvd.sHtML


<!-- 参考信息 -->