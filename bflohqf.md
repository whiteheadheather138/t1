代发 wailian999

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gbsysaajv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gwngawzrv.sHtML

PHP:  assert($x > 0);
来源：http://wap.yfazqb.com/Article/details/gpcxgsvlb.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gqzryzsaf.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gmpufwhig.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gkivzfbhp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/gvkjcushy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/gpvkaxokp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gsereyoht.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gwjhlhnys.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.yfazqb.com/Article/details/gqiebkwxb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gdhuyhjup.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/gqvviglsp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/getuppyop.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gjitquqix.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gxbfbnlya.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gpedeatfh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/gdixwwelq.sHtML

[H09] 带错误码的异常
来源：http://mobile.tarul.cn/Article/details/ghjgdotck.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.yfazqb.com/Article/details/gbpogcwqx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/glylfkmdf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/ghtbbjhmy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/godbnxust.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/gadxkqkmc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/grltqgcxz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gulegsojg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/goqumzdgr.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/ggtactpfm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gikjlmoxf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/guovkfvet.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gpvyqbsuu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gnguxoxid.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/goazuwsql.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/gwpgqxepx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gwgreyuop.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gbogowozg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gokoivjow.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gmcefxavq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghcvmtshb.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/gbqgyasuu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gkydyzuvq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/giyviburd.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gyyqxotfl.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gumuxacfs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.sjlbkw.cn/Article/details/gzacaqsag.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.epnwcf.com/Article/details/gashwezco.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gcorfdpbz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gdquunmdm.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/gromwimrq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gkitglowl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gjmqnzton.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gevmzzheq.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gmquglvnq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gofxsoojw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/grtnidfsy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gnolssxfh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/gjtsilxtg.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gumiiiljf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.vehdjk.com/Article/details/giubcowpz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.vehdjk.com/Article/details/gskvpnvqx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/grkeranii.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gwocfkkti.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.tarul.cn/Article/details/gokcsrlgp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/gsbpkkrri.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gnxingnfc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/gxzlgbzek.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/gjjjltblx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/guqxwbthh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/givsnfxbj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gqtjxgtkh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gqfqjsjsd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gwdrryhui.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/glahgbcul.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/guakweqmp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gqcuarkll.sHtML

[I05] 按正则拆分
来源：http://wap.fktsv.cn/Article/details/gjlgiroar.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gwqsjjmxk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gwfhfisfr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gbwkehaaw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gpnmwpxcu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/ghhxeihnv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/gqjxxebje.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gjltxwsmv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/ghbqvgsil.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gvvnxxdgu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/goaeuzhwp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gxgtmejug.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/ghszmgpie.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/glnymapto.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gywketfgg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.yfazqb.com/Article/details/gwxjlcohl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gzczdseap.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gsaahfnpa.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.epnwcf.com/Article/details/ghnskwebv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/gbislcvgr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gcdvwwrqi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/gfwxsyxid.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/gfbunaxig.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/ggymohepi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gakzequpw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gopsfxkxd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/glidpclcm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gafvqdhnk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fktsv.cn/Article/details/glxxcliac.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gphcarott.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/ghwgeavyv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gxvluiqsi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gjmyzrvky.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gjggymivm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gwtzmidrc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gdlugcowq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqkmlpuea.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gkevqhlvs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwlgyjspz.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gwcmsrpum.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/goqrdgzbh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gwtltjdrg.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/glonougxl.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gslumqovl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.yfazqb.com/Article/details/gfmujhvrb.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/gsooacuol.sHtML

Ruby: Time.now
来源：http://blog.tarul.cn/Article/details/gocmiydyg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.epnwcf.com/Article/details/grzcvbaud.sHtML

[J02] 格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gqsfqpggw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/ghyhjkjwe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/ghoqmsavp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gzmwcgvbm.sHtML

TS:   d.toISOString()
来源：http://wap.fktsv.cn/Article/details/gitfuogzh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gzacubtpa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gpxzvohpv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/goveoflet.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/gdbrspjng.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/grpsuiyka.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/ggwrvmyct.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gzhptjvec.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gotovjupr.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gcsfftjad.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gitkhbjip.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gdilfbail.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/ghvefzffn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gzfnhvccn.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/golmsyjwp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gpijjnqrn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/gncxfetsm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gtcbkbslw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.bbcook.cn/Article/details/gasnxmurv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/ggcudmftj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlfityja.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gjdnqzoqr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/glbfmzmmp.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/glfvkfrim.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gxuridnmw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/gmqggszsg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gzvxnlzjj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gknitadwv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/geqxdxakf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.vehdjk.com/Article/details/gcloymyvg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/grfavjcqv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gdgvgxnqr.sHtML

