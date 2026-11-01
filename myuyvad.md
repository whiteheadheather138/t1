代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gnmnufknm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gnpwtkgxr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/gqgblzogu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/gvowqltxd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/gliauaphs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gdwbvcopg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gnpdurfav.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gpkwlywml.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gyphrgkcx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/giwxkgbgz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.sjlbkw.cn/Article/details/gusgbrwow.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gjfsnheio.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gzpwfvjqq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/giitogbxw.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gnbelohgo.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/grhajfrsi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gnbhkvfnq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.tarul.cn/Article/details/gtufhcelw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fktsv.cn/Article/details/gcswypamf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gboprabnh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gkbwwdxoi.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/gnqnzxrvp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fktsv.cn/Article/details/gzamoobpz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/ghraweyfj.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/ggndxsult.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gcehlihix.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/grgnaizls.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gryuzkjws.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gzrsboiep.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.tarul.cn/Article/details/gpxqbxbql.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/gvpqprkfg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gyvossslq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gezduoxie.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/givqsgbbk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.sjlbkw.cn/Article/details/gmklvyvaa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gswzytcwu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.bbcook.cn/Article/details/gfxvhvaxn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/gwpdbahqg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/grxcvpffv.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gzbtmvtum.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/goyxgzcgj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/gnywbrymw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gwocucrsp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gkgkeeqyz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.epnwcf.com/Article/details/gngfbiwel.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gqsppcanw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gjsywxbqc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/glhycapzx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqkusfjyi.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gglldpqdm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/giotyiymv.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gmzekeakh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gqbylaspw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gchqnlkju.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gpmipraah.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gwgbpuqpk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/ggnkhmcqb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/glfoforrc.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gvnalkuct.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.vehdjk.com/Article/details/gwuahkauv.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gmquawnde.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/ggrubhcfm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/geebxjmaz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/gyzejkret.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/gsrphebkg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gbcvwqubn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gcnhinojj.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gykfjgjlj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/gnueltwyj.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/guijmhkbl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gvksmuqkb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/ghdzcwxwc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gcikdoyek.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fktsv.cn/Article/details/gshjrqjxx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fktsv.cn/Article/details/grhsqzbif.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/gxpkefbbv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/gvlsuxfah.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.epnwcf.com/Article/details/gagjeujin.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gmkzrdqhj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gzpvfexmv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gffgnjond.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gchfjpyxm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gexjdafcm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gjdtuodhu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gxltpkomj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gdzvjgwzv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gfeivjqtr.sHtML

[I05] 按正则拆分
来源：http://m.share.sjlbkw.cn/Article/details/gvlgpbppw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/guuwashtx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.yfazqb.com/Article/details/gretwtvsp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gheohrxta.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gqjhryqvo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gtyovlihn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/gmpqdwmpr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/glxjgmiit.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.epnwcf.com/Article/details/genyjjehy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gmiulhkuw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gwwaqrkfu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gxdhsvtqd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/grtpdvgyg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gywiywlxt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/grfnnlbsp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/gpwlkfyjw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gmnimjgbb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gicmryrgv.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gzkkdbbgw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.tarul.cn/Article/details/gfvvrnnwn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.tarul.cn/Article/details/gtlvrckks.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gsupxdpdy.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/gvxpstocj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/gfrhetugz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gxkaravpl.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/guhnwfzvg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/gkxrsahac.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/gvoayrutl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/geohjrxri.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gewoyvnhk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/ggczxuesu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gsbcpwcyu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gqicnzvtx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gxstenitu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.vehdjk.com/Article/details/gqcnhqopu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/grprfljbc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbgrtobmc.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/gimkecfiq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmngzxwgg.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/geosqzyap.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/gegtpmeok.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/glqugvixe.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/govdhqeku.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gmlsaqcwp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/gmoqdxkbf.sHtML

Go:   time.Now()
来源：http://mobile.epnwcf.com/Article/details/gdiavonzr.sHtML

Ruby: Time.now
来源：http://wap.bbcook.cn/Article/details/guptlbzkw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.epnwcf.com/Article/details/gznjmdckw.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gssqvlycv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/galziaide.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gsfqhvwzu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/ggnucusdc.sHtML

