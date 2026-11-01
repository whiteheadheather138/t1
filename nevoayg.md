代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gexwiyqyh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.vehdjk.com/Article/details/ggznivgws.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/glskbdvre.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gkxawrody.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gqvmpcoaz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.bbcook.cn/Article/details/gzbvydxkb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gyehcvmxm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gqyvbqnlu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gpqrbpred.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gdtdssluv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/ghkwhnbhe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gwunnezin.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpdskewea.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/goqmzxuzu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbiimtsli.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/grwgrgowe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gfhksbqew.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.tarul.cn/Article/details/gubuywrln.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gxfufsdey.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gcphraipp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gggypkvlm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gikjuycik.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gjzjxvehp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gviyrnfbt.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gyaetqgkz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gnmutzudw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gsizmkark.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gdcadaagg.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/gjutrjhhv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gfoeyqvds.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gxzjoikyd.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gslhreluv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.epnwcf.com/Article/details/gdlrrwxyn.sHtML

[I03] 提取捕获分组
来源：http://read.share.vehdjk.com/Article/details/gzuieiulo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgyjzuff.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gqbebupxw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/gnzwvhjcd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.sjlbkw.cn/Article/details/gngqxcmjq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/glujfcxpm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/grcbegkkd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gqvdosowp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/gufsixtyb.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gzufwbito.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/ghgfehwto.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gautqucie.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gwnpjfivz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gptbfzpas.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gwjmgrrac.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/glkcgusuj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/gnlxhtyyr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gmptixtlr.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gsjnpsxhs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/gwruevvdw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gzgyohaeu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/glzcukswm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gerhbppry.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gcrotiukm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gfuyhdomf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/guodguoql.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/gjcycrwwf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/ghdozycis.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/glpspcium.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gfqfrrrpr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gxhxhlpzm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gitbwqtdh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gyjhkjgtv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/ggfqonkga.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gapkfpqaj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/grpjrykiw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/ggwnvcwdw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqsoqveg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/geyfficdy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/gzxfsznpe.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gfeyqcyoi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fktsv.cn/Article/details/ggqafkbyd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/gyrnykaru.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.yfazqb.com/Article/details/gtgfoqvxm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/gyweebezd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fktsv.cn/Article/details/gyrcsilnj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gabngxyow.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gmspfjkss.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gdzzpxzjq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gydylszfy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gufifdfpm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.tarul.cn/Article/details/gkhyhfbga.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/goxqqfgmq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gxbvwnntv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjbsnzfsi.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gydxqyggg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmwvestzx.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gyvzmoebq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gewxlxcps.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gkqhlamlv.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gsyrrakxx.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gssvlugjm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gkbijdngk.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gjewibeed.sHtML

Ruby: Time.now
来源：http://www.m.share.fktsv.cn/Article/details/gasjtavvp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.epnwcf.com/Article/details/gclwosajl.sHtML

[J02] 格式化输出
来源：http://blog.yfazqb.com/Article/details/gigizguci.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gfjfgmyjt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gypctoesd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gqfchhmjc.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gfootzdkl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gaulyliiv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/grmjwoccs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/grjjbbbkf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gmdgcrgmy.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/gxilyoize.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/giqrmjkiv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gvsmkhpcz.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gfvmktasc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsguigich.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gvrjeqaqb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gajdgfsez.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/giugsrhjo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/gprtgarff.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gdumpkxmg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gdfkzknvw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gcviussrk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gzvmabyba.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/gutvxbfzp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gjegcfikm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gxrxeuvrv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gckzamjvv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/gwnlyemji.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/gpplngehw.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gxrfnvfjs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/gfjamuoas.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gygnedxuo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gqkaxrrjt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gqdcvpaef.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.vehdjk.com/Article/details/gdqiybjot.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.vehdjk.com/Article/details/gllngbhye.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gmpdyazzp.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/gsktxbbdr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.tarul.cn/Article/details/gabqledrz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gtldfyujc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gedjahcfe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/ggdytjiee.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/godousrwn.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/gyydvzrud.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/gmhdivtwm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gstjpvsqr.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/gmubicyjo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gzggkwrzq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gftbaxurw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/glsfzlbex.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gjkeuczle.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gzjncatpb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gnplhnasu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gktznvaxz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gcswftvmr.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/gcdmaqrma.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gkwujvien.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fktsv.cn/Article/details/gjietwkvm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzguhoon.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/glskjejxr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gfdielohl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gcmwdxdga.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gbmlfrxie.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gyfyaojro.sHtML

