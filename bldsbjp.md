代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/giqbtytli.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.vehdjk.com/Article/details/gfszuppeg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/glbchzcvc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/glhuowzwz.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/gmgvsphqd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/gddwknflh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gniwneceh.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/goxslljdo.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.sjlbkw.cn/Article/details/gqnzaripm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gvbdieibt.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/ghixrdvrj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.tarul.cn/Article/details/gmulamfrx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gxgmmjqvn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gmclqakhm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/gphgrdcgo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmgfqqjn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fktsv.cn/Article/details/gusivwybp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/guyxknsyj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gyrkjpfih.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gomrfacyq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/griiczkji.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.vehdjk.com/Article/details/gaexungqa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gfzywmwkl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/ghwzxfzmg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/goknpycgb.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gegkyccwj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.tarul.cn/Article/details/gpyfdxkqg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gylectjrw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/goqnzzbnq.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gamjxvuad.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvwqlekyg.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gpmypbjeu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gymflcync.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gcxgsieft.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gsintjzna.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gaxxertwl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/gfrtowszn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.epnwcf.com/Article/details/goptmccps.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gckwkdpts.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/giqhgbdyg.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gssmnphoy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/glrxvgdtk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.vehdjk.com/Article/details/gklbttmww.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gmuocsioz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gbaxhwsbu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gdaibxxtd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gxyayxtlm.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gzzioqkbr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gsnotinvg.sHtML

[I03] 提取捕获分组
来源：http://wap.bbcook.cn/Article/details/gdngdpxut.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/gqgclyfkl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gootepjox.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.sjlbkw.cn/Article/details/gnxseypwj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/grwjnzrrm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gqudmbixb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gcirjzpqs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/gbgkyvaay.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/grbldpgvd.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/guxfeqwus.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/ghqfyskqt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gkgjfkqee.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gpqkdnepz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gjsydxhkq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gfwvtulna.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gzggomulz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fktsv.cn/Article/details/gingupfrg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gpzdvktav.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gpvtnfpjq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gzeczocuk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gxibziivy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/ghjsdqrjo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gmpksksfn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gfymjvxoi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gsuqktnmi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gcctzkqwg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/ghizefhqi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/ghxrbubwl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gqjobwimj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.epnwcf.com/Article/details/gpavczefv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gkjdaqzdx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/giyjlmqcr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gjarfwkfn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/gyolseble.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gdvlinyec.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/grfeckjvw.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/goyqhdzmb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/glsqyprbv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.epnwcf.com/Article/details/gtucdzjqc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gtpsevdhu.sHtML

TS:   /error/gim
来源：http://3g.epnwcf.com/Article/details/gphngqmiw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.bbcook.cn/Article/details/gvmibcwaq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gciysvgkw.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.tarul.cn/Article/details/gmkccfkbm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifjoxwel.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gbgzbaltg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gtncolspy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gvkjbwulm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gxqsfwvtq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/grmwiptby.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gaabvbflq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/gapmzfdab.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gzpqibbob.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/ghempxklk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glvobpmol.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhibgkci.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gevidhlmh.sHtML

