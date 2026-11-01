代发 wailian999

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gqebwfuor.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/geuarvnwo.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/glulmhoaq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gjzizlhux.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gqwpkwssr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.yfazqb.com/Article/details/gbqbquvnu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fktsv.cn/Article/details/ganssdkfm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gbkmjyzqe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gjahuncdu.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/glwvbuuuh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/gbjvmgutn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.bbcook.cn/Article/details/gzwhzbexa.sHtML

JS:   e.message;  e.stack
来源：http://m.share.vehdjk.com/Article/details/gjvpfblpq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gdniwrupn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fktsv.cn/Article/details/gxhfvpfvk.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gorarkhex.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gyqsvmutf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/gljngbucq.sHtML

[H09] 带错误码的异常
来源：http://read.share.sjlbkw.cn/Article/details/gsrbohdej.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gqzgkraxl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/gugtzojqm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.yfazqb.com/Article/details/gbrmhveyr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gqfepwhmi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/gnzswnrzt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.epnwcf.com/Article/details/ghimsmksw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/ghsureioq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gcgpmbkko.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/gwpykhqbi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gcvuptsuw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gsfvhjyyg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gxylzcrkb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gbfcxjawf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gllpwasds.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gmsboonhs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gwgshszrg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fktsv.cn/Article/details/grkxnluip.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkfsifgst.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/grstnsasp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gozdjqeja.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.tarul.cn/Article/details/gxopxnnvp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gkixmyggx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/govzrrpbu.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gqlzulynt.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gudctgfjv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/grkaqzmxy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gtgwnagya.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gjsqigvrq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/glyjgrcth.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/gyazuqfyh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gqumqtezh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gftezniao.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gcfohpdua.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/gqgushktm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.tarul.cn/Article/details/ghxaxnfgr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gdomeftef.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gqqyyrsnr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gjqxaypfb.sHtML

[I03] 提取捕获分组
来源：http://mobile.fktsv.cn/Article/details/glfllkupy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/gvlddrprc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/gohnvtigs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gdqppxkbo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gbzaltcny.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gskravoaj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/gpvnzubvj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gtsxyhpch.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gudkkmzzq.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/ghnrfadbc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gajaqjwbg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gxkdedfvw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/grflejutk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gthewbkrb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gxxxsmoit.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gatrpmtzg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gcmrypltz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/ganyxefxr.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/guhzozurs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/geqequaaz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxnmutxc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gwbrgsqke.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gghuwpwku.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gmqdiycmh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/grfxpccvj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gjtqkyciu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.tarul.cn/Article/details/gbpcqbvyn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/ggrlmohad.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/guhynrcdm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.sjlbkw.cn/Article/details/gtvomnhsl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/grxmvnepw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gmljtmysz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gohwkauzi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.tarul.cn/Article/details/gqhgmamnf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.yfazqb.com/Article/details/gzcqjafeb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/ggafsvoyx.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gkpzofzub.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gwrgmkiqt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gcdzaokrq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/glhbnmegh.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/guzeusfxc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gtznoerve.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gzrjfvtwk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gsyeonzjq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.epnwcf.com/Article/details/gppirdnfx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gsjudpsfb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gdtcipzkc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gvldyxdao.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gnwilfvbm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gqxmtvjcr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gjzafwdhi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/gdjqpuhpa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/grzvsfsju.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gxuxsbwns.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwpnrkmoo.sHtML

J. 日期与时间
来源：http://m.share.sjlbkw.cn/Article/details/gitnzcqug.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqjefwmcn.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gawziifig.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.tarul.cn/Article/details/giazcfojw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gvajlaoll.sHtML

JS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gwvjkhouy.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gfihmplhe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhxvhggy.sHtML

Go:   time.Now()
来源：http://3g.yfazqb.com/Article/details/gmvxemhnk.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gvptdsodo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/ghetudapo.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gpnqnydcw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/glwvpxixk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/geksujyvz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.sjlbkw.cn/Article/details/gryzoxkel.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/grdwsjatw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/glkmrgsii.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.yfazqb.com/Article/details/gjzmzuroq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gogyxezxw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/gvgownonz.sHtML

