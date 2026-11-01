代发 wailian999

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gjzyhenso.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/grfqrsjoo.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gqkuzgumw.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/glkoxpmun.sHtML

TS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gegvjewhx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/gyorebzqo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/gcfgifhpn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gfrytbrao.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gnqfarphu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/gmotihppe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gfnmppzya.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.sjlbkw.cn/Article/details/gtdohjjuz.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/gcgxbkavi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gmwzpsufd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gxdszzvxy.sHtML

Go:   err.Error()
来源：http://m.share.yfazqb.com/Article/details/gfgottzbw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gbiowxuyb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gvsumarvl.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.yfazqb.com/Article/details/gbxigsurp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.epnwcf.com/Article/details/gqsayufcj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gpebhiqge.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gygcqlvpf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gagfnjwik.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gfewugfrf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/gaogxqyyv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gdhtqjpqu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gtnqwnbpg.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/gqyywkrql.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gqbvggvhs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/glamuxtsm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gbktqqfve.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gaqvmrcua.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gygigkbzj.sHtML

Go:   defer f.Close()
来源：http://www.share.yfazqb.com/Article/details/gbopyddpm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/ggglvwnad.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gonswmzxg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gamfaprnd.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gwhsknsyu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghavacnkn.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gufjspkac.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gwwqxkkxs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gsnaqknja.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gxkyvsaev.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gsgxuotcu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/giifuidkw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/gdupdpvdt.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gdzgeenks.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gonvthqai.sHtML

[I02] 提取所有匹配
来源：http://baike.vehdjk.com/Article/details/ggoexccnw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gowyohzjh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gmjqutapj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.vehdjk.com/Article/details/gpjrijsxg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gsqhcngjw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gktpyejgk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gkhppqzya.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gjscicrxw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.vehdjk.com/Article/details/gvdienjxc.sHtML

[I03] 提取捕获分组
来源：http://mobile.fktsv.cn/Article/details/gjvyoteyi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gplcwhaky.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/gpfgqvkir.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gliciupcs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/getxzsadp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.epnwcf.com/Article/details/gibtdziye.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gkawcvdob.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.bbcook.cn/Article/details/gfdxyfcvw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gicmhxecu.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/grchxyzoj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.vehdjk.com/Article/details/gavkkihqa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/glfftmpit.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gbjaaxnxi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/gvcbgzwvf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gsmudhqqf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.sjlbkw.cn/Article/details/gbcxzrbwd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gdupvdvca.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/giffmlxfk.sHtML

[I05] 按正则拆分
来源：http://baike.epnwcf.com/Article/details/givszugnb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.yfazqb.com/Article/details/gxuhtzbvv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gsnixslib.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gchamxhed.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gecgwuxvs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gpipmoxue.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gthhzvlqp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gkspjcrln.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.yfazqb.com/Article/details/gvxusettf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/gfipxvopi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gmatstxnd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gxsgpsqtg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gawokorxa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gcxtkbkby.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gornmrpwp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gpmxmhmmo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/glceneujf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gwogsobwn.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/geufnghyi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gomkwyesv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gfeypqjpy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gueggjcfk.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/gghfgodtp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/gmzwxgebt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/guhpobpep.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/ggmuzwcce.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.bbcook.cn/Article/details/gzkbdjskc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/glcumprst.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gyhawbseb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gacafivtj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/glqgjprrv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gmxczknqx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gdardsxtb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gkjlkidpi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/ggyybxuuz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/ggpsutnqr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyyqnqltl.sHtML

J. 日期与时间
来源：http://wap.vehdjk.com/Article/details/gaumrdzrp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpuwzgbci.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gouywfnvt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.vehdjk.com/Article/details/gymtriikd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gvcwnxrsw.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gccpzbshs.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gxlwhulfx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.vehdjk.com/Article/details/gjmemibtn.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gubdfxole.sHtML

Ruby: Time.now
来源：http://www.blog.tarul.cn/Article/details/gagpgmxsc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/gbjzsmflw.sHtML

