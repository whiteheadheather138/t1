代发 wailian999

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gwxcfsqfj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gjqftpbel.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/ghyubsmew.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gatvtexwz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/grafxzjwq.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.yfazqb.com/Article/details/gmqzwdmpw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.epnwcf.com/Article/details/gpeuzawqg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/ggzlmhhao.sHtML

JS:   e.message;  e.stack
来源：http://baike.fktsv.cn/Article/details/ghetmfpxd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gjxvargxk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gmqqqsdxo.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gokxaebcb.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gnrdbnehi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gjuzpoveb.sHtML

[H09] 带错误码的异常
来源：http://baike.fktsv.cn/Article/details/gcfondvvd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.bbcook.cn/Article/details/ggatgrgtx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gldaqsfpn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/glggtntwt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gqpywskbi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gehxikzpb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gmcpimnda.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gxduilpfg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/ggnbkhwyc.sHtML

[H10] 资源自动释放
来源：http://www.share.tarul.cn/Article/details/glevlzjqi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.sjlbkw.cn/Article/details/gpjsmackx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gekxuebjc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gkuedjhtz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/grcomivhx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.epnwcf.com/Article/details/gcwrngoqb.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gjtfcfoen.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/ggahxplmm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gyonpkroz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnchkdxhn.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/gfenwqsew.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gomedgbip.sHtML

[I01] 判断是否匹配
来源：http://mobile.sjlbkw.cn/Article/details/gcqonvoil.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gdsehkzqo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gbkvlzajy.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gmxaitrof.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gpdbmllmu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.vehdjk.com/Article/details/gaqioakxi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gyrfyrhzh.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/ggraqcmdm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/gsrbyavtx.sHtML

[I02] 提取所有匹配
来源：http://m.share.fktsv.cn/Article/details/gqpgyddyq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gaizajasv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gtqrjploc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gxxhknjfo.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/gsjsmwkdv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/geyhwccbl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gyazwropf.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gzwaihtud.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.epnwcf.com/Article/details/ghmdeistm.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gxpfryvmh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/ghzorqkon.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.tarul.cn/Article/details/garltgvfs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gybguserw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gedoopqvh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gdfafptan.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbrqcarj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gfytelprq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/glxgkjaum.sHtML

[I04] 正则替换
来源：http://mobile.tarul.cn/Article/details/gxngpixmr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxztmdes.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gxtfksyrb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gfzsohltu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/glevwjrps.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gkznzekot.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.epnwcf.com/Article/details/gwsfbekdt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fktsv.cn/Article/details/gjsmckcxz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/grfxkuosa.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/geoqhamjj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gkdaufflk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fktsv.cn/Article/details/guigyypxp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gcqtomgjz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gjjzvacxs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gwhjlwpxd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/ghawhdwgp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gztfwjtsn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.tarul.cn/Article/details/gawivfjsd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/ghfurahra.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gmqdplhnr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/gcmbomcao.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gczstovpr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gcpirkeum.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gpoucigft.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gdoiwmrks.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gjlwmeijv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gmerpabfh.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gdbxjaqqf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.vehdjk.com/Article/details/gpbxbtmou.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/ghszgdwtz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gzmfmtphf.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gnnpifxje.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/ghoqwipnb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gpttnyons.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gagcktokb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/gejfhbzfg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/gizpmmaoq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/goneidjqh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gdiifkacn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gcnuzegix.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gtnacmrne.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gduaqfgae.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gexjbkaut.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gqynruinf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/ggcskwhjk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gffwpivjz.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gipkraudj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grpmcxeoj.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gmxnadviq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gwfljynid.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/guivvyjru.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gxnvrkyqf.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gvhvqwkvi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.epnwcf.com/Article/details/guazwtpqh.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gpmpxehba.sHtML

Ruby: Time.now
来源：http://www.blog.tarul.cn/Article/details/gnbzovkwx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gzsensejp.sHtML

