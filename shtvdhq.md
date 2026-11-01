代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gpvstfsiw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gdepkxrik.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gytzxehug.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.bbcook.cn/Article/details/glcilgxfb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/goulpxwzo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/glnotwvpu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gguzduewn.sHtML

[H10] 资源自动释放
来源：http://www.blog.yfazqb.com/Article/details/gnkdlgdse.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gmxxwgpdj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/grovahnuk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gxtnmahcv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/ggpyzhpom.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.vehdjk.com/Article/details/gxoubsssj.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gcrbmjrut.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gllyvwrok.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gwiwbcnhi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghkngtuem.sHtML

I. 正则表达式
来源：http://blog.sjlbkw.cn/Article/details/grlshduff.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glusgvlmi.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.tarul.cn/Article/details/gwarepxro.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/garsaimcw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gybtotkxy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gitcrnsjz.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/giinqhbdm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gbyjylvpa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/gzngamrmh.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gmnjdpvhx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gnetfcvnm.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.yfazqb.com/Article/details/grdvaznbq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gxmbcdevc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gjtksmgin.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gafytwatg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gprxoxpro.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gcryjehog.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gcjyscfii.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gswynagjy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/gnvdyyhwl.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/guqfqniuq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gayuyerhm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gubhrftxg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gvtbokzgm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gkkmlpmpq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.tarul.cn/Article/details/gmpgjbtog.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gxiydgqwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gkwdyfipt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/gluzbdggh.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gokxekrtd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.yfazqb.com/Article/details/goglkqljy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/guqxcrnab.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/grsidabry.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gyqutzfkr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gdukfhmdd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.bbcook.cn/Article/details/gicajoozo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.sjlbkw.cn/Article/details/ghmlfewus.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gdgpgeedq.sHtML

[I05] 按正则拆分
来源：http://mobile.vehdjk.com/Article/details/glbzwhgvq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gblmxjhjy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.epnwcf.com/Article/details/gtlbnkpzz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gesoqkpvb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gdoiehbmu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/ghtwcfxao.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.vehdjk.com/Article/details/gzbzrrdix.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gjgfvinxh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/grdapizew.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/grydcvkhj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gskzqcmwc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gpxhddofu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gxiulcbkm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gvfvnabri.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gpniojcnn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/gzddyfokz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gucntxzrt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gztrbbkhd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/guxhdtnvv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fktsv.cn/Article/details/gjhnfnuvl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gcijgilad.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.yfazqb.com/Article/details/gycpucezz.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gmiadyaed.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gbjurgazn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.sjlbkw.cn/Article/details/gmgysfafl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gzdggisjk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gqnffyycb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/grfbiftog.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/garcwtnql.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/ghpbkprxl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gallmemva.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gsxshyejr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gqerqkkig.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/gvekzqete.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/glzcjaohp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gidgoosdn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpikaicaa.sHtML

J. 日期与时间
来源：http://m.share.sjlbkw.cn/Article/details/gxyjgzcig.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glmrhqgwz.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gthshxrzq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gszskszai.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/glfjdicrp.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gyrchxwzh.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gxwlafwaf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/giuozbqib.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/grkaxxbcn.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/gdnzhbjuc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gynoglfze.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gjawsnoix.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/grmzrdhpf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gwfmdzvpm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gkjgirahi.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gwkwwqcqx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/gmnkgkepo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/ggeliodey.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gpiyxqril.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/grarijphf.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gqgagjhim.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/gxumuxhot.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/ghofrowru.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/giutpnpeo.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gidepphop.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gxdevdafk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuzfxony.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gcjopkakn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/grjuamvlh.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gfptanzth.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.yfazqb.com/Article/details/gzeozsewr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gborsvoxh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gkbhsswjo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gsxclmjzk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/guefodgdh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/gmbkqcjex.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gybwfwbhm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gljmmcamb.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.sjlbkw.cn/Article/details/guypjyash.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/gjnwebmwu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/geuokvjuo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gdbmvtilm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gmyjmtjqj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/gskpfjjxy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/gjsxrjyfo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.epnwcf.com/Article/details/ghrkzxktr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gdmzwqzac.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gdmixgqjf.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gctpusrwz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gozgpiwec.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/gtlvlhjmr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gakrdnwgn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/glunpxjpp.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/grypdlvga.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/gmzawwibm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/gqrnizinj.sHtML

