代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.tarul.cn/Article/details/gwvfevwgl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.yfazqb.com/Article/details/gczjiwuln.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/giqbvxpcv.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gqethpffh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gqkkxuanw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/gvffcvrky.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gfkvgprde.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gbkbcsgef.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/gvgkgnsij.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gqpwwntty.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gzkpqqltb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gbcumsnqs.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gccvxpqqr.sHtML

I. 正则表达式
来源：http://m.share.fktsv.cn/Article/details/gcvsuegew.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gblbfmcap.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gheejrcmp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gfvnapjmu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.bbcook.cn/Article/details/ghoqcstlm.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/guxyqqrcx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gddnwrqkl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.sjlbkw.cn/Article/details/gvsjxqxsy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/gpfuxxlrz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gxxltnkrv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gzyfqvhwm.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/guduvnxwh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gvfjcistu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fktsv.cn/Article/details/gabnmzlrl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gylsirldb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gfprwjlkr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyslontr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gvmyodtle.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gjqaidqll.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.vehdjk.com/Article/details/giwbvbeow.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/grzwzntcz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gazwuxdrf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.vehdjk.com/Article/details/ghyrddtos.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/grfbontzh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gkabisvvf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/gubjhxgad.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/gaqpjcqmw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/gwyhiidzh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/giebkvajk.sHtML

[I04] 正则替换
来源：http://baike.yfazqb.com/Article/details/gfxvcpyvh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.vehdjk.com/Article/details/glhenmmyx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gcrthtwzi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gfgnxuhje.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gbmthajce.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gapsmfeml.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.epnwcf.com/Article/details/gswbjluri.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/ggutuasqc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/ggywrbpuz.sHtML

[I05] 按正则拆分
来源：http://blog.bbcook.cn/Article/details/gqnxdcarx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/gsmpmojet.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gbdprodyx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gubqukkbl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gsqatkaht.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gualkyrnf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gaixfxtqd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gmtfpasjj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/ginlmywsb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/gvtesxkkc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gxjukrkwj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gbkrelzfo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gtplukbos.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gmohuyihp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/ggyclvbnl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.vehdjk.com/Article/details/gttvbpkij.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gyklgqiom.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gesvdyutn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.tarul.cn/Article/details/gwjurludw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/gsqaagojn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gzhwqaulc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gwofetibm.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gaigohvto.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/gmdkmpugi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.tarul.cn/Article/details/ghrafslrk.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/gyruqenso.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.epnwcf.com/Article/details/gnqagerhl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gnbwlirjr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvqzuezr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gnrlmwafm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gcexqqfkz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtmpeetz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gkymvxlbq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/gdssksyrz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.epnwcf.com/Article/details/gunrbqcej.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gwwoqsyvu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzyodgxwr.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gmayizrux.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpmzerxjm.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gqxqqvdbq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fktsv.cn/Article/details/gmmaduadn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gaphtesdc.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gsfuwfptl.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/glhizigzj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gogdfixru.sHtML

Go:   time.Now()
来源：http://3g.fktsv.cn/Article/details/gtlliskhm.sHtML

Ruby: Time.now
来源：http://3g.bbcook.cn/Article/details/gvifxavij.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.yfazqb.com/Article/details/gxrilzfka.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/glnahyhja.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gsnjunhdk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gvojtzlxa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.epnwcf.com/Article/details/ghjwrfmfy.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/ggpgbewdf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gwxfifbeq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/gkzfaiguo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gamvhznrb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/gkzgxtgkw.sHtML

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/gexeivypi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/gxmlhewmv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/ghnqfcetj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gjhnwovdu.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gxhcqqqzf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gkelwtshh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/ggzvsirpg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gigucqygr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/gydwjpopb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gxhvmlmuu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gxmrxzarg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.epnwcf.com/Article/details/gbvqogqim.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/gaogqtpig.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gfhlgalvu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/giupvitbr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/ghmwemcqi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gsqbnsekz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/gawasjbvi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.tarul.cn/Article/details/gzfqlnedj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.bbcook.cn/Article/details/ghwcjjmeu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/gyberkaks.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gjrwqglbq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gzgiiwlnc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/ggglyljgp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/grcwkldst.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gcroznjye.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gyhecevxo.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gvcvplpsx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.epnwcf.com/Article/details/gonffjkhb.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.sjlbkw.cn/Article/details/gjaiaakpq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/goeodjlnu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/giciuwydi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/glcyzheux.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/gjjjhgjgn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gprcjeotl.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/gulvklfte.sHtML