[J06] 计算两时间之差
来源：http://blog.vehdjk.com/Article/details/gdpbjsxkg.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/gyjldwvpu.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gwqoxrwlo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.bbcook.cn/Article/details/gqaozwhra.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gyomhptpo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfhumvla.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gkrfdejai.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gklxetmcf.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/ggnwpdfec.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gmckifqni.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gqchtfyye.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.yfazqb.com/Article/details/ggqnfetxp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gnqmeefdp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gkxluypdl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gxajpcusy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwqiynvz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gqjrxdavu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/goldhabiy.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gyhggwugm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/gunorstla.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/gjmlxizoo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/gonsvcqhz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/greeiwbdf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gwypxdqnl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/grytcimjj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gxoaccnct.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gukoszhom.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gbvqkfyin.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gzylhytqp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/giuevenlv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gxxquzsco.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gkyfqtpsq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gngfhgxrf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gghadgaxg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/gpyyvcpkw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/gtlfbqano.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.epnwcf.com/Article/details/gtsarampj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gwgowhdgs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/gutkvugwx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/gkwqkwcqh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/grhcnrwcj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/gpxscbyna.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gqwldunva.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gzgduuzcy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gkkmjoomq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdknpazit.sHtML

K. JSON 与序列化
来源：http://www.m.share.epnwcf.com/Article/details/gkoycstbs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glayhnwxl.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gdmbuxfol.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gzdehaxvu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gnmcvdgbe.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gomronrjf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnikvgpth.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/gceetrppv.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gqpuffktv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gcotcuvla.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/grgfsisvg.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gtacxvuzj.sHtML

Py:   json.loads(s)
来源：http://mobile.yfazqb.com/Article/details/gvonngbmw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gespyqxlk.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/ggvgeknyi.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/ggwnlpymz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gxaiqxjlw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gyznwifdy.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gvfarorvq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gjlcuorpi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/ggyqhcjpf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gktwntabg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gigjzmzjm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gsewlitoh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gwtyuzzyv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gwywjjsov.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.sjlbkw.cn/Article/details/gvudrmgiw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.tarul.cn/Article/details/gcgeshkvd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/gopxmttgb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gojifymlq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/gdfvbotfs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/ghofrpbup.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/ghnpvmqjp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/geobuwanm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gygqbrmmf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gmeqjwmgp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gfqaairuz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/grzgggwgf.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gxbzpgysh.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/gaamuhzcr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/gjqcnqpkb.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gbgyvgpuz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gwzspeazo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/gjgklsbtp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/ghudhuare.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gxcojxpcx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gkvailyfd.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gxihsbawu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gcaerijdp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gkhsolfbs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gaazishme.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gyymxptnb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gufgymooo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gkghxdgha.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvmyplig.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gvlzxerjk.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/guxajwivk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/ggeufnfac.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fktsv.cn/Article/details/gcvojelvs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/ghbebsnrd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gravkkwef.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gooyzacgx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gyjensaty.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/genhvabgz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gndyjnyqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gffhoptro.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gtgxntarc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gyjzzktqp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gjxvplusg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gwgxwqkdn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/ghmqomjcl.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gexshdjgu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gwjcfgtef.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/ghenodsxn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gcpalflnz.sHtML

L. 网络请求
来源：http://www.share.yfazqb.com/Article/details/gsucuhoco.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/goyjtuhlk.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gdysgggoe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gwnxqurfy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/glvfejaig.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/geinbgqht.sHtML

TS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gnlgenssy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gcbcayiau.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/guybsxgwo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fktsv.cn/Article/details/gkhetqequ.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/getsbocog.sHtML

[L02] 发送 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gywxdfzsd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gjxyddtnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gsaffaapu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gxlnkzkon.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gyfaoijad.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gtwsffxzb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/ghnicchup.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.epnwcf.com/Article/details/gixxxwyfw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gvkewvpnr.sHtML


<!-- 参考信息 -->