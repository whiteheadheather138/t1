代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://poa.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://jbm.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://lhh.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aok.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://pnm.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zyg.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zsk.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zpp.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://lkr.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://qcd.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rff.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://hyo.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://rpi.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://chu.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fvz.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nqh.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://xea.xziqi.cn

[H04] 自定义异常类型
来源：http://jdx.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://get.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://zkp.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://ime.yuxming.cn

TS:   class MyError extends Error {}
来源：http://baj.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://ilk.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nxv.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://tll.gzhubu.top

C#:   class MyException : Exception {}
来源：http://ynp.yongpay.top

[H05] 捕获特定类型
来源：http://xvn.nanxuanxn.top

Py:   except ValueError as e:
来源：http://msw.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cgp.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://ilw.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://xvy.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://svm.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://asg.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://pcy.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pia.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://gtl.fehbvm.com

Py:   value = d.get("k") or default
来源：http://wpr.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://mhy.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ucv.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://jdx.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ust.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bui.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://vga.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://fsc.hcnkem.com

[H07] 断言
来源：http://wze.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://ubi.9152youxi.cn

PHP:  assert($x > 0);
来源：http://vyr.zycfv.cn

JS:   console.assert(x > 0);
来源：http://xrk.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://zpc.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://jpn.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ukt.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://ssr.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://uoq.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://bik.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://iqd.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lgy.cashguo.top

JS:   e.message;  e.stack
来源：http://ymz.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zcu.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yek.jinqigufen.top

Go:   err.Error()
来源：http://eax.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://gnr.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://pcn.jianghu66.top

[H09] 带错误码的异常
来源：http://hfr.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qer.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sfl.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ydu.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nvs.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffs.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uqw.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fcf.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://xmz.aibaodan.cn

[H10] 资源自动释放
来源：http://pup.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jdn.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kll.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xys.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tnz.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dbn.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://hxm.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gmn.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jgx.fehbvm.com

================================================================================
来源：http://goc.ehwqpu.com

I. 正则表达式
来源：http://zuv.pengpengdd.cyou

================================================================================
来源：http://vgr.sxryk.cn

[I01] 判断是否匹配
来源：http://khg.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://drj.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://iey.mhx1999.top

JS:   /\d+/.test(s)
来源：http://guc.yfazqb.com

TS:   /\d+/.test(s)
来源：http://nvu.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jri.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kdm.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://ooc.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qut.jyoumei.cn

[I02] 提取所有匹配
来源：http://fop.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://fwf.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qcn.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rrp.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://wzw.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vrz.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tkd.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://dtd.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pme.zdqjudy.top

[I03] 提取捕获分组
来源：http://zqz.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bgl.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tqc.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://npd.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://esr.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qye.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dcr.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ped.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xkz.jyoumei.cn

[I04] 正则替换
来源：http://doz.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ehc.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bwu.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://len.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://hta.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://vbi.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wql.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rqg.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sti.yuxming.cn

[I05] 按正则拆分
来源：http://wuy.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mbx.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ope.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://axj.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://hqp.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://mxr.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wno.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://urc.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tno.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lno.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uyk.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oer.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fov.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yne.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nah.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xpj.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oeu.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fde.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://lzt.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hzs.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xhh.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lef.ctjpmb.com

TS:   /error/gim
来源：http://smu.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ejq.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hgf.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://mor.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ykh.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://jzo.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yxs.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zqf.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nns.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmq.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zbw.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://elo.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ugu.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dtg.yongpay.top

================================================================================
来源：http://ldm.gotoacloud.top

J. 日期与时间
来源：http://ldr.sxryk.cn

================================================================================
来源：http://gwb.jiagoushi.top

[J01] 获取当前时间
来源：http://zpt.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xol.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ncn.fehbvm.com

JS:   new Date();  Date.now()
来源：http://hpc.bbcook.cn

TS:   new Date();  Date.now()
来源：http://tll.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://njq.hongshengwenyu.top

Go:   time.Now()
来源：http://ujz.52xcode.cn

Ruby: Time.now
来源：http://wog.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fjg.zdqjudy.top

[J02] 格式化输出
来源：http://zvr.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yga.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gfb.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nbh.52xcode.cn

TS:   d.toISOString()
来源：http://rag.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vdk.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://njh.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tkb.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nag.bjfxy.top

[J03] 字符串解析为日期
来源：http://zga.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vcc.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jqe.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://zxi.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://ipo.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://oqn.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dvi.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://ncy.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xwh.tanke756.top

[J04] 时间戳与日期互转
来源：http://zad.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gez.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vwb.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hbf.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://psm.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ujk.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ftz.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://szi.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tky.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://fxx.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://jmr.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mct.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ujj.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xrz.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://ugv.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tso.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://axr.sufxvd.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cgv.xziqi.cn

[J06] 计算两时间之差
来源：http://tnw.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://wtc.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://vqp.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nnz.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://afs.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://yuq.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://ihh.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://xer.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://ldf.feifeiyinyue.top

[J07] 比较两个日期
来源：http://wpv.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://wqg.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pyz.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://dho.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://hke.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jvw.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://erz.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wtg.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://kcf.chenzaomai.com

[J08] 提取年月日与星期
来源：http://ljm.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xmi.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pra.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pbt.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jly.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bpv.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrd.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://crf.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pjn.ywan-chungtsiang.top

[J09] 时区处理
来源：http://qet.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kpn.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pzk.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://imp.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qve.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uec.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ama.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lrc.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qno.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://ijh.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wan.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gri.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pnt.shangyingyoupin.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kqh.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wzy.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jrq.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wsr.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bjw.jinghuilouyu.cn

================================================================================
来源：http://raq.hysaishi.cn

K. JSON 与序列化
来源：http://ktn.nanxuanxn.top

================================================================================
来源：http://kti.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://gch.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cqg.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bas.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://etp.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://ows.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://neq.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://jjb.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://wsy.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bki.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://hgm.bbcook.cn

Py:   json.loads(s)
来源：http://mub.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yqu.havefunace.top

JS:   JSON.parse(s)
来源：http://ago.hcnkem.com

TS:   JSON.parse(s)
来源：http://yjk.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tuw.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://jtl.ybcxt.top

Ruby: JSON.parse(s)
来源：http://brj.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pvy.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://zdd.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cpu.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hln.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mku.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jmp.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dxh.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vwr.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://bzx.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://umc.c1oappe.top

[K04] 读取 JSON 文件
来源：http://nvo.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vej.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bws.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wqi.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://irk.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nia.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://buy.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://hpj.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wny.jinqigfzy.top

[K05] 深拷贝对象
来源：http://wyx.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://qla.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://jmw.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://eiw.aibaodan.cn

TS:   structuredClone(obj)
来源：http://qsg.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dvu.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uhp.jiagoushi.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qox.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ngj.fehbvm.com

[K06] 解析 URL 查询串
来源：http://jxe.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qtq.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mfj.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://app.daria6918.cn


<!-- 参考信息 -->