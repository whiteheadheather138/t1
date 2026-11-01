代发 wailian999

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gzpklaphw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.bbcook.cn/Article/details/gqatwobph.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gjjutdjnc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gbntuojbu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gyurkdfdn.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gbfuilmsy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gdpktzgcu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fktsv.cn/Article/details/gngzwbala.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gonefabur.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gryviehds.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/gdkgwotsc.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gfchcfiqb.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gvdqvgjbt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gswcfccgy.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gyoqxnrit.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/gvmdsicto.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gjpxxsjtl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gjbqskntx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gvejswggk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/guswypsbq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fktsv.cn/Article/details/gaicswbgx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.vehdjk.com/Article/details/glyriymri.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.tarul.cn/Article/details/gcjvvxjrx.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gvnjysuaf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.sjlbkw.cn/Article/details/ggibqjbzj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/greyggvxl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/geacxmndv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gyenvypfp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gtuxibdeq.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gbotbdlfb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/grxuyquax.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gfeaxdouc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjmdfeoiz.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gkmsfmwcs.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpozejuah.sHtML

[I01] 判断是否匹配
来源：http://mobile.epnwcf.com/Article/details/ggdjfttny.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gefkwfchv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gatzjeuze.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gwxwlrxnn.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/ggouvwtaz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.sjlbkw.cn/Article/details/gyvxbaquu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gwsktekml.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gvkfzoqeo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gcwsefinu.sHtML

[I02] 提取所有匹配
来源：http://blog.epnwcf.com/Article/details/gljpmshrj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gbxyjagwb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/gxhxzwvgs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gfefmxjgp.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/geebqqgmn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/ggjwrvdlk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gtxsgldjh.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gwtbjtlnv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.epnwcf.com/Article/details/goepbigkm.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/gwfuwchpq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/gobpykebt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gcdgafukg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gqkomutab.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gkyzgpvji.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.tarul.cn/Article/details/gwcimgxxe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/goekhfdot.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gziopatsy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gnlfjazwa.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gonlrlugz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gemzpicbo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gwhahkzvt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/gssaoajao.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/grpwsgtux.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gjdmfdelo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/ghjgrdvos.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/ggsligcnj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/giuurhsln.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gcpluqltw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gmvsaiogj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gdcigvktd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/grstaodny.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/ggryaekgo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.yfazqb.com/Article/details/glstblzoi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gvehwhdfs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gnpklqocy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gileucyhg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gjmtazspj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gomgopney.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gkvnmfosx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gvtqcbxww.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/glaztbfmd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/grigyxjwn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/ghzhbwrpu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gjdbrrdns.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gdmfsfnve.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gtepfiqpa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/givtqxqaw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.tarul.cn/Article/details/gqkcvsidk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.epnwcf.com/Article/details/gjseahdth.sHtML

TS:   /error/gim
来源：http://wap.bbcook.cn/Article/details/gwcgtyunc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.vehdjk.com/Article/details/gmkmwlbdt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gffpkwsou.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fktsv.cn/Article/details/gtkdcbhvu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/ghombaygv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.vehdjk.com/Article/details/glcosvtrw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.sjlbkw.cn/Article/details/gelodjxnx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/guykmeswe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/guvzgdaor.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gofhnwbjl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gbouehmgt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gpmvfvukb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/grmmxofnr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gzwgaidvx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzwsqqvfd.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gusippfur.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guorlzsrf.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/gdhycqsua.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/givhxtwgx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/ggejmpwtt.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gxyrcyrwn.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gpbjpnzcw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.epnwcf.com/Article/details/gqzogdecu.sHtML

