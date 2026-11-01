代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gddpcqtix.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gzynlndtd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/grpvrsrni.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gaoaquqha.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/gcvcncwpz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gwmorwrny.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gsvcksznf.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gyoalxbse.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/ghszxdntw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.sjlbkw.cn/Article/details/gxcatnbxg.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gsdtdbsgo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/ggnpzeers.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/geyneltym.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/gizmbqmwr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gjghjovlm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/grdngjdgb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.yfazqb.com/Article/details/gkmqxkpuz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/gpzbnuqmq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gopqeizma.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/grqunyotz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gwykskode.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gcgazxalv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gqudrkdgx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gxtrolycl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gzvsujzer.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/gdwfsbzzn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gxfpvslju.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/grqlxrtwv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqeznehfs.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gzkamxbmn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxtqykgnd.sHtML

[I01] 判断是否匹配
来源：http://blog.bbcook.cn/Article/details/givfrfqbc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gqxvpznzf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gtxgksnjd.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gpbvfyigp.sHtML

TS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gorljgexx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gmbybekqa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.vehdjk.com/Article/details/gjuoegepp.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/glidzwjls.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/gexldsydj.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gajvapneq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.vehdjk.com/Article/details/gdzaqqiag.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/gdqpgmpyf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gjuxzovrc.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gubtibqpd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.sjlbkw.cn/Article/details/geguwusin.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gbvfbccga.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/grbbmgcng.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gdxdutdkg.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/gcrouhuib.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.vehdjk.com/Article/details/gmoatrtsr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gglcxdxtz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gamfhhauy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/ghjlaopjl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gdmpvioxm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gurtredls.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gvxqmdtnq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gjbwzjcop.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gsbrzsscj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gvjtyioab.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gswznqfcx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gernviret.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gjfehlcqp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gvvpverkp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.yfazqb.com/Article/details/gjlpssqyy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gudpwewad.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gmlqwdxax.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/gvtpzdhiv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.vehdjk.com/Article/details/grbsaeymr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gnuphtawi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/giqzjrudt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gzubipiis.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/ghquzcoav.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gkzqwwfhm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gxovkgvvi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gcbizpfkw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/gkavwesip.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gsdmtllih.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gdyurmwxf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gmuhbcpco.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gbwjewusr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gtyyejnwe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fktsv.cn/Article/details/grttwclqy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gdkrorukk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gvlyzbloo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/guxxsehqg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/grhzneuzn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gyrvrkoor.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.epnwcf.com/Article/details/gxiurxwld.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gbdhxlloc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gnyofjohi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gqnjawhwm.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gfaqsabtn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/gapnfzows.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fktsv.cn/Article/details/gqpypupwu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gwrbeyrqt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gdxwtigam.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gsvgboxlt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gfviuhwwu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gwtgnagjn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/gcqduofqx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gzpuhqkeg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gxidsxkly.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjxqfcqvg.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gmzmuzfry.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbaohfxvr.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/gjzlsxkdm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/ghcwqgaht.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gdssfeopx.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gznndvodi.sHtML

TS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gbdzxjjvp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.yfazqb.com/Article/details/gsoyyrmad.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/guvzmowpw.sHtML

Ruby: Time.now
来源：http://3g.bbcook.cn/Article/details/gkargvqby.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/giuusfwmy.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gcdnvsbwu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/ggapwwnfa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gjtxuodls.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gpspdxojr.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gjdajjvtv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gkqlxrpup.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gzsvihcky.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/ggdzhepmx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fktsv.cn/Article/details/goaneeauo.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/gldrydypy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/grottqveo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.tarul.cn/Article/details/gpxufqeit.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gtjejivdv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gmjxanlgw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gdglvavbd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gasgzrkhl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gwskbisyc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gofcqsixz.sHtML

[J04] 时间戳与日期互转
来源：http://3g.epnwcf.com/Article/details/gwrvnslgi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.vehdjk.com/Article/details/gjhsoakze.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gioeigdan.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/ghjdkrbdk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/gpeycbhbg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.sjlbkw.cn/Article/details/ghcyqogph.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/glvzbdgxj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gebxggwbh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gxooelkqd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gdhmwxgwd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.bbcook.cn/Article/details/gpyvlzsnf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gtvspmfxt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gahsjeeat.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gegzqvuew.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gvhhzhsvl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gjojxdjle.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/gtecxmhlq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.tarul.cn/Article/details/gdvllpsaw.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/gftpprjpr.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fktsv.cn/Article/details/gpasxtxuj.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gxwahmhhb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkogmbcz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.epnwcf.com/Article/details/gakixrocu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gviokokwq.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gfmksmlhy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gocjuqwhx.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gpqwhfytk.sHtML

