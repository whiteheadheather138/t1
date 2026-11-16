代发 wailian999

[H03] 主动抛出异常
来源：http://bxb.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://dml.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ozw.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://wem.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://qrw.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fyy.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fyf.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mzd.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://nfm.mhx1999.top

[H04] 自定义异常类型
来源：http://jzl.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://bma.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ewo.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://tdt.fzhhl.top

TS:   class MyError extends Error {}
来源：http://gza.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://njj.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rlp.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://crj.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://mva.jlsjyb.cn

[H05] 捕获特定类型
来源：http://huj.cashguo.top

Py:   except ValueError as e:
来源：http://rzd.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zgn.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://djj.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://dwp.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://ksu.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lvp.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://ixf.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ejm.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://igp.yvedp.cn

Py:   value = d.get("k") or default
来源：http://jue.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://krw.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://yun.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://smc.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vgu.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tqt.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://uec.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://ykv.cdnleiting.top

[H07] 断言
来源：http://ivf.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://gbs.gzhubu.top

PHP:  assert($x > 0);
来源：http://hln.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://esb.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://lzk.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://ils.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sqb.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://drk.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://jdi.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://wwj.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://znu.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yyw.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://phh.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cua.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uyk.xziqi.cn

Go:   err.Error()
来源：http://fse.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://jpt.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://dbj.gzhubu.top

[H09] 带错误码的异常
来源：http://ycn.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xwn.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ozw.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cez.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xfj.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://edx.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cyi.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://lxz.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xix.xziqi.cn

[H10] 资源自动释放
来源：http://bqp.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vkk.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zve.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://myg.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vhb.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://psu.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://fab.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bqq.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mmi.gotoacloud.top

================================================================================
来源：http://rum.yanxiufei.cn

I. 正则表达式
来源：http://way.xylfe.cn

================================================================================
来源：http://nov.yfazqb.com

[I01] 判断是否匹配
来源：http://vrn.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kde.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://huw.birdmap.top

JS:   /\d+/.test(s)
来源：http://uyd.jianghu66.top

TS:   /\d+/.test(s)
来源：http://ogf.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qnx.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rue.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://tmu.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gxh.hesvh.cn

[I02] 提取所有匹配
来源：http://ece.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://ews.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxl.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xpv.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://uoe.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zcp.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://owl.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://dds.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cjd.hammf.cn

[I03] 提取捕获分组
来源：http://jsj.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dgm.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hmm.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://syz.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ohe.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vgc.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xna.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iic.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zyd.vehdjk.com

[I04] 正则替换
来源：http://hpp.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://cvb.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rkr.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://hck.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://lwe.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://djn.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ufk.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://tqz.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wbt.jyoumei.cn

[I05] 按正则拆分
来源：http://eke.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://plu.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vcp.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://nmt.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://swq.xziqi.cn

Java: s.split("\\s*,\\s*")
来源：http://fgm.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://usr.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://krn.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://epe.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kjr.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pup.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qiz.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oae.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vzb.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jqi.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hxd.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ugm.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://prs.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://lva.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://igt.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mpe.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rgr.316326.xyz

TS:   /error/gim
来源：http://mse.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://awe.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xws.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://hyf.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgc.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://ffb.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://atn.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vbv.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://imx.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ajo.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://brn.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sai.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hep.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mmz.cheryme.top

================================================================================
来源：http://wgl.xuanzx.com

J. 日期与时间
来源：http://byp.yfazqb.com

================================================================================
来源：http://tif.fzhhl.top

[J01] 获取当前时间
来源：http://onq.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ufw.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lbr.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://tyu.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://qlq.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://kmw.tianlin.xyz

Go:   time.Now()
来源：http://ctg.zhaomingkeji.xyz

Ruby: Time.now
来源：http://tnr.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zlp.pycfn.com

[J02] 格式化输出
来源：http://tkm.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wkr.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mis.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lro.bbcook.cn

TS:   d.toISOString()
来源：http://gey.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://niq.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ygn.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wum.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ojh.cucudq.cn

[J03] 字符串解析为日期
来源：http://lha.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://khn.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iwa.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://asl.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://dkd.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://ddp.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://siz.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://tqb.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ibx.xylfe.cn

[J04] 时间戳与日期互转
来源：http://sff.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yjm.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sfm.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vwj.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qzm.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jta.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://knr.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xqk.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eld.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://tvy.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://idw.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ggh.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mwd.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bri.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://ttl.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ras.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://uvf.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://tox.chenlongwang.top

[J06] 计算两时间之差
来源：http://pap.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://bdz.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://vup.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kug.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gfn.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://giu.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://amz.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://fwg.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://fmf.yanxiufei.cn

[J07] 比较两个日期
来源：http://jeo.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://ury.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bcz.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://bht.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kbm.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qrz.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oos.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://nnv.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://dby.tanke756.top

[J08] 提取年月日与星期
来源：http://ofo.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cbx.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fhc.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oeu.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ifp.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yfc.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fzl.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://coe.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kyf.andypj.xyz

[J09] 时区处理
来源：http://igs.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://umh.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://exz.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qdz.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqq.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gkg.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oxo.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nph.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xrx.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://mgg.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://srd.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://scq.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wzp.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cie.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lhz.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tbf.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wtr.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dkx.zhijiandao.cn

================================================================================
来源：http://roh.zhiwuduotai.top

K. JSON 与序列化
来源：http://bcq.yonumen.top

================================================================================
来源：http://naq.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://xgd.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rva.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://til.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://phi.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://amp.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cdq.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://jzp.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://wyj.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://voa.yfazqb.com

[K02] JSON 字符串转对象
来源：http://aft.ydjk.org.cn

Py:   json.loads(s)
来源：http://tfj.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fvf.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://zxv.ppjwa.cn

TS:   JSON.parse(s)
来源：http://vwb.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mub.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://pll.cheryme.top

Ruby: JSON.parse(s)
来源：http://xyr.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gcv.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://xfe.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ryd.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rgq.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://etn.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mtb.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eca.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://phy.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kmw.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ayf.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://uio.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oqj.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dto.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfc.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mel.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nbb.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mim.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xkx.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hgb.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://jti.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://ejo.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://mng.zdqjudy.top

JS:   structuredClone(obj)
来源：http://sux.jinqigufen.top

TS:   structuredClone(obj)
来源：http://bmb.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://inn.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pqr.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qtg.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xbq.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://tge.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rpr.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ckv.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dci.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kus.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cxx.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xxo.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jxp.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://agw.fengsongda.top

[K07] 进制转换
来源：http://xpz.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wld.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vtd.guannengcc.top


<!-- 参考信息 -->