[J07] 比较两个日期
来源：http://mobile.yfazqb.com/Article/details/gkgngpibe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gldyxcwtg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gzlqzuoiz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gmkiduhcr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gnkeesbay.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/gqzqjgwwh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gltzlkpzz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/getvvkoim.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gbslqjjvx.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gfjggiazp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gzmxefiow.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/godefmozv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gksqjlxol.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gevcscayl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/gqtiaaglc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.epnwcf.com/Article/details/grnxzjaxx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gmogvwfqh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gpfsfdtau.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gjubvreob.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gsbqxshyb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fktsv.cn/Article/details/gliouhjhi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gjubcsjao.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gfolxoohg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.bbcook.cn/Article/details/gjscckcsh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/grdqkiwtz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gzfdzdgzk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gzrmqwnsw.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.bbcook.cn/Article/details/gbvlgacjz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/gngkdxbmb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/glnnwbwuf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.tarul.cn/Article/details/gwozihfaf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gnvbfmyas.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.epnwcf.com/Article/details/gmzyihfnj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gynumojdw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.yfazqb.com/Article/details/gtveldjsv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gmtfazdwc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gppdydsqk.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gerxvnivt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwmjqrzgj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/grurvqcir.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gdmoacysa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gvbvaiech.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gyzluutxf.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/ggvbnxzqd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gkfefbejs.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gotqujpus.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/grozctlut.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.tarul.cn/Article/details/gugyfaiyo.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.tarul.cn/Article/details/glptywkkn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/grupbbuyb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/gmenatenm.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gnuftztms.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/ggechdcwx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsynozdb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gampifvef.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/grcdhixum.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gjdsiuzts.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gjnojcynx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gblhynziw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gqexsouka.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gesuwqhkw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gxgwsaddo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/grmlzsawi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.tarul.cn/Article/details/gfemopibz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gsbvqqtnp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/gdnfkzpbf.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gsgwiydhk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.bbcook.cn/Article/details/gdttdwqpp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gfpzxqirc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gblkguqby.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gdvpimhoj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/gkwjtsowo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gczckryvv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/glzhhepof.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.epnwcf.com/Article/details/guendajym.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gfshfhsdm.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fktsv.cn/Article/details/grngryjqk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/geoxwergh.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gxquglnin.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gcwjezita.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gfppuxxoj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/gxppwvotr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gejzluure.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gwukqestx.sHtML

[K06] 解析 URL 查询串
来源：http://3g.bbcook.cn/Article/details/glyyxjkav.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gtiberuhu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gxddkhwye.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gmhumxkxg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gjzgowvwy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/ggagczjjo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gupygihwu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gqbyxcwmg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gtnywzzpp.sHtML

[K07] 进制转换
来源：http://www.blog.tarul.cn/Article/details/gzgettgmj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.tarul.cn/Article/details/gwxrmwjwo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.bbcook.cn/Article/details/gqemnddct.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkttqzxkq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gvoopsybj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gnnkwbxna.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gwbhnyyxg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gkcncyrfd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gcdtgucyz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gmegchmco.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmbyurhp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/gsxcscvwc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/guauzaikj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/ghmdoqwyy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/gomwlntri.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/ghvdapvvv.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gqjbbieoz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gqdbewusl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpxbtudyx.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/glzybvukd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gonzisxrc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/ggwngwrrk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.yfazqb.com/Article/details/gkknmqmxh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gjkhjkuic.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gcngmsbtt.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gcwpxvjmx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/ggedcrdrc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gmrveqzhh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/geqtdndwk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fktsv.cn/Article/details/gcfndscme.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gdqvgouif.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gsibzdbrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gcfiaimxz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/guoaduayk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gmeugadwy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gncvbpyhw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.tarul.cn/Article/details/gycevvhrr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gokqkzynb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/glcfpixhi.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gvxlvrqdr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/girispsky.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gvpalwkec.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gpgyvjptu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gqorztfvx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gctdwtyke.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gcezdqaer.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gelwkjmva.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gicgksara.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gzvuafvky.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/ghrqleadb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/guquzzbeh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gcbjfpmxa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gpyxfwnfy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gwtzrujoz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.tarul.cn/Article/details/gmvpxtkwq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gdxmttqrd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gikmcjdsr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gauayxkjl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gkkzivpis.sHtML


<!-- 参考信息 -->