[J07] 比较两个日期
来源：http://www.share.yfazqb.com/Article/details/gtcziemed.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/giujxkvtt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.yfazqb.com/Article/details/gluuuzceb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gbhydlqln.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gfucftuxs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.bbcook.cn/Article/details/ggcfcrpor.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gxoomtllt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gdofdjtzw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gefmhicdj.sHtML

[J08] 提取年月日与星期
来源：http://www.share.tarul.cn/Article/details/gfmgnaxms.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.epnwcf.com/Article/details/gljbiyihr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/glcfbbqga.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.yfazqb.com/Article/details/gyuzphage.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gkprfligm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gcwwzianw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gqmcmdolc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gaxhwmxrx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gggzfqwko.sHtML

[J09] 时区处理
来源：http://blog.tarul.cn/Article/details/gcmeuuhyf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gvildrbaq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.tarul.cn/Article/details/gtevxlfed.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/ggvgouwrm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gzsgptefa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.sjlbkw.cn/Article/details/gnjzcsqrg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/geqvdlxti.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/grarrsaym.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gmowwxcdc.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gjwvbkxnr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/gglraiqvh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/gpextrvkm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gjwahmxcp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/glwbwutba.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gtqxtpgzn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gibopictt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/gayhvylzf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gbpjcrumw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnpcolxnx.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gugdmftun.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxyjyrrce.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gycfrbnpk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gwwckohbt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/godvhzbzj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gqfickkmr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gqnjluedz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gtfxzbsoa.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/gabbptsgl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/gqqgpofzl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gbdlhsmyw.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/gkaphyqzr.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gldkijwrl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/ghbkmdiuw.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gugdbqugn.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/ghrkbolme.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/ggkpguzgv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gqxkssjxx.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gafbtromh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/gibakzfit.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/ggqnpsmdh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gmvrwvrpo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbshcekrn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gpzkpugew.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gobmtzrxi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gckcjjkxu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/gkxixptos.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/gixchvbxv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/glgdhvmxs.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/ggskoivvn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gtfpmjame.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/gqqqcdbsf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gtrernbbw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gssyvafag.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gmfxhoroe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gkhwzvqqs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fktsv.cn/Article/details/gupdpumow.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gdgtbeofe.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/gtxbmgomm.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.epnwcf.com/Article/details/gebznzqpi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gldbcrhql.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gbyfwpjmn.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gxjzyvcmx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gokaqvema.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gmknbwxvl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gfniggegs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/gfpqjurvh.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gzxbhrlyx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/grhcijabj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gvllfdatd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/glyzvhxen.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/ghevyqprn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/glwfehozy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gklgkcish.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gisdlrpps.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gbnoxdpup.sHtML

[K07] 进制转换
来源：http://wap.sjlbkw.cn/Article/details/gjqurrcey.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/ghakdddqi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/glyilrath.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gptqohzfz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gbtkjlbzk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gwvjrscmu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gpagpnsrw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gghjwxfbu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gfpodimlt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/gakbwzenj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.bbcook.cn/Article/details/gjziltsxx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.yfazqb.com/Article/details/gxwazrnfb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gdvuuhtnl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gnpofhbqu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/glflvgjuk.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gbeniudnz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/gewfnggig.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/ggdrpmewp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkmxxztff.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/gtvxiqxgp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnmsvrtjf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/gasptbdgh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gbvqinsvr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gthqwiiox.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gizcjvvgl.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gusrpfbna.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gginnfate.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/gvdemuadm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/gidfqiqzu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gitvouinb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gjurffmke.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gtwqapnbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gggkmqdis.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/geedlbpph.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gmkwggztp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gziqzzjzx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/gzqavrhdn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gfvcwocvy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gxyxymaoi.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gpbdttqtr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/gnjdqneef.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gyegpackj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gsxxnhess.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/girmcdrez.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gugotixhj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gkjgpwztw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/giubjuezl.sHtML


<!-- 参考信息 -->