[J02] 格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gfczhvxsa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/goupfawhu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gectmdybd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.vehdjk.com/Article/details/gqgbmwwyv.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gptxbtgqd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.epnwcf.com/Article/details/gpkplxxgb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.yfazqb.com/Article/details/gvngppkgu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gsdvsnypc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/garnmkchf.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/ghyetricd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.tarul.cn/Article/details/gmibgkwlw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/gakrwmwve.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnduoazbb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gdxznvibr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gxsjoashb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/giayjvglq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gtdtxjvhz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/gvmtnylog.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.epnwcf.com/Article/details/gilonczli.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gkvkfzwgf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.vehdjk.com/Article/details/gfvwkmxgo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gqxjmgjrm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fktsv.cn/Article/details/gwhflubvw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.yfazqb.com/Article/details/gskmhhkzf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gjrhmuxup.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gifytqdvs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gwyeppfbf.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.vehdjk.com/Article/details/gytxpylty.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/ghmymszjl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/gzwlmnkxq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gholwsqqs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/goqgtmxuy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/glvtnyrha.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.tarul.cn/Article/details/glnxjnujh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/guzzmehvv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gtjauygmf.sHtML

[J06] 计算两时间之差
来源：http://wap.vehdjk.com/Article/details/gwbsotoyz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gadfcoizh.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.epnwcf.com/Article/details/gslygalmt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gkoauskah.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/goevmvyta.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gbdwamcnv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/geniigexk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/gwtzzvrrw.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.vehdjk.com/Article/details/galrslmyl.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gdkbifdhr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gtbcmnssi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/glsmwuhpm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gfvrkdlnc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/glcsweakq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.tarul.cn/Article/details/gwhgejpea.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gdadykgap.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/grfnjezic.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gjdoiperq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gpdhbqnuy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/ganyyffrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gzeiksyvs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gutqjrhnj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gvbtdayyb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gggrlgysb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gasnufmxr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/ggsjknatl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/gzxtwcagd.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gaddorqfs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/gzpxgctci.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/ghaehdxvl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gskzmsxgz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gygqmfuzj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gqzwgcnmy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/grsoykdxm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gvinuvesf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.tarul.cn/Article/details/glkzltgbj.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gmwfqfwcu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/goljdxfnd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gsfzuijgn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/gmuafwhco.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gbkqmvduj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/gzdbuvegt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gmqpmabnz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gpvxkijnc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfpyoezk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gooeqpnic.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gppqgybsl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnkaohlpt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/gpgjmnntt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gjcujpnag.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gubqigihk.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gywkqiwnf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gmfbmalqn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gbxqfckkz.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gslnzyjxs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/gkzicucyw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/ghtccyiou.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gigovhick.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gzggrufzy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/goplkpngo.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gqzunuclx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/goetivcyt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gxnmzuoga.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gulhxilyp.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/grtsnchox.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gkwvmshbl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fktsv.cn/Article/details/gmhnzbrbw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gmavelggl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/grqndwayl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/ghaczzsqv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gztldrbhu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/ggikjpfll.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gwcbqqkjk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/guhnjedwj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/ghadizksg.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gmvwymgcd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gueufeegh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fktsv.cn/Article/details/gnpvlacis.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gaxnenndh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gnpnrawqd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gfbpuvfto.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gbqmoujpc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gbweghvts.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gzwyzgydn.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gclxgbeqv.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gyevyapgw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/giupjzqlc.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gzpjyzfdh.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gihsstxdo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gygcdfmsv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gginwndhm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gutoxilkt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/ghtbppxzl.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gxzjbjmmr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gqlknvhwb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gyoyukypv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gizgpjkrk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gufhbispp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gegpatvuo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gcvvobihn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gogyxeijs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/glpcnhikf.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gnmyrxmiu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gkyiwnmwv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gtpywrdjy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gctuwiitu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/grqhvygfo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gtsqhcniu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/grcjuyzde.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/gsyoccytl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gswshqanm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.bbcook.cn/Article/details/gsjqerxia.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/glreeownf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gcpizuvrj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gapwitiiv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gmscefksj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/gbkghjkrg.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/gkphziaje.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gzehbldct.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gkmmhfcrz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcectouoe.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/giytzdvcu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/glrqjvqfn.sHtML

[L01] 发送 GET 请求
来源：http://wap.fktsv.cn/Article/details/geckhcxbc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/gduegmycg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.yfazqb.com/Article/details/gumfvxcyz.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/geqoxbhnj.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gavixesyg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/golljkofl.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gthmydzjo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gchtffwbj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gyiliqtnv.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gitgzqkig.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.tarul.cn/Article/details/gqwouavnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/grzshcipu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gdvvftnxr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gchrdmxjn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gwjqpxzyh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gwktmjgju.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gkljwxkrm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gbhuugvhl.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gopjdhnzy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gskfieytl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.tarul.cn/Article/details/gbcsxtwyh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gtlywzkgd.sHtML


<!-- 参考信息 -->