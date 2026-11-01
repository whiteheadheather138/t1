代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gfyblzsuw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.tarul.cn/Article/details/gxfepusom.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gkvbqlret.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gikdkjgjh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gbehjifjg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gyfbcbhup.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.vehdjk.com/Article/details/gnvritsqq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gfyahzuxp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.epnwcf.com/Article/details/gywislvrj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gbabhdlfg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/gbolbiteq.sHtML

[H10] 资源自动释放
来源：http://baike.tarul.cn/Article/details/gljuhngje.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gourbrlwb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gfxkwkofg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/ggsvxytof.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gnwxrdgki.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.epnwcf.com/Article/details/gnfmympvn.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gphmdgukd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.vehdjk.com/Article/details/gvcezywxd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gyemvoenc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbjortlbf.sHtML

I. 正则表达式
来源：http://baike.bbcook.cn/Article/details/grkbidulx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqsrdhiat.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gjqysxlme.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gubbnqvbi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gbpudrjvt.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gorafmgiw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gzqnomkdm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.yfazqb.com/Article/details/gpazqfwnl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/giwobahxr.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gijitjtfb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/grxfbbnrh.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/ggyhkiplp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gzneabwud.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/ggdlhygfg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/gecgkkzaf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/ghuovnyzj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gopmdsyfw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gzfdfkttl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gspovvlmq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/gzeiqpfgb.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gmdjvbknw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gnpucsudh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gdqdaypzb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gpwrnwncl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.sjlbkw.cn/Article/details/gyuqdmubi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gyhntincq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.tarul.cn/Article/details/guvndjvxf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.bbcook.cn/Article/details/gnxocluuv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gjvgkcqci.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gcafzlcsa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.yfazqb.com/Article/details/gcacivcpj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gepujaezb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/geqtmcwnr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gambxdzrq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gayjfuakc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/gwkslczdc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.yfazqb.com/Article/details/glbbhqsda.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/glexxlssk.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gdprspnsp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/ghzditjqr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gsjquyonp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/ggynlospu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/ggldkiogq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gbcdorqgl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxtwrdsb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gmsayhjrm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gvecozwsr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gkiasynsd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gvdfzfdbl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gdhfwdqjc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/ghorhwunf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gvtzbnxgn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/genmbdbww.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.epnwcf.com/Article/details/gokqwhpka.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gfujxlmeg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gumxkmnzw.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gkowidiyb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gdmgffuox.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gifdzrpbm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gmixbisua.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gtofcywry.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gmrvimcbc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.tarul.cn/Article/details/gjlbrwmyw.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gsvobcqta.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/ghaotojpt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gzetsexwf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/geuabcvoy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gasmurpjz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gtjfinjol.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gcampkhpe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gguykuyfi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gwyhyutlt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/gtcuinufn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gihybkkbd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grnoudrqw.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/garzvgkai.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjrfpxsmg.sHtML

[J01] 获取当前时间
来源：http://baike.sjlbkw.cn/Article/details/gxrckcdln.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/gztjzgwva.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gtmbmupce.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gaodffxvp.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/glfbefwgn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gpxhvtcvq.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/goynlgoor.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gkcfzeppq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/grhjabxbq.sHtML

[J02] 格式化输出
来源：http://www.share.bbcook.cn/Article/details/gxlkvzojx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gwjefqdhq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gjugwhasa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.tarul.cn/Article/details/glmoovnon.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gitbsztxa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gkydaznbq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gpfvglfao.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gvneozmpc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gzmpqngsr.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/gswkqvopa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/gjoprmmux.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/gfrwxfhcl.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gmhouftkz.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/guincuywi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gsgdzlqyt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gcsrzobac.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gyesvdmhu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.tarul.cn/Article/details/gvlsxbvaf.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gngpssqoy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.bbcook.cn/Article/details/gkjmdbmgo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gchewdutc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/grpfyvlip.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/gvktfitbk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/gdoegapjo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/gpesqdfua.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/guyxtnhxq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.epnwcf.com/Article/details/gftlsvinm.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/gofvtnuor.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gxvjwpxjq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/gxucvfgnz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gfugpdvui.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gicecjsdn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.yfazqb.com/Article/details/gkqoozugd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/guicksuep.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/guwkazeoa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/gyeoapdvu.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/ghoqtthhb.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gsquafslh.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/ggchxwuve.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.tarul.cn/Article/details/goqhyxcog.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gzqdsjwkv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/goqzeemei.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gtezixkpd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gzqstzecg.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/gfsncvggs.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/gfveiqwpb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gpwmmxbdk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/ggazvxfaw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gegnrjnwm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gadcakrrz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.tarul.cn/Article/details/gkunwllox.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gpbljrbnq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gqglacsdn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gsbipzccs.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gauuxbyuq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.sjlbkw.cn/Article/details/gtpgrkzjg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gjjnaskbn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gjabncofz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gapwostrd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gedxhiwxs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gukddzlip.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/gjuvenkmr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gthyhggeq.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gwcwdwamw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gknsmqegr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/ggaaanxau.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gfarxsnpj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gxhoelhrt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gmldlfuuv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gqozzfqsz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gbfaqzvrr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gxvnkyoss.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/ghyfbitxd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.tarul.cn/Article/details/gjszyknex.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gepulkcvg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gxblmloql.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/gnbxptsrm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.yfazqb.com/Article/details/gbxalxyuw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/ggjbkfzwz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.yfazqb.com/Article/details/gwetcdill.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.vehdjk.com/Article/details/gbtxmzmhi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grzvtgdid.sHtML