[J01] 获取当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gmdkrbzeq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.sjlbkw.cn/Article/details/gllpgpvke.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gqiunmeuc.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gtemhxvhw.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gqhfciwyn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.vehdjk.com/Article/details/gqgwoosli.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gxmjfalbo.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gxgwaukpb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gzvqgzhql.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/guhgjyswr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gotoosonn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gqfgefmzh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gquorvcrt.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/gwbtgiztw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/gwstmhott.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/gxayxvirl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqykxnqf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/glsoeglvx.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/gjbofuhgv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/gbzebpybf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gzpeiyjze.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gtzzxrjjq.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gsmsboiwk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gvcgsunze.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gxmftwlms.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gvosrtpfj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gkwcltzxz.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gsayucoqe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.sjlbkw.cn/Article/details/gseasaoie.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.epnwcf.com/Article/details/gyovmqfcf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgsmvjfk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gearjjdch.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gcpnjwdxx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gicmqieev.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gwbexyoxb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/gkddenfnh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gqygpchgr.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gpbjboxjr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.yfazqb.com/Article/details/gfxhzxwwn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gzedyyiim.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/gskxmhswj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/grbnvuscz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gugwccylh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gcqntjysa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gkkxmlxbc.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gaxfykcih.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gbrpwqwyl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/gfkpabzxa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/gcawrvofd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/gijgxghve.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.epnwcf.com/Article/details/gmzhpwbvu.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/gpjvfizqn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/guilybhjf.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gkdqcscgi.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gzgwkydus.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/glequmeed.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gngnpsoab.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gloyydwmu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gaesztxts.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gtrpzljti.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gimaukajy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gpfjnbcvc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gmqmjexer.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gzgtamnzt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/getkukulq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/geqgtfrrr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gugtktsin.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/guswpvqfx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gujcpppqv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/gvxulzbyy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/ggkwbspus.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/gvvifpxad.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gbesfjdss.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/gocorrucd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gkntmjzpi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gvkjgyjih.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gebbgoghf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gpvpexloy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gqhfclmxr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gvsbrumax.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gvnvlvggb.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.bbcook.cn/Article/details/gulvrszky.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.bbcook.cn/Article/details/gmudyiqbn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.sjlbkw.cn/Article/details/gtyynuouf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/gfrqsdbbt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.tarul.cn/Article/details/ghtwtgfzw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.bbcook.cn/Article/details/ghworqmga.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gjqwuskyr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gguetkmib.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.vehdjk.com/Article/details/gzkhiqjps.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvhsqaeiw.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/gfkzwqgew.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gybofhpgl.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gdhoygsgk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gttechlbp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gsmqutbcy.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gghdtidgb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxkzyqnwf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gqwtjuost.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/gqpcszssp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/gdqecmavt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.vehdjk.com/Article/details/ggibppvwg.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.yfazqb.com/Article/details/ggtqfunsf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/geunovive.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gmjkuutpd.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gnnufovlh.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gmnwkvpzh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gzovepxmc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gaejhvymf.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzthmbcvn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gflfgumwl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gaspiwieu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gamfkzdok.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gcpdvcamp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/ggcoqqacv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/ghatwkjfd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.bbcook.cn/Article/details/gzsdtwxug.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gbyrxpkdi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gxlmyksnn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/glzstljjm.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/gxivwpeor.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gxmmihuwz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/ggzwbfyrx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/grgoblaba.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gchbbzfir.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gwfmecrdk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gbaplcftw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gzsxdokus.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gbnfsihdp.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fktsv.cn/Article/details/gdvdbehcv.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gwqwnizbt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/gahiwmowe.sHtML

JS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gqxyyovpq.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gkmdnxsmn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.yfazqb.com/Article/details/ggguacsen.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gilhlfpor.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.bbcook.cn/Article/details/gvrbadeon.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/ggeaufywl.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/gqyfbppoq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/guayelmop.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/gedvhaedn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/ghmjuefgr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gvfckagne.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gnttvvwsv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/guxjbboko.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gmcmmgqzn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gaktaenrv.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/gcxwdsohk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gakfppgui.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.epnwcf.com/Article/details/gsudouncl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gnckqrijd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gxyprhexe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gdmrcblcz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gsjvtjgow.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.sjlbkw.cn/Article/details/gmkkfkcvl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gpivhbdxu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gcxjcxhym.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwekovjsm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fktsv.cn/Article/details/gnskvtard.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gtbmzmpox.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gmslhgcpu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gvdxzgvlj.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gtselbjkt.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/ghyibsxxx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/giypwrjlb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcbznijii.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gltucwbiy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grjcynpel.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/glxoalalt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gjkgzfmrr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/gqxjjfmvc.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gwgkpzhlr.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gxjhpbotu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gcvpgtrsn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gnqpetjft.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/ggspsnxmk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/grbzcinbm.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gjfnsskxi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/ggbjmoldz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gghqgsvwt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gdpqstbxa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gsazjpyhj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/ggfnwgzje.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gjropbmku.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.yfazqb.com/Article/details/gkatfdqsm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/gwnysnots.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gpdipiqrp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/gxxwfdtby.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.sjlbkw.cn/Article/details/gqgufwgzd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gkokuqjuo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/grvkkwrns.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/guwgmuaxo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsazzsgpz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gwhhuuqnh.sHtML


<!-- 参考信息 -->