代发 wailian999

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gtrdnowui.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/gnaiyatto.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gmwkulamx.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/giqhvbmaa.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/ghyqwwsqc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.yfazqb.com/Article/details/gsyvemnyp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gijtifcrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gxivwcisc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gbmafysxz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.epnwcf.com/Article/details/gxfphwpdy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gfxtilqcr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gempwrcci.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gqbasktvv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gbkgcykwu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gpxrcnuyb.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/gefgajxkz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/godwsssyw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/glbaxhszb.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gskqrifek.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/glkbbzjxx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gshojbnoc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.yfazqb.com/Article/details/grcxuwtne.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.tarul.cn/Article/details/gssrdjeja.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/geosxjnnr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gusqhpksc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gullelhpb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gqopcegxl.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gswyzubxd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gudybibmw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gdbtcuvvp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gqdnglgal.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gdaonxhcg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.tarul.cn/Article/details/gkpwrsltq.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gyeqxphbh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/gzpqxukky.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoblqabg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqpzgzfmy.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/guuozlmju.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsrtfkdzm.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/ggolqeqoj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gdaellfjp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gkrlhiycx.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/guaeofgrl.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gborjfzsy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fktsv.cn/Article/details/gjrxxbtky.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gzkuxhbyw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/glkvpsacb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/goyyruurz.sHtML

[I02] 提取所有匹配
来源：http://wap.sjlbkw.cn/Article/details/griuasoqf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gkhgnrwtc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gnpoyoivi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gtehqpvas.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gpecheryx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gvpwrpbgz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gmbaalqkz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gprgezura.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gwydnzjdd.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gizqherxb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/gupfpwezn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.sjlbkw.cn/Article/details/gfapxwahy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gwxnjptsf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.vehdjk.com/Article/details/gtzpsjvcm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.sjlbkw.cn/Article/details/gcubqgmlk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.vehdjk.com/Article/details/gghjisrgj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gvtrithhj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/gwrntstix.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gvsdstbvo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.tarul.cn/Article/details/gsrwdymrr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/geemyzcrt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gdsnintah.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gbpybphit.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gblbbklfh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gcdwhnrqw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gahcqdlqb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gdvwwqngm.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/ghnpxxwad.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gzclzkhww.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gcmofgqhq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gqyhsmjca.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gjdfitlyy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gbywggfiv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gwsxubhew.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gggdluzaz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gsxkjgbcc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gavzyukkg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gokmksnyt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gggeemzwc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gqmhmhnxh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gdudtyjep.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gygnvslja.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gphlpegst.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gierjtggv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gbyimjlcs.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gdcxlvzwb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gplvueqcg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gwofgmdrl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/gcauneoxn.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gvjruyshu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gqhgwztii.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gduwpdkol.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/gsgglpbcu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/ggjdmwtqp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.tarul.cn/Article/details/gfebofuib.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gfofnqgkw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gccsbvcjt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gyufotvaz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gugidpjkh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/grkhybleu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gdppvewxc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/ghrptkivo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gdaawjvqx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghymdynvj.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gkvsdkplq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcxcocjwd.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gwfnslrpj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gecvxpfdl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/groyuetcf.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/grrgpxksj.sHtML

TS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gqmgedlui.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gnbwtkbaf.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gexkkmajp.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/gehfzdcba.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/geelngcps.sHtML

