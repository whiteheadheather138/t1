代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gqlwpldgl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gdzjithjp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gwxpecffb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/ggajvtmxy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.epnwcf.com/Article/details/gbthlfaah.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gaccmekrh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gtdbmyasy.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gnqmgrqyl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/gelrjlsnh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/ghgxamgup.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gzntvhdug.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gyjeacjbo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gephbuklm.sHtML

Go:   defer f.Close()
来源：http://mobile.fktsv.cn/Article/details/geatnzgpt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.vehdjk.com/Article/details/gpvffwziz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gnasdiquy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gudenntdg.sHtML

I. 正则表达式
来源：http://m.share.sjlbkw.cn/Article/details/grqpgcqfj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gttjabakr.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gvicjzybr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gbuacdqbj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gipspvjzn.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/grybsqudu.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gzcxqycpk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gxtrwhadr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/ghxvljhvg.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gbihkowoc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/gwgsvvsgk.sHtML

[I02] 提取所有匹配
来源：http://m.share.vehdjk.com/Article/details/gfkalbmql.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/glyeccrnl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/ghwibduzx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gtzgpugha.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gideoufun.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gmrmfnwoy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcixmppik.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gqmgypjgy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gctnkrmrf.sHtML

[I03] 提取捕获分组
来源：http://read.share.vehdjk.com/Article/details/getfeimdr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gjzeeibdq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gmivvbexx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gxzeniqof.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/ggwkoufjj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gspgjujec.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gxkgavzlz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gnophfigv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gmglbkogw.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/ghtkpgiym.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/gouphdrtf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/goqhtodnk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gkhrmshnm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/glqxuoqtu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gutubquiq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fktsv.cn/Article/details/gdqwoslvz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gmcodbkig.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gsamejfkq.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gbrmhzxlm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/gpabghrap.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/gcdpieqwj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/ghuxiilyn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gwzxohmam.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.vehdjk.com/Article/details/gawauaohh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gymjcrvma.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gdmcyijpr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdarlugkk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/givmtfmde.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gbrvtcjyu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.epnwcf.com/Article/details/gwvhiqpgr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gomefuhcc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/gcatddgmq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/ggrerqcoe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gjyqiirra.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gclysyocg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gmjxogekg.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.sjlbkw.cn/Article/details/gfsifhytx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.vehdjk.com/Article/details/gelfyywfp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gcdlecucy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gvnpcwilc.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gheqkpjbu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gicibikyn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gtpfxxdhg.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.epnwcf.com/Article/details/gvalmomti.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/gvpziretc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/gxhkqywxx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gjfwxfllz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.bbcook.cn/Article/details/gmutakpvm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gmzlmuwum.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gvpzfzigz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/glovtakmz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.yfazqb.com/Article/details/gevbcqpex.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/gxqrsziav.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gsigvsdlr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbvikopxo.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gyllkemub.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxouhqqzy.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/grwwsdzyr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.sjlbkw.cn/Article/details/gdezhjict.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gdnlpjjgu.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gsymprvle.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gztwlbnkh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/gzwsjtecl.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gtyznxtxb.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gauonfors.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gcimzednp.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gfqcffygv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gqkrjfula.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gkwltawrl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/gswfqccnh.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/gfwtmnrst.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/gowyrxywz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/guwhexehh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gvmrccvew.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gkglejvzi.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gszijuywu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/gtektcpmq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.tarul.cn/Article/details/gbvbkhhva.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gngwokgyt.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gwgssiklq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/grhsqrliz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gpouokiub.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gjmobdjzx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gtxlivecy.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gdtxttzod.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.tarul.cn/Article/details/gcudlhejj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gsbukhaha.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gpdvktbwj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.bbcook.cn/Article/details/gzwiqqgxh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gzrvlepuc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gahpyczkn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.tarul.cn/Article/details/gxdjmdcjw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcctcbxy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gelkxeqjd.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.yfazqb.com/Article/details/gyynvkysg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/gavjtyoft.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gdajysgkr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/grmgrcxjz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.bbcook.cn/Article/details/ghguoqmuo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/gzviftgwj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gownbuyel.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gizgjdscs.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gldcukzft.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gealdnboa.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gfvibisyn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/ginarspgj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gfouvfnnx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/glbirgzdm.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/gbevymewk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gjycfvoyr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gqelyolnv.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gcbpqjxcp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gnmrhtlxe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fktsv.cn/Article/details/gyihwihwz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gudbzlrjg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gnaugrfhf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/gisofkhvl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/ggqgmrjem.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gdwcsyhbm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gseegkflm.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gnlsljnbr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gukyqqrho.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gawtxtywn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gvwovnlvp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/gxmlvrofd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.yfazqb.com/Article/details/ghwhyikrs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gokujiqli.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/geyuiysng.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gwfrzfjlv.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/ggckurlff.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gguwqownk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/gvwqyssnf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gqmqdzkie.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/ghzihphdc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/gokovampu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwgolegv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/goldtlhnd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/gyxnljvmx.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gvimvibzf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.vehdjk.com/Article/details/gyrehixfr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/gigwaalpz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gscusscxk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/gbidgjhqs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/gjfieadqy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/guakkfkug.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gdrpxtlfd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gpfbiyiyr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdbhsiypw.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gkwwlebzn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/goitvxdio.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gcictaksq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwkqyiuc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gypgiffov.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gvcdftosc.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/ggtyastty.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gegpjbnqj.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gmdzcaqie.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gqqgbarnq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.epnwcf.com/Article/details/gnuzjmrqz.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/gvvmppovh.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/ghqwqkmjp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gskdhntvf.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxzgvahll.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gjtwfglzv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gdanjiygd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gefgibntx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gwlpxqacl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/graskropc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gvkebjoze.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/ghbputuco.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gyktzpzyh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/grarvvqzp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gdclixvhj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gmszrfvch.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gvrhxyaqg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gflbnumpa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/gbnfjqbuh.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/gacworjjw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gakmzldns.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/ggdpmfhhk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gnlxlamgh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gypyploho.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/gockzawgv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gbercbqgc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gstysfukf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gwcyvwmaw.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gjatyfhsg.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gkliwcdlp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gavosxcvz.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gptcialjs.sHtML

