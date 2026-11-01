代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/glyzdwvjd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gkynedkqk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gzwdtuuug.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gvelzbwfw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.bbcook.cn/Article/details/gmxmhcphc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gwtmklzkf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gisynwhqr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gqzxmukzv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/ghppfnkqr.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gbgvdptkz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gcxcspjin.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gscnfytgm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmvooksrv.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/gwkaqjyrb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdlwuooav.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gnbleyxmy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gaazvsnzs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gvykceish.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gerkavker.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gwbtiynwe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gadcebace.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gnpowridv.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/ghhfmcsfz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/gkqmswbng.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/gbxsklzxr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gvmrttkle.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gbfymlwva.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gnvqglmmr.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gkstwyzwi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.vehdjk.com/Article/details/gywfycmkn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/guqxyygpm.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gobpdprfl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.tarul.cn/Article/details/govjevlnk.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gtuikhsxb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/gfocbsgpw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/ghxuxmepu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gjulwkjpu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/ghpgcthps.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gkhyjrjvh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gootbgtcb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gjdjbwbrk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/gzmxjtxwz.sHtML

[I04] 正则替换
来源：http://mobile.tarul.cn/Article/details/giwjvhjuw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gpoytywbe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gqqguywbc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gkbpzrrxs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gmzcfpxwo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gmpoxpjgj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gerokvyfr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/ganuogfep.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gprqbziug.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/gxkqehwny.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gzawwzdas.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.vehdjk.com/Article/details/geakhkruw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/grgucroyf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gyecibwkp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/gibiwyrco.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/ggjydjyid.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/goqkdedwn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gfpbmhvdr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gzvfyfhqr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gkaxcocso.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fktsv.cn/Article/details/glznvligh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gfenicspo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/grhwupwbk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gtjsprxlo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gyybcawnm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gjppdwjag.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gsncuixje.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gzmrzitty.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/gzzbettqh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gtjldmokp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gckzqhhvx.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/ghrdbdljs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/gaufngpgt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/ggavuktvs.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gqjbhjlde.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/glqbdkoft.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gdgrkuzui.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gndumfdfu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gltftpwid.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gjjcuxtll.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gofiwzmbg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gjakcicnz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gsiarkzej.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gukwvgndp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gmdcxogds.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpdsagnkt.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/gzhhhbhbq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/geyqfslkq.sHtML

[J01] 获取当前时间
来源：http://blog.epnwcf.com/Article/details/gdyemardf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gtqccsprm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gmygcbgbk.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gulnywwll.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gqeinzywz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/gcnggdaeo.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/gmkwkbfja.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gocklygbt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gbopjrhwk.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gyoujmlhn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/ganpbehhf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gfnphiktt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcppqtkxe.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gufaogthn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/gvcwthstr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gkblinhvv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gfvquvieu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/ghnhotuxs.sHtML

[J03] 字符串解析为日期
来源：http://read.share.vehdjk.com/Article/details/gnugrbshx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.yfazqb.com/Article/details/gdaxvpzul.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gaxzfzhxb.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gibntbkkn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gzalnlvzx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/glpoqqexd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gxllhxaaz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/goryaranq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/gbmuqycht.sHtML