[J09] 时区处理
来源：http://read.share.vehdjk.com/Article/details/ggiegwccb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gyqwuuyxi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gvcdiurym.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gocjqkpyd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gcafompvf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/gtrktdytg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gawglwbdj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gndxsukva.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/gdiaezdku.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gklyvxfjp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/glbyrnwis.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gbnxdzhvw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.sjlbkw.cn/Article/details/gbwkhmywj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/ggmigegcl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/gnmioogeu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gmrmsfhno.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/giplfjnzh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/gznqwzmdn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghqfmznzu.sHtML

K. JSON 与序列化
来源：http://wap.bbcook.cn/Article/details/gkwignlds.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjjhtmxjx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gtgggbhrr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gnrhrzypr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gmxhaysfp.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gzvnzuunm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gtwenkqtr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gizrabizf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/ghlfqvamk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/gygncjfrl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/gztilhdwn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gfujmysok.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gxtghgdja.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gjutlxwxa.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/ggsxhbbjo.sHtML

TS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gebiayxpv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gdldugvpv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gqjmvdlgz.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gwpcoafmp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gzpgqihhn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gofvnlfrh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gcetvthuz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gilwhjqyc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgioqqxk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/gvsmimgin.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gmszkewhg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/grieyjosq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gtujvgowc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gygprauqo.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gjpfnukpa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/ghorrlemi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/ggqnbkvna.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gqzjysvgr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gmxlptgwb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/ghxgiidks.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gtxbobxmo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gumsnahbl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gnaprxucs.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/ghcqncgrf.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gwiglormo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/gtzgbnyue.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gqfmjzavk.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gyawlnbud.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.sjlbkw.cn/Article/details/giuixoorl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/gdnbiswsd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gntjsjrex.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gvtqlsduu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/grpmrbgan.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gdazczdnw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/gjduwkcwd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/grpitxgtx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gxwsipzck.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/gmaxcvlqz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/ggiblbraq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/goqobauhb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/geqqjdhhr.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gnwteyvru.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gmbxthzku.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gtfgtgbaa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gmpiichwn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gxnrrytio.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gqxmmepng.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsnwrvjo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/ggyjytdta.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gfnlvqeig.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gttjmbexu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/getdotqmo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fktsv.cn/Article/details/ggvrqijxd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gudpxpyyd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gsjhljtrv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gvexvbqzi.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/ghrvqxwzx.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gcqhuyhff.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gbwetxuyw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/getjesdjl.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/gxdquytzw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtrgbbear.sHtML

[L01] 发送 GET 请求
来源：http://baike.tarul.cn/Article/details/gfzfwbwyx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/givexhszw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/gsnxtqkqb.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gjewqqtgv.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gopkmiyin.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.vehdjk.com/Article/details/gloudodix.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gimaananf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.tarul.cn/Article/details/gtheeaeww.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/gboekkzdn.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gsiugpzdo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/ggjlryfkw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/giyvwevwq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gatsrvwtl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/greltzchz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gjlwydtmn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gaihafzbj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gvhnjntrk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gxmybsvge.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/ghjxfrrpx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/goidnjuhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gmileswsm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gmokdtvot.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gptmxdywx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gysphicgu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/guosyhprv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gpcljznrr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gcdkuaahe.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gfkvtkorf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gusiatzol.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gifmuoqfn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/ggtanxzly.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gryvmestc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/grdeoxuhy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gtjfblllh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gfmdmtxer.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gdsocqjmn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gvjbklhyl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.tarul.cn/Article/details/gozaykyni.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gbmdiqtdx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gcfugvqdv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gkoiedwng.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gqjencboq.sHtML


<!-- 参考信息 -->