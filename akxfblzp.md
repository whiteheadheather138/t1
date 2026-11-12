代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://grv.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ynd.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://spb.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://qsv.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://glc.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vzc.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cae.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pkh.hysaishi.cn

[H03] 主动抛出异常
来源：http://djz.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://axb.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tik.pycfn.com

JS:   throw new Error("错误信息");
来源：http://auj.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://cns.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eoh.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://evx.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yjo.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tgp.sufxvd.cn

[H04] 自定义异常类型
来源：http://svc.tanke756.top

Py:   class MyError(Exception): pass
来源：http://htn.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://ulm.fehbvm.com

JS:   class MyError extends Error {}
来源：http://whu.aizwys.cn

TS:   class MyError extends Error {}
来源：http://ycr.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://upr.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lhv.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://tsf.yongpay.top

C#:   class MyException : Exception {}
来源：http://hty.zhongyouzk.top

[H05] 捕获特定类型
来源：http://dha.yongpay.top

Py:   except ValueError as e:
来源：http://txa.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sqg.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://qld.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://has.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://ser.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xzm.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://ilw.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yxu.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://uqc.fzhhl.top

Py:   value = d.get("k") or default
来源：http://nmz.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hbn.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tou.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://yrk.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://whg.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://gnp.xuetiantiany.cn

Ruby: d&.dig(:a, :b)
来源：http://mws.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://laz.fktsv.cn

[H07] 断言
来源：http://btg.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://amo.tarul.cn

PHP:  assert($x > 0);
来源：http://mkm.cheryme.top

JS:   console.assert(x > 0);
来源：http://wvv.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://zem.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://vdu.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pyh.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://diq.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://onv.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://pgg.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://uyd.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://olu.ydzc1.top

JS:   e.message;  e.stack
来源：http://puu.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mgj.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xrg.ydjk.org.cn

Go:   err.Error()
来源：http://rgf.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://skv.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://ruv.tian-w.cn

[H09] 带错误码的异常
来源：http://agr.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nqn.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xdo.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ryw.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uhx.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zjt.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aud.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://mge.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eli.dianchejie.cn

[H10] 资源自动释放
来源：http://lkn.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eve.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qyf.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://boc.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vbe.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fiu.cheryme.top

Go:   defer f.Close()
来源：http://fel.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kgq.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uxm.cqqwz.cn

================================================================================
来源：http://mik.snrcjt.cn

I. 正则表达式
来源：http://dlg.tanke756.top

================================================================================
来源：http://hdc.yuxming.cn

[I01] 判断是否匹配
来源：http://phy.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jvq.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uss.xinyue.icu

JS:   /\d+/.test(s)
来源：http://gbs.hesvh.cn

TS:   /\d+/.test(s)
来源：http://hyl.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rnt.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kja.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://uoa.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ztn.shuidangran.top

[I02] 提取所有匹配
来源：http://agj.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://mnc.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zts.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ycl.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://eak.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rpp.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eoc.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://ouf.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xjl.xziqi.cn

[I03] 提取捕获分组
来源：http://rzd.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://umj.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://njp.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nqn.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uya.shuidangran.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vvp.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://frc.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yks.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gmd.hywenlv.cn

[I04] 正则替换
来源：http://ixf.shuidangran.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fwz.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vzi.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://ovn.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://umq.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://oge.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qxa.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mzw.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pxt.ivvv.top

[I05] 按正则拆分
来源：http://ypr.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bcq.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oit.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://urq.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://mix.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://bxq.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wnt.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://aoz.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ujo.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tkq.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iib.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://djf.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ucw.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxy.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uht.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cnx.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhm.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qht.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://kud.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cae.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ifh.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bbm.yj20258.top

TS:   /error/gim
来源：http://ryk.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dph.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cpd.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://ouh.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://msr.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://xxw.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kcv.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bkn.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xky.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ftp.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ohr.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ces.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fxc.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ztb.snrcjt.cn

================================================================================
来源：http://rms.uphjek.com

J. 日期与时间
来源：http://fwp.feifeiyinyue.top

================================================================================
来源：http://dcv.ydzc1.top

[J01] 获取当前时间
来源：http://fry.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qtg.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://itc.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://ljw.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://pvu.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pfa.hnxiangtu.top

Go:   time.Now()
来源：http://qtq.chenzaomai.com

Ruby: Time.now
来源：http://yvv.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lrj.snrcjt.cn

[J02] 格式化输出
来源：http://wwe.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pac.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mph.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ono.tian-w.cn

TS:   d.toISOString()
来源：http://mbs.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rzb.jyoumei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yky.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fhc.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hmr.zhengqikj.top

[J03] 字符串解析为日期
来源：http://tac.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ftt.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pog.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://fob.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://vwm.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://pxa.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ool.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://bje.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://boj.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://zyg.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tes.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kry.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hir.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zuw.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rch.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://omn.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vvc.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yly.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://cap.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://ezi.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qta.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dxt.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zqu.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://rhz.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zxb.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://qhn.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://vyl.c1oappe.top

[J06] 计算两时间之差
来源：http://zhg.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://qyc.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://pui.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fgn.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://soj.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eew.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://epq.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://okq.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://wrn.yanxiufei.cn

[J07] 比较两个日期
来源：http://uvq.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://jne.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cag.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://jsm.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://zsr.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mwc.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://egh.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://dhq.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://npa.ehwqpu.com

[J08] 提取年月日与星期
来源：http://lzg.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozq.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lhk.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dye.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zqv.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://svm.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://roq.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://biz.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bal.hammf.cn

[J09] 时区处理
来源：http://rbi.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cvb.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kfy.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ztd.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jho.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qnj.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://swr.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://xup.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yuw.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://hga.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qam.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wae.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wby.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pxt.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gax.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vzx.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qhp.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xfh.daxiang520.top

================================================================================
来源：http://ufl.sweek.top

K. JSON 与序列化
来源：http://wcw.fktsv.cn

================================================================================
来源：http://rrb.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://ylx.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ryh.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ryp.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://kmq.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://fxz.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lnt.jianghu66.top

Go:   json.Marshal(obj)
来源：http://uqa.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://qxa.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ens.cheryme.top

[K02] JSON 字符串转对象
来源：http://kym.gaohongyu789.top

Py:   json.loads(s)
来源：http://rsk.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ezf.sxryk.cn

JS:   JSON.parse(s)
来源：http://obl.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://yrs.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lbk.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://wrp.yuxming.cn

Ruby: JSON.parse(s)
来源：http://gnn.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://apr.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://vla.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tmm.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ozs.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xxj.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ezr.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pqv.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lbl.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://xqh.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jre.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://lcd.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wtr.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vuo.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bof.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xqd.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cbu.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ufx.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dsx.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gni.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://tft.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://wvq.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://zqv.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://wku.birdmap.top

TS:   structuredClone(obj)
来源：http://ekq.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://twx.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qxy.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sgk.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://dtu.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://abe.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ptl.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cqg.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gbi.mhx1999.top


<!-- 参考信息 -->