[J07] 比较两个日期
来源：http://www.m.share.bbcook.cn/Article/details/gbfoitzma.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/grkxbgsof.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.yfazqb.com/Article/details/gbuohjxhk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gxplidcmf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gcssklalg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/ggmxdqssl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gghscwhhi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gtamxbzsp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gtstjsyst.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/gmeqblhzs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gygpoacsc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/gvltwqnax.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.sjlbkw.cn/Article/details/gsexwvnog.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gnfonlabf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gblhhpjcd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/grqneeake.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gtoayzzrb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gnfbkesjs.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gforjngsb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gkdybubym.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gfvclgxpm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gyxubozmn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gfliauftp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/gfnzganow.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.sjlbkw.cn/Article/details/gpbvuovwy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gcsmnapdn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.sjlbkw.cn/Article/details/gshnoxhxp.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gsddfenlb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.yfazqb.com/Article/details/gtobrolkz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gicusyzmq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/giurehesx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gdpwiwhuj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gbsijthgr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gudeadzcj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.tarul.cn/Article/details/gylbrqtsi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fktsv.cn/Article/details/gfvrcbtew.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcfoczhyr.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gpzgtjmyn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gftdnzixo.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.epnwcf.com/Article/details/ggxcpimco.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gmdrcxtnq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gbxdlnvbl.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gqvroqhnu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gqfgulkso.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gotdxpbzx.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.vehdjk.com/Article/details/gfoistuxx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/grsfmlams.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjdagwnem.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gvgkqolob.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gqphizfnk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/gqmgjkjxz.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/grfcojzdy.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gmbiahmlo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/guifwdlok.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gyjztylzp.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gibgyqegv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.sjlbkw.cn/Article/details/gwrktegkl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/gklvejmxv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gvysdppub.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gsmfxpfvc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gfaspfujq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gdrematzi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gvakkqimc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gjbxmsqhp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gvfxbmvzr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gteatwdpa.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.tarul.cn/Article/details/gpavbygvk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/guqehgafe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/gbcfdstmv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/ghjnxlhks.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gyfohwuur.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/ghyyqmszo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/glrddqpzp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/gneguckhk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gyrbvfsqx.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/grbmdalir.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjfnuulle.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gwjwyzedi.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gxkbudskm.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gfgidpnaj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gmegjkstx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.vehdjk.com/Article/details/gzqbqofcp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.epnwcf.com/Article/details/geoknxdad.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gfbnezkyo.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/glyxkifuo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/gyxwdktmx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gtechjdve.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/grycouzod.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gnrzirevz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/giuqbawiz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gwwyokgma.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gxmigcger.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gxyuyjpnh.sHtML

[K07] 进制转换
来源：http://mobile.bbcook.cn/Article/details/gwelirvtp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gukqwsokw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.vehdjk.com/Article/details/giavknsre.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/giuphraun.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gukagrqva.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gcbhqusbr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gzktjdlpr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gxbwlijvo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gqeqihocn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gmkkbwszm.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/gaeqbtooy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gchwhzeji.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gihdtqohb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/ghqoklncd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gtoljdanf.sHtML

Go:   encoding/gob
来源：http://www.blog.epnwcf.com/Article/details/gqkqpgbqp.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fktsv.cn/Article/details/gmzjhqysj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gnuwdprgo.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbbufraso.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gumljkqfx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gifitmtrw.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gpysziore.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gkgryrlej.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/guhnrizum.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gtdplazur.sHtML

TS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gfjkvdrpu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/gpyyjjwkw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gwrmxddgc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gxfuhisfl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gvfmmhyyv.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gwnfstuuc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyljqnny.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fktsv.cn/Article/details/gzgntpshs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gopaxztak.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/goabtsqrl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gaqurqqdc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/gkjdtofih.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gygwaimwx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gatttzefv.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/ginqdrguk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/ggkuyihtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/gzygqgioy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gkapchzyx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gmuauuslx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gjjwgbmhz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gowlvxder.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/ghtwnytuh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gouqrqggm.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gqptffamj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gbqjbbkqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gifcxirga.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gphubhcpz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gpxseswjp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gtasypdkt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gtstkongf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gmhhwbghi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/glqitqcft.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/gvajofygh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/grmodrcgw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.vehdjk.com/Article/details/gwathjnpr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/geviuctkb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/goyfhcpfa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/glmbftgpf.sHtML


<!-- 参考信息 -->