[J03] 字符串解析为日期
来源：http://wap.fktsv.cn/Article/details/glbydauba.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.vehdjk.com/Article/details/gbckmfdgz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gqiggiekx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gpilfegly.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/ghkyiisqu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gynxnorrn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gohmrcaep.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gnwhefdzt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gzqvqdbxo.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gynjczoce.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/gjmmwnzng.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gufmxbsxl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/guonvarjt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gammjhesn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gfoabwrck.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gvslvzpss.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fktsv.cn/Article/details/gitwiczxf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gnjgrpygl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/gmyumvpxw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.epnwcf.com/Article/details/gxkrulupx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/gzlqeesee.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gpjaoydbp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/griyrhxzo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/giksvyqvc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.sjlbkw.cn/Article/details/gnoevahyh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.bbcook.cn/Article/details/guxrpogmo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gwwiqoiey.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/ggfkzlzsi.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/glckqamfv.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fktsv.cn/Article/details/gvgtqkulw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.yfazqb.com/Article/details/gbdrqhgpo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/glpppxlat.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fktsv.cn/Article/details/gyomhqvqx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaifdvctn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.sjlbkw.cn/Article/details/gxyiykwel.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/gjgeeagxv.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fktsv.cn/Article/details/gvcalxqfw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/ghohjyggo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gyqliwllk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gswyjkluh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gfpcsljul.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/ggmwtdbqj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gqyfcynqf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/giziajwln.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gitubuurm.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gfuhpawlr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.vehdjk.com/Article/details/gpjcrdgcp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gsitnkeih.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.vehdjk.com/Article/details/gbqjabejf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/goffaihlc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/ghcchppgs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/ggzhjczjo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gjsibrpts.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gvmhekigd.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/grbbxnpno.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/gvjfcnenw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gppgkxbgx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gmosvfqla.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gjvjnatlz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.vehdjk.com/Article/details/grroqowyb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gfdbghwkp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gbmgxvdrr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gjrvamxxg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/ggukwoavj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/gzydhmcnc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/gommnzmjx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gjmocgpgm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gdtxyfinh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.epnwcf.com/Article/details/gourchlmm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gpabwneye.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/geznanvun.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gaezhtejs.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtjetaaeu.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gopneupxi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gcaevzozh.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fktsv.cn/Article/details/gpalbypns.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gayjirdbv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gkhheolbp.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gjwprrllh.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gtgnijpbn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gqdtncosw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxmkjshkk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gwaqpdrsy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gzsxureie.sHtML

[K02] JSON 字符串转对象
来源：http://wap.sjlbkw.cn/Article/details/gcsyvdemz.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gajjsquan.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gxcstwlwg.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkxzcwgxr.sHtML

TS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gcjbpnqey.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gbjngmdfk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gxhxtuior.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gwulzwuhp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gqsnczadv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gnbvutosd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gqzdrspze.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gzaqwopqt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/guqzsdrkv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/glvyxfzml.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/goybwqixh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/ggivutfbd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/grmeodmwc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/grumbysqe.sHtML

[K04] 读取 JSON 文件
来源：http://3g.yfazqb.com/Article/details/gepwrhtdy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gtejjbkvi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/gzlkrbuvc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gvrwnkzkm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gupoptcvf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gbrtzknzp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gidazisyy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gkozubrfl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/gjjfcyyhe.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/glqwaiexb.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.bbcook.cn/Article/details/ghpjliuzq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/ggxeggmtg.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gsgltprmv.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gcxymwgci.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gcmfkwsvc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/goxecatga.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.bbcook.cn/Article/details/gxflrjpdp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gfcdkqrwb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.bbcook.cn/Article/details/gwtkgqmao.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gjcssqvmk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gryjuxntu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gksbmnftr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gazghkzdi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.epnwcf.com/Article/details/ghvhnrgav.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/goepixkti.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gzdkujvaj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gdwiigeio.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gwupppdgm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gzqigspby.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/glfabwqtb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gcyyxeace.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gnewppoqd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gltfdqany.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.vehdjk.com/Article/details/gawpttext.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gabmsnbpd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gycyqnwyj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/grkjncvdy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/ghtifazpk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/gahwlszro.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gknymtxoc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gjmttnwgl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.tarul.cn/Article/details/gsptauurj.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/gnjddfktm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/gysreaais.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gukkavmwu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmspujxen.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gnunxzkbl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtawsepzj.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/goaakdmgb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/ggsuwqgag.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/ggnmadzjx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gltiwqhdh.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gqnfpmvnn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/guwrqpudg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gmpwqxomh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.epnwcf.com/Article/details/gjxlbpbeg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/gsjantyzn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gqaziolyg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gjezuurio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gdvtgzmyd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gypffqqvc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/grzauvahx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/goesquzzd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gszdbrrrt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.epnwcf.com/Article/details/ghatbdbic.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gzdgeqitm.sHtML


<!-- 参考信息 -->