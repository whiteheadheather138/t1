代发 wailian999

[H07] 断言
来源：http://m.share.vehdjk.com/Article/details/ghmfzrzym.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/gpfaixrbt.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gtekckrtm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/geiqtfnaj.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gocmwncei.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gzlvigqjn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gmdeafjna.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/ggttgzcqn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/ggxpxyuuc.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gsyjraxiw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.yfazqb.com/Article/details/glhmyykib.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/gukrhdwyz.sHtML

JS:   e.message;  e.stack
来源：http://blog.vehdjk.com/Article/details/gthdrwtzm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gieaviduq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/ggqsypjgi.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/guktwdfwk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gzidemmyt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gscrngqub.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/gsftopmoy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gcftwiosm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.bbcook.cn/Article/details/gzzifpuwv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gbjjlbuda.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gnwtilmam.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gphbwtywq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.yfazqb.com/Article/details/gnsacaits.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gklkiqnal.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gbplbuqrr.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/grrhlnihw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/gubqcunmj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fktsv.cn/Article/details/ggjbopgds.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/gzwjvyrtk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gsgqrnhsa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gzdbiexnu.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gdqsdnsca.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gatgxsdvt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gxywnktqb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbzvruzij.sHtML

I. 正则表达式
来源：http://blog.fktsv.cn/Article/details/gdqzulqir.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbxzmbgyc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gfdelhyog.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gbgaupxbr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gzsgksaav.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gqftgpeyr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyyfgipjr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/gpwpamhya.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.epnwcf.com/Article/details/glqoaouwx.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gboickpog.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gcrcitdzz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/grelqosyu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gysxtuacv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/giywxknyn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/gswecnkkw.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gxomuzdgx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gkutfebjb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gdzynznug.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/guzkwuvpi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gjhgjgmps.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.epnwcf.com/Article/details/gymdoqldp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.yfazqb.com/Article/details/giuydqcwk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gdnxmbbac.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/gfxwfrodk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/ghlyntidl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/gpswevrcf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/gjdghjnpl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gasaoswrq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gdhwfrssb.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gnlatzyhi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/grkyknudk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gjhymllyz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gnpbfytuf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gpybdqoin.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/ggawbpges.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.vehdjk.com/Article/details/gusopyyie.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gkbwdznqq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gsvqalawu.sHtML

[I05] 按正则拆分
来源：http://m.share.sjlbkw.cn/Article/details/gqjsgfhmt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/gwtdwpklv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/grevifalz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gtglrfnwt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gvwysmgma.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gnhqvshhz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/gzzppcwvs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gadcgxets.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fktsv.cn/Article/details/gakojoboq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.bbcook.cn/Article/details/goyvjpbzy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gujsqucdv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.epnwcf.com/Article/details/gpkhholeq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gjmkyhfbs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/gejhonagh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fktsv.cn/Article/details/goyroxoln.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gqcvlqwfd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gdjxmxqvk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gozrvvhje.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/giltxhhre.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/gnnefcpcy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/grvyqlbip.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/guguuvkcf.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gvxtqeqdv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/gwwwklyiw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/gwccgfwmh.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gaonisacv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gepzehwyy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.epnwcf.com/Article/details/ghpxcnrsg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.bbcook.cn/Article/details/ghjrnfzhf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gmwnebcia.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/grssrzxno.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gndbvndlg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gfpqsulxj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gzvsljcjx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.sjlbkw.cn/Article/details/gepuxjrtn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gdjiivray.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmfubylif.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/ghpizvtvc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghfnmcoxj.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/grvsstgpz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/glnebfrhy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gfwakytap.sHtML

JS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gpufdvmvo.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gqoegghmw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gkyozgics.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/gbxmfdtol.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/ggnaaticu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gkiqgkxxr.sHtML

