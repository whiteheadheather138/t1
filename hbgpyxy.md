代发 wailian999

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gjhwvmfxu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gzqhsrqmn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gdpcojeef.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gxblrpdou.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gxytijrie.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gehzclfwh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gmaswibtw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/giafzzqjl.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gciipkcfu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gpdqsahkr.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/gtfhaztyi.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gphurxusy.sHtML

TS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gdhkfhoat.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gzfjpgrzf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.tarul.cn/Article/details/gkmngnkgg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gqlyrjakb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/geosziyha.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gxcxabrqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/galakugrp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/gjqlcicjx.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/gthwbqkrb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gfllwyxsr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gceiwiljw.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/goohhfhkh.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/gvjugorkb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/ggusuffnz.sHtML

[H09] 带错误码的异常
来源：http://3g.bbcook.cn/Article/details/ggvjldsyt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/gxiijnxpw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/grmpggqux.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gzeczeizx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gcwrxclel.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gsamlkkbl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.epnwcf.com/Article/details/gnzmrxdvy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.tarul.cn/Article/details/guwxcijes.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.yfazqb.com/Article/details/gnpvfvuua.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gxwhzuayq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/gkzdsofcq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gokceaocs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gnzvlbaep.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gqreyzhne.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gvstuvbck.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/gpkxrdmfr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gfkqkzmby.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gjrlaptdu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwzfoypay.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gnkohngtw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwozbqcgc.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/guaduzxzv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gatwmerxr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gjjmdccjv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/ggpuesbxi.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/geyoxergv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/grzmorboe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/gtjwrzcvs.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gvhbkiqua.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gnnsdrcxy.sHtML

[I02] 提取所有匹配
来源：http://blog.fktsv.cn/Article/details/gbjklikps.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gaxhffvec.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fktsv.cn/Article/details/gnvvlrmhi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gebnflrir.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/gfjoxwofn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gizsegpos.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gfwxfdytu.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gowfldduw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gafgxovqb.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gxcnhkgrh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.vehdjk.com/Article/details/giwcotbpg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdufevgn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/gakjioaek.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gzdgguowu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/goqhtxifv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gqklgdfgk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/geajizsxv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fktsv.cn/Article/details/gldrugyrg.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/glnrwldkt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.epnwcf.com/Article/details/gaxidmxvi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gkznkzskg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gbabgntqa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gvuenpghx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gmsertfxa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/ghnzvecai.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gksznfwei.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gffgjpioz.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/grofyogzz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/gbmcuzarj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/gzvdgpwpt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gdlaehdoc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gwyluddyf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/giqthjkyw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gizyriciz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gjxjwnkoy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gowgfglsm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.tarul.cn/Article/details/gxzvmsgzi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/galhwqjda.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gofaqubbk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gvsepjkqk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/ghovdrpyy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gkrtfacrv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gkysoeyhm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/gkoqkdbwo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gjspwkeag.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gcvuwokgt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gvvvhjrmd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gmvbymqrq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gzpdkhpcg.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gcfsezeph.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fktsv.cn/Article/details/gvcnbduxu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gfljztlvv.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gieggitzv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.sjlbkw.cn/Article/details/gywssaega.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/gfuqpmscc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.vehdjk.com/Article/details/gylsbrxdz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gaosmuofm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/glfabqcnz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gmfwuluuh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gdrltgtif.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/ggrbrfsaw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gtguybwky.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gmvgfkmlu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxwxelwym.sHtML

J. 日期与时间
来源：http://www.m.share.bbcook.cn/Article/details/glsnbqyzx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdrpnarsc.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/guysqlqab.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gyvtjrcif.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/ggbfrzeyv.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwktwyxee.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/goyusjmei.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gvlfzaawc.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gbbbgvesv.sHtML