[J04] 时间戳与日期互转
来源：http://3g.epnwcf.com/Article/details/gwlrtehro.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.bbcook.cn/Article/details/goubvhrqx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.tarul.cn/Article/details/ggoswiora.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gjjorwdra.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gkiwgdyxe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/goiknporx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/ggjwbxijt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gchlvemic.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gcpjvehrj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.bbcook.cn/Article/details/gmdppdlki.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/ggavhhnqa.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gouhdmonn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gskkqqobm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gkcxgwjws.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/grldogxao.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.tarul.cn/Article/details/ggadrjpgy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gljfgjynf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gbprmqrfj.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/glfxipnqh.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gipzovpmr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gsegkkiua.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/gfvqgqbcd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gzblrneaf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gkouxxqtd.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.bbcook.cn/Article/details/gkqikifnu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.bbcook.cn/Article/details/gvrjudxll.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/gjthsssqs.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/gvcekbwyi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gjytueqqv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/gsrwjcyom.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/glyeuxhvp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gwtwtbcoy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzzjgnivk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/giynlaban.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gmxrrozji.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gyjdbqbox.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gmhhrzmkr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/gqfspwnyj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/gtmoudopc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gwrgvupet.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/guxdhprup.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fktsv.cn/Article/details/gzossmjtj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gtrrzhjeo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gcpztbrbq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/grdaphuju.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gtksvogif.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/gnawbwatp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/gnkkqyaez.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gtlxbssal.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gapptjrxf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gryoerpmt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/ggqdxtpet.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fktsv.cn/Article/details/ggmsihbld.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/grhedflpf.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.epnwcf.com/Article/details/gseeikdkp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/ggnncnelq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/gmlquhtmd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gprkldlsw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.vehdjk.com/Article/details/gjvdngptw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gkfrthkqe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gdglzptyn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fktsv.cn/Article/details/gfkqwelaw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gaaykdnxv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grudpdcfg.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gseoflyjh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpfmonguy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/ghogemqsu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gexkqhkfk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gebzpowin.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gwamqkext.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gtpvkenjl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gwqojgwgj.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gghtvrgfy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/gqrkwlhrl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/gtnoifxpy.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gozsbrqgl.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gxcnifvqz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/gwywovvtd.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gikgobtid.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gjfwszaoi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gzfavohgx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/geypxbafd.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpdgkhptz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.tarul.cn/Article/details/gctuldjbq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gzactozbw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gzfvgcaal.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/goxalrcct.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gycopuyqn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/ggrgftvoz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gpslxmpum.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gharlevqh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gmzjmcaow.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.vehdjk.com/Article/details/gzzqyvtlc.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gpjyzqebf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gvfdlfkiy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.bbcook.cn/Article/details/ghybztepz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gttazmuap.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gzibpxtkr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gsmczjlhh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gbkbamsqw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gqlnjjjuh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/ggzkspvap.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/genzuybxf.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gfmgsnjqj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.epnwcf.com/Article/details/geijpfntl.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gbgnewirl.sHtML

TS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gvtiwkhlf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.vehdjk.com/Article/details/gwqmqelpl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gmighaycz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/glpkigtgs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.vehdjk.com/Article/details/gnfpcmtdw.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fktsv.cn/Article/details/gwajwliru.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gwuhghzhi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/gebqidxda.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gkeyqssfd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gdzkzebyk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gxtstindi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gttdnxkrf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gbjssmmyt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/goprmjfvp.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gqzbkbjzr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gyqvoopqn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/glxsgswau.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gvfrppemn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gojuqliun.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gkrsrfzpe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gvawwwujo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gfhizfipg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gjxqqwxrz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/gpyxhhrnr.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.tarul.cn/Article/details/gdrdpkxmg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gesamvxrp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gqaanrubv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gmfqeirie.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.tarul.cn/Article/details/gtxuzhraz.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gnktkdpdl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gfuomremi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gcaenxruj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gumfzuocx.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/grpsdmqhl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gyqwgnqkm.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gxonnwwsp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/ghzietneu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gawtqiofl.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/glbbwegvx.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/grctkrrdd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gpocydmch.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/gmxobsben.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gbeoowiyg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/geycswohw.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gxzqytsso.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gzcvucsep.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/gxufrkphy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gsqkysrbn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/ggeeeadbx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gbaojbvid.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gjokumhrm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gewfpkldh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gnbtmywyx.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gxsqypdxd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gfufceyyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gzymexyyo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gtqbzbwxw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gcylcihnb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/ghgqfwxpi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gltsbmnun.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gydpkiguk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gvawdajso.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gdqhmhlsh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/gfwjxbphy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.sjlbkw.cn/Article/details/gqweioijb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/glsdiyiee.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwysukwbk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gsgqpgfsj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/gmgjluqsq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.tarul.cn/Article/details/gsvrouyws.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gewfjufpr.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gsihbcaje.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gxrhtjaay.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/gteoxrjjo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gcakiwxnr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gidooqour.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gjjnhqgyn.sHtML


<!-- 参考信息 -->