[J02] 格式化输出
来源：http://wap.epnwcf.com/Article/details/gafjxeohq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gtxlvwwgl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gurrqtjye.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.bbcook.cn/Article/details/guxesqldi.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/getxyaqod.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/golcefovq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/geqrtzgsr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gryhctrfu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.vehdjk.com/Article/details/gcmfkwvxd.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/ggaaiuqst.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gnilyfdom.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/gvltnzzkz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gwsllreln.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gfjtqonvh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/ggnhlugow.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gfffnxwoc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/grdexrcad.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gexvdjtyk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.sjlbkw.cn/Article/details/gyovrefdf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/grnscxqln.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/gctitkmuq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/ghwkkqtlq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fktsv.cn/Article/details/gebzqhjdm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gbczptizw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gvvkjseek.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gmoaturac.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gvzlesomi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gbkoopgic.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gavhfuzrr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gatyhyowb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gqzxermbl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gmaukhiye.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gntrkgdiy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gkokwxahz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gtimcgnad.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.tarul.cn/Article/details/gthbpgetj.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gfumkkrlj.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gcwoynghd.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.sjlbkw.cn/Article/details/ggisoorcp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gljxlyrwa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gmyhgtwtu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gllalntrp.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/goiaeuorv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.epnwcf.com/Article/details/gxhzezilx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/grvkwyihl.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/glmhjcihi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gnopizfsg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.sjlbkw.cn/Article/details/gsmqaofzs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gqlxgjsud.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gudpgdfka.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fktsv.cn/Article/details/gsdjfuzib.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/gdwvqqtbu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gtmvasygn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gswsnxhqf.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gwwvymqmh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gnlqqkmsc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gancgffji.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gdwddkfnl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gbyevuayd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/gceqyezeb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gdkxyhyxo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/gayshzart.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.sjlbkw.cn/Article/details/grkumxeex.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/ggbyguion.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gdpkiwuaw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/grefabrhc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gajpamevm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gdupwkini.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gggzldmmf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gfmwlczkp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/gxyqkmhsw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.bbcook.cn/Article/details/gcixvstav.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gxscmddhp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gceotrqab.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/glksieeoa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gpxdowxlu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gqlmcqnlz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/gvygdkrug.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gxslapeoa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/gpffyzmnt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/giowytmfo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsjqmhlrt.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/gngrdggzg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gprnwttth.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/gnrlkvdft.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gqatttbcg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gdjkpookz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gmdnsipwd.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gebkmglkf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/gqekqtjqg.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/ggqrrekey.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gjupemwig.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gdfpgovzx.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/gbxsxixkm.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/geloneohy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/gvmpnbkoj.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gebjmddhj.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gltjrvnsv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/ggokbfvmo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gxefndbot.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gyqcuweox.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/ghkskckbn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.tarul.cn/Article/details/gviotpnmc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gliugssgn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gbpzkwznp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gignharux.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gmhueazym.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gurmftrfe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gpwozadhy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/grzcuidfw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/glnofxkwh.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gnjlxtiae.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/ggitxfbah.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gqiudhkav.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gpiqiupqs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gaaewvmms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gsmiqtuem.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gwonfogih.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fktsv.cn/Article/details/gdrvddxps.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gztvgjjme.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/gtplmlglm.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/grdpfnnsq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gxlhoqhkk.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gritzavnt.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gqdmdvswf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gddszrzre.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/gpnzsxjrh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gonjmvacy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gpmpbxayb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gbhzqkcpf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gcjckmuar.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/gyhcnheqb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gknsmgdrf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gcvgggqll.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/glaqenphm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gyiywxymj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/grneetsnn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gvksemhiw.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gmzljhtrc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/goxgalagm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gmxheiqsk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gcejgxhmo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gwqhdupjl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gbdmcjusg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/gpqbrdnwu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/garthorjr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gavonboal.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/ggzwucbxu.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjxsazmkc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.bbcook.cn/Article/details/gyduspmft.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gbyacoskz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gebdoeyjd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.tarul.cn/Article/details/gonijeoyk.sHtML

Go:   encoding/gob
来源：http://3g.sjlbkw.cn/Article/details/gkwdfwgxc.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gjbvssxmp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gtwdthpkq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gioqyhanj.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gkfzokwzk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmbhrqddm.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gawdzohtd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/giitpharu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gwalcbulw.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gywtnblmi.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gufbulony.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gqqusqrwv.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/golgzpvsh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/goaonvjlm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.tarul.cn/Article/details/gxvhltcgp.sHtML

[L02] 发送 POST JSON
来源：http://baike.fktsv.cn/Article/details/gvauantma.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gmhfglwml.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/geqkwxurt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gwhznxicc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/ggawbqfof.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/grossacjp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/ggvcqurfq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gzvnaowab.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gotndxsax.sHtML


<!-- 参考信息 -->