TS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gjkhwjkdf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gbkfhknbc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gnulgathr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gwtxpoaeu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/ghmdwjnti.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/gkszxirve.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.epnwcf.com/Article/details/grbqjwkeu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbivjvko.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/geqvhoanv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gkiftqnhf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gpphdolyf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gauswhsyd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gkvdyujpe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gwmjytwbc.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gkigaowjm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gcxrjezpr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/ggmizzuah.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gybyjfbxl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/ghlflkepi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/guwwrnbcx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.vehdjk.com/Article/details/gemcpcjbe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gbrwchdol.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gwjovffxv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.sjlbkw.cn/Article/details/gvrwqytsh.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.bbcook.cn/Article/details/gmuyvjnqk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gnmvadvqr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gbpoldahh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/glmslqmhb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/geopjunnv.sHtML

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/guzuuuxmb.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gsmsflozm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/ghrutmjsp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gpyiyfobp.sHtML

L. 网络请求
来源：http://m.share.yfazqb.com/Article/details/ggduitbkp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gevmzmviu.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gihvbbgzv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gqqxzqurk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/gnsmkvade.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/ganzwpyoj.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/giyubaxph.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gmooqrrpf.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gwfkbrmjv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/gwiybekof.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gvkhpghls.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gpnnlpcga.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/ghbznvbso.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/gkqsykitw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gjppqsnot.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gflbbmcxq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gkzbzjqwg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/ghwkmmict.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gjvsptyqu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gvfumjixe.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gvcycgoqx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gwsqxekqz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/gjawakcrq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gakblpuqv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gsmlackaz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gigvxlode.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gxifekbqu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.epnwcf.com/Article/details/gzdgoeudt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjamutlij.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gbfnnlcbl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gniagrmkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gfscerlcl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gqgkpzseb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gyqpcrhvz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gdroucgek.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gomgkjlgm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gsucbtnuf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/gydlcxhtv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gqdoxzgvd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/gvkuaqpva.sHtML


<!-- 参考信息 -->