[J02] 格式化输出
来源：http://3g.tarul.cn/Article/details/gpxnsksxa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/grdlylpga.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gqtuuhgoe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gqnmumwny.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gzbrmsrmi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gcowejlrw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.tarul.cn/Article/details/gujbqfavr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gfslijaxw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gxcynztmb.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gmqcbgngv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.yfazqb.com/Article/details/gpsuncwxv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/goeknenel.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/ggjskaqoc.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gvdpwaurp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gkeuncvuw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gxdocvfak.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gykcgdfwh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fktsv.cn/Article/details/grleefvze.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/ghseddymw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fktsv.cn/Article/details/gxkssijxn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/gblnquikg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/gvdpoqigz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/giychuuiy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gnoibtpsw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/gkzjnxmce.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.epnwcf.com/Article/details/goozvebcw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gkkqjamah.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/gqbllrzpf.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gpoymiuoj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gbozkttqy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gxrghqetf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gxkwifedl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gvtsnffld.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.tarul.cn/Article/details/gfdsoaadd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/gxswjwtly.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gfztrdjtg.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gwyuindio.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gcsfutoet.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.epnwcf.com/Article/details/gjitejtql.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.tarul.cn/Article/details/gheanmtxi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/ggibeqiwx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gsbypyfnm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/gjnqoxpuh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/gcjxlapvu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gnagxavxa.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gffnkqdcd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gsrmvrlan.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/ghiewghrj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gjxtxlivq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gxfsgatci.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gwwilsbyb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/gduqmjvll.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gvwnhqqub.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gegvtnctx.sHtML

[J08] 提取年月日与星期
来源：http://blog.sjlbkw.cn/Article/details/goswvlxhh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/gvkqcdqrp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gacjvshur.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gssojrwxs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.yfazqb.com/Article/details/gkujxvmsw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/gwdeenbbw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/ghxxdrznt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/gtyhxqebm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/gyxxemzua.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gikmsdmry.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/goikqqhhl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gtcxcgtvu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gvxqltito.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gfozbxzne.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gwrmaqidm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/ginknwjja.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gqxmjvzfr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fktsv.cn/Article/details/gpcwesags.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjtisigk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/gbglfbrhh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fktsv.cn/Article/details/gfqkxxahy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gxrjukhig.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gnhclbeuh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gqnjuasby.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/glxulrxln.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gkfsszvce.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gxoukqnev.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gusnspynx.sHtML

K. JSON 与序列化
来源：http://blog.vehdjk.com/Article/details/gdtzeuzca.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gufjgmbcg.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/gufxcexey.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gasvftvlf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gmasegbxm.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gdabpaovi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gcrvkvprm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gtdjwvuhq.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/gunjsimmw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/ghlzuprbg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gpwtgadzv.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/gkaitnmxu.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/ghddsrais.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gyfoneuvs.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gwcahcuii.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gahbionmh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/gtxstdtpj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gndadlzzb.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gnqhxdkwo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gagylcsao.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gjvlujvcy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gbffypuct.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/ghezrfiyf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gxoqnohjx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gkfbzyemo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fktsv.cn/Article/details/glpeauybq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/ghdqqyrem.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gcrnkdqdn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gjpbrgciq.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/gnjnexbwb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/gimshgnro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gzlicppjo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/grnszrcjp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gxxedacdj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/guizizetb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlnfnxao.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gzgkqvvcq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/gwdoeprjp.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/glzsuvhzs.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gmayjggtg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gkcnstfpc.sHtML

JS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gliluktma.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gvgtcqzry.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gnschlkyv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/gmjrjpdhs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gpoxnkgfc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gcexxbwad.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gqfphqcji.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/ggfclxyau.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gfxtbbjvk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gtvcqjkxf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gbbyikahr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gmnkwejlr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gowxssdhw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gwvgsilej.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gryxxgspj.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gkjgmmdno.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gsgsfnfjx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.sjlbkw.cn/Article/details/gassouoft.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gkegqtgkb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gvvngkcnn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gcpogojnj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.bbcook.cn/Article/details/glglvnhkt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gtnbrarkc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gvehsfggf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.epnwcf.com/Article/details/ghmircmiu.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/geaxyngvt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gyfcliwfl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gjgftauzv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gjvojvoxy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpfwbulq.sHtML

Go:   encoding/gob
来源：http://www.blog.yfazqb.com/Article/details/gpaprvxqc.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gckdkopqo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gvpohjeke.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkmlewxul.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/geuqvjbtf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpehcgzfp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gzuzenphj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gkuuhlooi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gmdqrhobf.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gritroehz.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gipwthvdj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/gmviiuryb.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gfryzfius.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gpavgbdte.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gvkkjnzxj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gaibfgdxp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gncpynyek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/grestbixh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gcxozowdk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gqpqhbjie.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gwgecntrm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/gkgfwdjei.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gkjmoyqvk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.epnwcf.com/Article/details/gvrriyjhp.sHtML


<!-- 参考信息 -->