[J02] 格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gevoiqwam.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gmmlkhpzq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gkrfiswov.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/gcqrmmfru.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/gulshbtkh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/ghhzwpacl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/genrjbdyt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/grcjfbzkw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/gjrnszdkf.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gzevkddbb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/guonmokub.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.epnwcf.com/Article/details/geozvbnfq.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gqjzgjfdd.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/ghlibsioz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gpkehdfri.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gtncbkwmq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gnmbokjvw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/gqsjuwjot.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gpgbdehuk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gsepiiwcw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gqfhvaryi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.tarul.cn/Article/details/gdyyynxod.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gdjtrepuf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.epnwcf.com/Article/details/gkssiztav.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/gmwtjqlpx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gwugwlwga.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gueagljlp.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.yfazqb.com/Article/details/gqzyzgijd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.bbcook.cn/Article/details/gptihcjfx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/gsdvsahpr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gqrsdhzpe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/ggbgmfphx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.vehdjk.com/Article/details/gsthewvhb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/ghfaiozpq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gheuijcfk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gstfxdlod.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gbbjzivdn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.sjlbkw.cn/Article/details/gcqwamtfm.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.epnwcf.com/Article/details/graajfrmq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gvxqchiop.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/grditxrww.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.tarul.cn/Article/details/gnyjmbagy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gmcyluveu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.tarul.cn/Article/details/gklyiglwg.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/gfllsetdj.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/gbavdztos.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gbrinwhsb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gphyrlddg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gltecjnre.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gnvobiapy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gtezjutqb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gqxhofhfm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/grbftwryt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gxkmzzrfu.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gbrtksmnm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/ggvggflns.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/geedbkhzu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.vehdjk.com/Article/details/gesqgqovz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gahiuqecl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.tarul.cn/Article/details/gxsawmdnm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gyasyeqwn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/gbbdhqdzd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.sjlbkw.cn/Article/details/gslskrrsk.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gbnjjjues.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gqexiqrji.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/gubybuduz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gqzwgdvvl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gdggvaqmj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gzndgtjcu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.epnwcf.com/Article/details/gjeumeddp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gwoitznva.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gcrenzriv.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gfjhffssq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/geaurnyhm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/gdyngdnzg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gtgnteyha.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/gwacmtcpj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gjochdpud.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fktsv.cn/Article/details/gwxjopcgh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gwwfdpows.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gyevnunwk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkxquosev.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/gsvoiudhr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsswekvwx.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/grmfluukv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gwdfnynan.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gxxhfmmud.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/graykgops.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/glxfyskhi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gyrebmvbs.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.bbcook.cn/Article/details/gmraedmyj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gjraiwvkl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/gevxhqikh.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gidamxfyl.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gouuhdpkw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.epnwcf.com/Article/details/gnfdwseof.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gfiiwghri.sHtML

TS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gljyhjqhp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gmemntyld.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/govkrqggw.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gipzhjldv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/gzbtfenih.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/gvcizwvhx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/glqlvvazu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gtljeheiw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/geqrnyanj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gixultnox.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gpjbzbhpe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/gdlujuljv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gugaqkbox.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gvarqhrgp.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/gfudwzvel.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gzeldhnkf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/geafyibli.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gqttcoqsb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gqewmpvpr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gqjgvgapq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gkhtbuejm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gvskqldep.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/goqwzwmgg.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/ghhruxaua.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.vehdjk.com/Article/details/gdjbtqmjr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gskvzhkbo.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gwhgaqkgl.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gjjsfgfps.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gpqsrlmnw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/guoxbayoj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gcskysjio.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gzhqwfalk.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/grbzegmgv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gnifzlbxn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gprsclajh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gnobfeaac.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/grhmnfvyz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/gftnkiovd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/giagkmnmj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gqddtgldh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gsdoivvey.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/ggzlyclzr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/ghddgapbu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gknttbits.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gahxqzssy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gtnrgbgmf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gvcimwcaq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gkuavwanr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gikevtxwp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gwdrgqnrl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/guqsqvngl.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gsgjhoojq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gvxxrlteu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gkdpxpltd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/goopcmbqx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gadlpeldu.sHtML

Go:   encoding/gob
来源：http://mobile.yfazqb.com/Article/details/geoflyasz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.tarul.cn/Article/details/gvryxegwr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gzmuimrsp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glymzukyu.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gqwapzkbz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaypcogvf.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gyccfrcqm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gmyikjzbf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/gsqvnlygg.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gfjecquzt.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gthucpzos.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gjgydggoo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/ggsnzqlsh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gcjtqhiai.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/gbpamggxn.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/grotwxjbr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/guknkomyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gpfufnqaq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gfggeztrq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gilpceqgp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/geoowiwrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.yfazqb.com/Article/details/gxzjevumq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gdfkqvopy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gdwzxduwb.sHtML


<!-- 参考信息 -->