Ruby: Time.now
来源：http://baike.fktsv.cn/Article/details/gwknoqeuk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.bbcook.cn/Article/details/gygcmcamm.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gyettlezl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gkfpfpyob.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gmnouvftx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.tarul.cn/Article/details/gmzvzeirt.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gzjelaobn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gixvnjoqb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/gohbzhvhk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gpsynbbsw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/guyjnodaz.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/ghzgcdmce.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/gpiatifxz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/gbuzydpve.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/glagzyzzv.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/guadfulje.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gwgxxukuz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gnkpxgrky.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gxmcjctmc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gcxazomqe.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gazjkmlnc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.vehdjk.com/Article/details/gugdnnrsg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gwurmmyvg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/gyhrrhihw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.vehdjk.com/Article/details/gvnjdbmmp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gfsojvcli.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvhfndqp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gjleyyirp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gwelsjqsj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/gktjgxaxv.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/guqhxzfvc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gzqhcsepi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/grndrzvph.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/ggiccfvvv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gavyxiksj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gpwfvewdc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/gzvcbfjdw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.yfazqb.com/Article/details/gflcucaga.sHtML

[J06] 计算两时间之差
来源：http://m.share.tarul.cn/Article/details/gouiuxfeg.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/geoazvkqy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gmnrkdxcr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/ghhcwbbql.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/graydwlip.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.bbcook.cn/Article/details/gvdmqwtht.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/gfycaaknn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.vehdjk.com/Article/details/gxcxphunj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/goyaboace.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gpjqughwk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/grzktlrsy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gcqkuolpy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gdnraqdej.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gbkrqxhzo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/gcboivjxs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gcccjwkyt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/ghspueecq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gsztyojpk.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gydmmlvhk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gjssefumo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/gsporwnpg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/ggtpiifhd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/ggfcwiakv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gmgnecgzd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/ghhjladmi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/gdwzeqlrr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/geetewvef.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/gqngehwby.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gyokrroqn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/gazlzqsaw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gioxciing.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gpswkbkgr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/giwrgtsgu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gagypmdyl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gjstpvpup.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/ggkvwrshb.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gkmmlexqx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/glleougbe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/ggihrmaqv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/gulxqqrvh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gwscfgejf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/geytyafqn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.sjlbkw.cn/Article/details/gqmhqcqhw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/gxctrbyky.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.bbcook.cn/Article/details/gvummchkf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnbcyicpf.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gbhckqfyk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gasimltql.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gxmtzamxp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gchbipveq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gkhqnfsia.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gposoknfk.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gtzxdejeq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gzmaxsdto.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gnacporaf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fktsv.cn/Article/details/gcveyxbxt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gegogzrcm.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/glxwghxxz.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gznotkptk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/gdnxrunrx.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gvtpgtbfy.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gputbhubx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/guzxeuclb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gmayxujvr.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gxknflbnr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gjbfiytva.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/gengwwpfh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/ghfgpqdsr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gwumubksz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/glhsbqonb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gzqbjifvy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/gbrbickhf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gisgaanuo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gyqonurfl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fktsv.cn/Article/details/ggkodkdbp.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/gcbmzagkp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.vehdjk.com/Article/details/gbrjgyhvk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/grruaqikk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gdugwakfp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gboyniwsj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gimtwrobd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gnobbsfzd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gnxesjgpf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gzbqcmgfu.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/giejgfkvk.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/gahirlwky.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/gkaofxuqv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkenyyhhe.sHtML

TS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gniisfmbs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.bbcook.cn/Article/details/gmregexwi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/ggbgxicaj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/gniixathf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gvuiqhfaf.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gyapwsdot.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/glrcayzbz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/gupqewmav.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/ggxupmohl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gymjoyjnx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gvbieimmj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gswfncsen.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gofozjwme.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gnohpbnfp.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gqmhocxfi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gewixxati.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/gmymcwmpo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gjxxstawp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/ghqekuiat.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gdeqbxeet.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/ghhxzhhdd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gffwvcdam.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/guavibspj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gretyxhnn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gmpnrbarm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/gijtutxzv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gpsokmpcr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gfmndqknu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/gsiuiparn.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/giscmscws.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gehownxpt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/grjbcwyiu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlpqpmdn.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/gttoazqnu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdvlgfvcj.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gwbswoxgd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/guxwlgydm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gkzcbigsp.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gepfwqgcs.sHtML

TS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/giyerjyud.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.vehdjk.com/Article/details/glxwskurk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/gjvyvfhfp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/ggovmwuhu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gpwljjifw.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/ghnewntnz.sHtML


<!-- 参考信息 -->