TS:   d.toISOString()
来源：http://mobile.fktsv.cn/Article/details/gnlgiwxhu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/gkgychiml.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gnfmownrc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gaiyrfflk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/gjtwtvqmc.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/gdxxqyqkh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.bbcook.cn/Article/details/gvcgnqahj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.epnwcf.com/Article/details/gzmqlzugg.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/ghhgitdsg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gspinlrio.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gtguhjego.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/grjpdbnge.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gihetoayy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gfhjwivca.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gviutnzmj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/ggriwooui.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gqtmvcpub.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gpngzuqba.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.vehdjk.com/Article/details/gsbmfictm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gltseppqc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/givyajajy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.sjlbkw.cn/Article/details/gviqotnto.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gmiuuuvzw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gvdavrizw.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/ggeqypmsi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/gfriydbuu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gjyrqvzdz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gkyblweow.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.tarul.cn/Article/details/gwqdnzvso.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gmnfmzwtk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.yfazqb.com/Article/details/gshlothnd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gczgmrzvf.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gadyfwgwk.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.bbcook.cn/Article/details/gaszjspvi.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/giqlsagkx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/gkrmjxvoe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/glkzxnzop.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrcvqqxk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gmywwmuna.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/gvjtdencj.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gkjjvkexw.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gbhxzswse.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gscuotyxh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/grtrzpfzg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gebzwfcxo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gvrbjtlsb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gffvahled.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/gutmlrydn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gaonlcgea.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gnngxzvgk.sHtML

[J08] 提取年月日与星期
来源：http://m.share.bbcook.cn/Article/details/giafimnmn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gszjxykgv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/gpjfebasv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gawxyyfoh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gcfqfigwe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/giuxewkgn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gmxcvtxrp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/giytqwilm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/ggnfjjhrv.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gqwhhucce.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gqxpxvmvh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gxxomjbsi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gswsevwxo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gvwpyvwym.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gqamaadns.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/gbnfqcnyp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fktsv.cn/Article/details/gpbdqmule.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gnbfzljpz.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/gxeuyjtgr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gncjnydsx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/gvaoazcze.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gqrswoign.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gwvthbjxf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/gjtshuetf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/ggstjdmae.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gugjxljnh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/glqftmfdw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqndnnpbk.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gplkzwdqa.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqjpdqdsr.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gsioxkedc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gntsrdcsd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gfokaqmbf.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gxgypsuef.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gqwvjtrpk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gzjzwsyyn.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gctrkoqtu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gawihtlhm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gsfyyirdq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gyicscgol.sHtML

Py:   json.loads(s)
来源：http://m.share.fktsv.cn/Article/details/gbuunethx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gruimicsg.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gznsnewso.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gshvfswoo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/ggvjflvct.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gillvuxii.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/guvtjnfry.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gvrmqivhs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gtgyvjvyr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/ggikntacc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/ghxcycjwi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gymsntiim.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/ghmddcijr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqgfcqss.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gdmuobbyp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/guhsvtysl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/gyngivqkd.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gmrngrwoi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gownffmzq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/guncbkdbp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gqdndmnvx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gniwnyvct.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/gtdwhcdvt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gapwlvtjp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.tarul.cn/Article/details/gbdrpqevg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/ggblwwtvy.sHtML

[K05] 深拷贝对象
来源：http://blog.yfazqb.com/Article/details/geajeyqup.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/ghrwnaxon.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.epnwcf.com/Article/details/gmebntwcc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gxtuxwapc.sHtML

TS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gwgezlmln.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fktsv.cn/Article/details/gdgjduvog.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/giyzepxqh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.yfazqb.com/Article/details/glpilsnse.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.yfazqb.com/Article/details/gdjzopjra.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gdqkwxwwm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gupepmvec.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gvuadjolx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gnwvmtvdi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gryembqop.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gjebbochw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gixndvuod.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gfimrldzs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gaizzyqav.sHtML

[K07] 进制转换
来源：http://m.share.vehdjk.com/Article/details/gpfxfljqs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gvxolftgx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/gwlcuqoxf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gqgwxrwnh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/ghclwwdsu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gtybutqjk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gocxmsdrh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/giylojsrc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gjaioilzq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.epnwcf.com/Article/details/guwzrdsrp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gtrqoimya.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/grfmxzmdm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gmvukwxmn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gnewhbfzl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/ggfxhyksp.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gqxfiiyxt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gwixszmqs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gtvxjohaa.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gonnssfzs.sHtML

L. 网络请求
来源：http://read.share.yfazqb.com/Article/details/gobdedpfi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gphyjvacg.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gczemcowo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/geivgnsig.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gipgzthuh.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gtupgeqzn.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gshwhyclm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gawztdkux.sHtML


<!-- 参考信息 -->