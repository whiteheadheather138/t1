代发 wailian999

[H03] 主动抛出异常
来源：http://due.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://lca.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iyo.yonumen.top

JS:   throw new Error("错误信息");
来源：http://yfi.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://fml.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pop.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://spe.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mjb.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://hcf.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://dly.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://rtl.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://ivw.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://pay.uphjek.com

TS:   class MyError extends Error {}
来源：http://req.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://hyb.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://elz.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://txm.c1oappe.top

C#:   class MyException : Exception {}
来源：http://dhu.xziqi.cn

[H05] 捕获特定类型
来源：http://cxb.sjlbkw.cn

Py:   except ValueError as e:
来源：http://hkg.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pkn.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://swi.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://uiz.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://lud.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kiz.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://eiy.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vem.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://rzq.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://fzo.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ymb.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://fcl.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vas.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hek.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://grn.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://elw.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://kgz.yj20258888.top

[H07] 断言
来源：http://jcd.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://flc.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://bmr.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://mrc.daxiang520.top

TS:   console.assert(x > 0);
来源：http://fgl.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://lwn.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qgw.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zfo.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://xip.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://ksp.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://jrp.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://amx.ehwqpu.com

JS:   e.message;  e.stack
来源：http://wul.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ukf.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://irc.jiagoushi.top

Go:   err.Error()
来源：http://mtc.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://kkg.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://ztf.zdbjq.cn

[H09] 带错误码的异常
来源：http://nne.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tog.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://wfv.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fcf.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pbz.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xay.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://feo.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tfo.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://zie.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://occ.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jzz.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://euq.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pva.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qtv.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://urr.cqqwz.cn

Go:   defer f.Close()
来源：http://lrx.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sqj.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rto.cqqwz.cn

================================================================================
来源：http://dhl.svipenyu.cn

I. 正则表达式
来源：http://rmk.zycfv.cn

================================================================================
来源：http://mey.gaohongyu789.top

[I01] 判断是否匹配
来源：http://ukn.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ycz.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fru.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://mvb.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://hia.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lzg.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sbe.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://tft.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fcx.xziqi.cn

[I02] 提取所有匹配
来源：http://heu.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://fnz.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yem.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://huq.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://vwh.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fwh.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://srd.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://phq.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://czr.guannengcc.top

[I03] 提取捕获分组
来源：http://mmx.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nxl.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lwl.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vvc.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aza.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://syc.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pgq.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pyk.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tve.cdnleiting.top

[I04] 正则替换
来源：http://cpr.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qlk.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aaf.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://tzb.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://tvg.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://ioy.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pjx.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uxk.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://det.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://euy.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tfm.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://amz.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://ytt.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://duq.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://ugh.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cml.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bny.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://owc.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xck.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yaa.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iyk.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aob.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hza.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gar.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dfr.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://apl.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://apl.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://nyg.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qrx.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dts.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gtq.zhiwuduotai.top

TS:   /error/gim
来源：http://haa.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zqi.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lix.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://dtl.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wkd.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://vku.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hgq.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://htu.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hze.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxl.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://muj.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gdk.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xnj.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hrm.haohaochexian.top

================================================================================
来源：http://yfh.yvedp.cn

J. 日期与时间
来源：http://lyh.gotoacloud.top

================================================================================
来源：http://jcj.smart0.xyz

[J01] 获取当前时间
来源：http://djb.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rtw.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jsq.ydzc1.top

JS:   new Date();  Date.now()
来源：http://thl.xuanzx.com

TS:   new Date();  Date.now()
来源：http://fni.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kzf.sufxvd.cn

Go:   time.Now()
来源：http://pda.xuanzx.com

Ruby: Time.now
来源：http://iyq.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://utf.yonumen.top

[J02] 格式化输出
来源：http://uhl.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://viz.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pkz.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ikx.birdmap.top

TS:   d.toISOString()
来源：http://hac.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://agp.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://era.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://akk.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rxv.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://zdc.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ozo.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mka.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://iez.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://eaq.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://agr.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nbs.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://qcm.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ryc.cucudq.cn

[J04] 时间戳与日期互转
来源：http://sud.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ght.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eil.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yfw.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fxw.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hxk.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hkf.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ixx.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bzj.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://ljj.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://egh.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://arz.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ugl.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bwn.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://iee.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iyc.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://iwh.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://myk.snrcjt.cn

[J06] 计算两时间之差
来源：http://tog.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://rly.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://lah.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oot.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iku.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://mqv.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://tmd.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://ewt.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://smj.xuanzx.com

[J07] 比较两个日期
来源：http://tmn.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://vvc.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ykb.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://gqx.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vnl.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jry.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://qlv.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ukk.vehdjk.com

[J08] 提取年月日与星期
来源：http://fzh.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bhn.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yrh.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ysw.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aqb.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dfh.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ogs.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xww.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vnj.guowangkeji.top

[J09] 时区处理
来源：http://nyx.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ljz.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fog.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uwc.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kpu.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cqx.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oau.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cfa.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tag.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://pve.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://deg.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bod.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dqq.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bzj.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uws.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ccg.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://npk.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://byh.gotoacloud.top

================================================================================
来源：http://lqf.sufxvd.cn

K. JSON 与序列化
来源：http://nqy.guowangkeji.top

================================================================================
来源：http://rpu.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://jhi.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ufm.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ndh.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://zth.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://ayg.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dkb.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://pre.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://xza.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://txc.sysykeji.top

[K02] JSON 字符串转对象
来源：http://ikj.yongpay.top

Py:   json.loads(s)
来源：http://bwx.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ofe.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://vsh.yueranfly.top

TS:   JSON.parse(s)
来源：http://vdb.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lsb.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://rts.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://hmb.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ckc.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://fty.sufxvd.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gce.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://roj.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wfk.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lju.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dww.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ibg.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://kam.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mhv.redwolf501.top

[K04] 读取 JSON 文件
来源：http://hxn.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jrc.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kmv.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qqe.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ntj.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jzv.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nwh.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pff.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rrb.bbcook.cn

[K05] 深拷贝对象
来源：http://nor.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://xcu.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://ufc.ydzc1.top

JS:   structuredClone(obj)
来源：http://fgn.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://arh.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pew.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lqw.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eny.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://srr.birdmap.top

[K06] 解析 URL 查询串
来源：http://mfj.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vdh.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gym.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rco.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zol.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oht.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dlh.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ydy.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ndl.sxryk.cn

[K07] 进制转换
来源：http://wgd.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ofh.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yph.wangshuangyany.cn


<!-- 参考信息 -->