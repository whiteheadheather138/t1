代发 wailian999

TS:   throw new Error("错误信息");
来源：http://mdm.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://amy.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://emr.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ddr.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://eoe.pycfn.com

[H04] 自定义异常类型
来源：http://yle.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://wsf.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://vhg.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://dcj.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://rrb.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://zdc.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iyd.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://nsm.sysykeji.top

C#:   class MyException : Exception {}
来源：http://fiv.316326.xyz

[H05] 捕获特定类型
来源：http://fzl.chenlongwang.top

Py:   except ValueError as e:
来源：http://lfh.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://scj.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://ngi.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://fzn.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://yzl.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pvt.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://ihz.jiagoushi.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qem.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://mgq.fktsv.cn

Py:   value = d.get("k") or default
来源：http://soe.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://olz.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hsp.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://puh.aizwys.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dbw.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://guf.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://few.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://gzc.chenlongwang.top

[H07] 断言
来源：http://kbp.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://ojj.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://zvv.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://hdi.ybcxt.top

TS:   console.assert(x > 0);
来源：http://xav.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://nce.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://idl.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://lde.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://jer.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://ckc.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://aah.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ryc.yueranfly.top

JS:   e.message;  e.stack
来源：http://zgi.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rrm.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dqf.kuanghao11.cn

Go:   err.Error()
来源：http://arl.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://kqq.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://hco.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://yrp.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qud.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rkn.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://smp.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://elz.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://edb.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xxq.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://fbn.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dkd.meibo888.top

[H10] 资源自动释放
来源：http://cwk.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ezd.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://goo.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://syg.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xoy.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rfv.shangyingyoupin.top

Go:   defer f.Close()
来源：http://fjv.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ppc.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bpc.guannengcc.top

================================================================================
来源：http://edj.quarkkingdee.top

I. 正则表达式
来源：http://xqh.wangdashe.top

================================================================================
来源：http://voo.daxiang520.top

[I01] 判断是否匹配
来源：http://ioi.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sdv.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eag.redwolf501.top

JS:   /\d+/.test(s)
来源：http://ltf.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://aiv.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yop.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wft.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://eaf.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qzn.xinyue.icu

[I02] 提取所有匹配
来源：http://mcv.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://eqj.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fsu.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pwh.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://xwi.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nff.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://row.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://vbn.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tyk.zdbjq.cn

[I03] 提取捕获分组
来源：http://rxx.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mvs.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://esf.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fte.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oxq.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tfq.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wvq.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mhl.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://twl.hongshengwenyu.top

[I04] 正则替换
来源：http://yrr.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ncf.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rcm.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://nxq.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://htz.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://srx.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://oyy.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wip.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ilj.guannengcc.top

[I05] 按正则拆分
来源：http://iww.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://bgr.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fxc.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://qla.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://tun.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://tdi.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lkl.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://npx.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jgu.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hft.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xyo.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://agk.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rlj.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zru.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gxz.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hjq.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://enm.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fzg.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://qsr.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uxk.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wnh.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lxy.jinqigfzy.top

TS:   /error/gim
来源：http://yga.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gmu.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://efq.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://fjw.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zxv.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://srq.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nze.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://elu.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dep.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxz.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jlu.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://och.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mej.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vkf.jinghuilouyu.cn

================================================================================
来源：http://lwp.jiagoushi.top

J. 日期与时间
来源：http://zeq.sysykeji.top

================================================================================
来源：http://rmm.tianlin.xyz

[J01] 获取当前时间
来源：http://euk.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lag.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uso.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://nou.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://gcf.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fmh.yonumen.top

Go:   time.Now()
来源：http://rpv.nwbrower.top

Ruby: Time.now
来源：http://rqf.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ztx.shanyushiyangtech.top

[J02] 格式化输出
来源：http://ifn.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://myt.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://daq.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ohb.tianlin.xyz

TS:   d.toISOString()
来源：http://jmo.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lwz.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cym.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sch.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uvo.aibaodan.cn

[J03] 字符串解析为日期
来源：http://cfa.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://igo.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cho.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://kum.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://jko.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://qlw.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tua.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://ccq.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kjs.ydzc1.top

[J04] 时间戳与日期互转
来源：http://irq.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vwe.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ygj.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yma.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://koz.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ang.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sqk.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yul.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hxz.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://uak.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://oda.cashguo.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kxp.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nid.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qfz.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://izx.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dav.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://ahe.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://isu.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://axi.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://ybe.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://eyb.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jxt.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lng.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rwe.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://zgz.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://zhg.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://zjq.feifeiyinyue.top

[J07] 比较两个日期
来源：http://okw.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://eql.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tnh.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://yfe.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tpz.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wiq.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fug.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lhw.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://unc.pycfn.com

[J08] 提取年月日与星期
来源：http://spo.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qda.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kpj.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bqn.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://skp.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lbk.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xhl.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pbx.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rux.hywenlv.cn

[J09] 时区处理
来源：http://ksd.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nvi.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yzt.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ypg.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvr.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bvh.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tzd.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dga.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fwi.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://xqe.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gjp.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yra.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://njt.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ziw.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rca.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://spq.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jvg.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mvz.xylfe.cn

================================================================================
来源：http://lsi.yonumen.top

K. JSON 与序列化
来源：http://tys.iojbl.cn

================================================================================
来源：http://heh.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://wdj.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kox.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tza.cheryme.top

JS:   JSON.stringify(obj)
来源：http://kae.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://zuk.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mjo.wangdashe.top

Go:   json.Marshal(obj)
来源：http://vzv.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://bbf.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yoh.bbcook.cn

[K02] JSON 字符串转对象
来源：http://min.wangdashe.top

Py:   json.loads(s)
来源：http://dtt.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vnc.bbcook.cn

JS:   JSON.parse(s)
来源：http://ogm.ehwqpu.com

TS:   JSON.parse(s)
来源：http://mov.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vfo.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://nir.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://ple.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bss.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://hoe.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ozi.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wmr.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://isu.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pvy.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uer.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xdd.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://xau.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zdh.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://fjm.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://umg.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ggb.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qfc.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrf.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ovw.guowangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aup.9152youxi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://coa.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wdd.hcnkem.com

[K05] 深拷贝对象
来源：http://vxg.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://jwe.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://rwh.sufxvd.cn

JS:   structuredClone(obj)
来源：http://ywm.cashguo.top

TS:   structuredClone(obj)
来源：http://bes.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://snf.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://slq.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://skn.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nwo.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://kvm.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yqn.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dsg.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sqd.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afx.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://khl.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://iul.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sbr.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://emo.sjlbkw.cn

[K07] 进制转换
来源：http://sgx.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qaa.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xtx.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zka.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rve.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jvk.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://epj.zhaomingkeji.xyz


<!-- 参考信息 -->