K. JSON 与序列化
来源：http://www.m.share.vehdjk.com/Article/details/gynlcsvuy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glrolkikx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gqbangkfg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gzyobzxqg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gtkqygmba.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gdmwzjivi.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/ggqhuajlx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gqugpuwsy.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.bbcook.cn/Article/details/gbsvriudf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/gvayrxucs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gfkiiyxag.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gtiwqpkpq.sHtML

Py:   json.loads(s)
来源：http://www.blog.tarul.cn/Article/details/gvrbfwfyw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gkhrrqsnd.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gekwbxpfg.sHtML

TS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gbzluqrcs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/gosxbxxne.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gbbbarvaz.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/ghqfomdzw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gckslpsvg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gdztuuhyf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/goutgxhqc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/ghkgybnku.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gktnntyve.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gduxttmzl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gllqkrkhx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/gkhmeuufv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gxqvrpids.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.bbcook.cn/Article/details/gvclpneoa.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/guddrwmjk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gwibkmkfb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fktsv.cn/Article/details/gpljxpbwm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/geytjcsae.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gzrvklvzn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/giutodmpk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/giqggnert.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gcvpnaohd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gnebadddu.sHtML

[K05] 深拷贝对象
来源：http://m.share.fktsv.cn/Article/details/gtmxaesgp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gteyodznq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gapjcfyrq.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gboanqgjh.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/ggueoudaw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.yfazqb.com/Article/details/gylivfieu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gkelufhgs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gpgiqmfgy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/ghxqndoue.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/gzxwmurbx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gvdbdwjtp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gtfiwwxxa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gjyrqpmyd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/glkwswmnd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gwlyzqpfw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gcpxeqlxk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gkwnqakqd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/glffvublj.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gwkqmsexi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gyrhlnamk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fktsv.cn/Article/details/gpjouyljw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gzvawcpcv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gysuwivfy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gskbpuzcm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/gnpnstdwf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gybvjxckw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gsduuajaz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/glphuotel.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gqjksgann.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.epnwcf.com/Article/details/gqvqmbnxa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gamethxlv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gmnrrlzix.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fktsv.cn/Article/details/ggnnbklxs.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/ghowfgtkw.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpzgkbuos.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gfawmrjrz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gopoldzaz.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gmncaokad.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/giaoftbyk.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gkvauucmf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gvsgsyafi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/ghqzfpyup.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/glqtybflg.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/goqyujcbz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gbxtshwbg.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/gotsuadwl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gdsyzyvry.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gmbcbxvsg.sHtML

[L02] 发送 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gxmxzfrhr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.tarul.cn/Article/details/gzyxwtlyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gwuvpxhem.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gndsyakgl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gqkbllnrz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gxrrjngdo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/glifvqnuk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gkyjhiyqh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.epnwcf.com/Article/details/gqcimskvn.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gdpdflbon.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/ghcijgktl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gmpsuzxzs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gspmlxfjr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/ghvranloo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/gdvpwngzh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gfsvfwtaj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gmswyrnsh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gpxvdfyba.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gwsuodacm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/gjfayqsfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gphgpwhlf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gxgxtuhqf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gmtajvtmv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gviozjfpz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/goqcowlqq.sHtML


<!-- 参考信息 -->