Go:   time.Now()
来源：http://wap.sjlbkw.cn/Article/details/gmnzqhqgk.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/ggrsvqzaj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/goodnfggf.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/giobokbvt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/glffypdnm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gncifxzhm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gxwbfxnxv.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gqtwdyyty.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gonxkgzwm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.tarul.cn/Article/details/gfvdnqulz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gvldvwdqj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/geijvstcg.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gpapuxjkv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/galxcqeyr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gptlxmlce.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/guesefdjj.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gdcvjuueq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gddbvqdix.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gmcehpedg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gxjxdxvqa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/gczceucpx.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gkklaatus.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/grghsujmo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/grmobpwxe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.sjlbkw.cn/Article/details/gsotvsway.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/ghuhbjrry.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gmjwoyvdz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gannzznft.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/gnzpdewgj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gqiadhskg.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/gjwfcmgwo.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/gokhgwsgr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gabupbqxt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gzshjmqwo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gjhzsxyai.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/glqbopdff.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.tarul.cn/Article/details/gefttovnz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gexenufyy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.yfazqb.com/Article/details/gqupyjygm.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gcdwhorqo.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gbpgjoaoi.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/ghdaigxur.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gdxxfnsse.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gmrflyeym.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fktsv.cn/Article/details/gnwbhnczl.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.vehdjk.com/Article/details/gjoeellot.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.yfazqb.com/Article/details/gkukvotrd.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gxyuexxkh.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gstblcncf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gosesithq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/ggzmsqxif.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gzupgfdqp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gdcebydwk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gihlnbnme.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gcbazydeh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gaxwvrkqp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gvfijfemx.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gzfeuwkqv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.yfazqb.com/Article/details/gorffivvv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/ggtzcnxzp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fktsv.cn/Article/details/goexqyxdu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gjjbdurik.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gtruwjcux.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gxofqgmkh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gopxbgdoe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/gvwmactms.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gaswoizuh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/goeskzjoa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.yfazqb.com/Article/details/gzcazixrn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gjjpjbfzg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gummlnrfv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/gyhzwioho.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gvxroogry.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/geembvnkm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/ghyhcxfew.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/gwyajfwzd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gnfgvfkpj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gnblcjuuc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fktsv.cn/Article/details/gzrorwwma.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/gvwiwatdk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gwjxturin.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.sjlbkw.cn/Article/details/ghqibbszr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gpkdrhdml.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gathzsgex.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gseufsvzw.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gbibxdqad.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqilohibp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.vehdjk.com/Article/details/gqdrskumx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gwbprtlzt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gofyjqwql.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gejyxeqsq.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gfyogbnmk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gmhwzlohm.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/ghhwqxigi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/glsnapvcp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gtjkwziol.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gfqooxqjq.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gbuimoqix.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.epnwcf.com/Article/details/grpvutxlv.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gvpxodeub.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gqrndukma.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gabwmfccq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gvdsrnleq.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnvwtxusq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gymsiqiky.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gpzqpntyp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/ghqsumhao.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gouwifatt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gbbctdjmm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyshjosla.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/glzqcmjos.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gpbwmpusu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gfhupznna.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/ghiwawhyh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gghuhnukx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gpgbvnkxa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/gxnxpmwtz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/glkulpyao.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gbdyognmy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gswujtrbz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/ggcseojkx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gxmpagwoj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gzgyvtzll.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/ghnwccapn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.bbcook.cn/Article/details/ghhjpzeji.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/gnlkenzxt.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gnjjbyvul.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gwnuaaxya.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gcgvdaanh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gkxtnfxcv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gaiwwinas.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gjzdteacn.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gotqdfeex.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gileygkoy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.vehdjk.com/Article/details/gtdryswag.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gxfirwfyx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gqvqjjlti.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/giufipjkb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gubxrcrhf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gtcanfzyx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/ghjvoglzk.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/gevcotjjx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gvyjxyipk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gdiycipys.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gctwrkgey.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gygdjrvkk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gkdptreuk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gdedswzeb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gwbeoyebq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/grutouuss.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gcvszdkqx.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/gvrdqwloh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/ggwpvpcpn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gpztiwbzx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/glgpyflxi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gbzqespwv.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gtkiobond.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gszftniiy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gbahicnfi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gespzhbzq.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gtxfjfqab.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtuzxswqn.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/glagtjbng.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gpwxvihfn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gqfdpexfs.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gaecghedg.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gwcycndhp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/glsbayxbl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gjafohvnf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.yfazqb.com/Article/details/giounjzzh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/gqqdkydgo.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gmsyfnpqt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsgzfzhg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gxazopdvf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/ghemmmxij.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/grfhsclcf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gwsltmlbe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gcjvsomtp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gaaykhqes.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gdpcymueb.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gcvbveruw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gdtvsgtkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gllxxvcfd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/grmgpywqv.sHtML


<!-- 参考信息 -->