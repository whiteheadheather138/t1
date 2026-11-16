代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://rdd.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://asm.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ynt.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://phu.xinyue.icu

[H03] 主动抛出异常
来源：http://eey.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://kin.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://coa.yj202588.top

JS:   throw new Error("错误信息");
来源：http://icf.yongpay.top

TS:   throw new Error("错误信息");
来源：http://olq.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gmy.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uzi.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://atc.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lyx.tian-w.cn

[H04] 自定义异常类型
来源：http://rlt.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://ufi.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://lve.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://ajl.tarul.cn

TS:   class MyError extends Error {}
来源：http://ghl.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://uoj.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://alt.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://pkp.mhx1999.top

C#:   class MyException : Exception {}
来源：http://lmy.fzhhl.top

[H05] 捕获特定类型
来源：http://uow.xylfe.cn

Py:   except ValueError as e:
来源：http://yxu.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rem.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://ybh.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://kis.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://hbv.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mgm.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://xcb.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xbe.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://bpl.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://sbx.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://yqa.nanxuanxn.top

JS:   obj?.a?.b;  d ?? default
来源：http://qre.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://hac.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sdl.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gzo.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://scx.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://lzo.sufxvd.cn

[H07] 断言
来源：http://zvh.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://buy.cashguo.top

PHP:  assert($x > 0);
来源：http://vmb.xziqi.cn

JS:   console.assert(x > 0);
来源：http://spe.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://mln.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://ecd.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xkp.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://rxb.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://qnw.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://skn.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://sso.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qvo.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://iaq.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ltm.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://tum.fehbvm.com

Go:   err.Error()
来源：http://kgd.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://tyn.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://wmm.smart0.xyz

[H09] 带错误码的异常
来源：http://ier.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ynk.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ldi.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qfz.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nnm.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qbb.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://frv.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://qen.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ewu.shangyingyoupin.top

[H10] 资源自动释放
来源：http://uio.haohaochexian.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ypt.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xhu.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rtl.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ary.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tfx.tian-w.cn

Go:   defer f.Close()
来源：http://wxn.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://exg.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mdl.guannengcc.top

================================================================================
来源：http://xgc.ppjwa.cn

I. 正则表达式
来源：http://ytl.meibo888.top

================================================================================
来源：http://rxe.hnqzz.top

[I01] 判断是否匹配
来源：http://gsv.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://smz.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://ejw.cheryme.top

JS:   /\d+/.test(s)
来源：http://syl.52xcode.cn

TS:   /\d+/.test(s)
来源：http://jyg.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pfu.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xuh.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://kcg.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vic.zhengqikj.top

[I02] 提取所有匹配
来源：http://nms.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://yic.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://amk.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ysv.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://gau.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yak.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hgb.sweek.top

Ruby: s.scan(/\d+/)
来源：http://fem.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pog.nanxuanxn.top

[I03] 提取捕获分组
来源：http://iwu.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lgc.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pla.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rct.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cxu.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kan.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bog.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ugm.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hey.yuanzhike.top

[I04] 正则替换
来源：http://wtw.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://peq.sjlbkw.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ekf.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hdp.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://dkf.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kcp.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wvc.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://idi.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://apo.zdbjq.cn

[I05] 按正则拆分
来源：http://dwv.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wsv.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ovi.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://kwq.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://hsp.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://pvx.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yhe.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://peq.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bhz.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ixz.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vld.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sfb.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gnt.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ydi.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://scw.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xou.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jev.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bzn.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://gqa.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cvv.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://loo.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oze.guannengcc.top

TS:   /error/gim
来源：http://fwy.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qee.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ifj.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://svi.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://doc.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://ipk.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tiq.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kqt.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ptz.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://muq.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ukl.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iih.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://voz.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://okt.jqgfzy.top

================================================================================
来源：http://ubq.havefunace.top

J. 日期与时间
来源：http://bej.shuidangran.top

================================================================================
来源：http://gdd.c1oappe.top

[J01] 获取当前时间
来源：http://ehx.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ajz.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ycq.gaohongyu789.top

JS:   new Date();  Date.now()
来源：http://ehi.xuanzx.com

TS:   new Date();  Date.now()
来源：http://avs.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fhd.jqgfzy.top

Go:   time.Now()
来源：http://jfz.ydzc1.top

Ruby: Time.now
来源：http://hjy.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bwd.gotoacloud.top

[J02] 格式化输出
来源：http://enn.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vod.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://edq.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tiw.jianghu66.top

TS:   d.toISOString()
来源：http://anj.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nqz.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xwu.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqt.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hdv.zdqjudy.top

[J03] 字符串解析为日期
来源：http://eda.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xpr.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://htz.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://png.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://lrh.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://vih.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rcz.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://jse.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vyp.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://uev.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://soz.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://txo.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pfi.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://znz.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vdo.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wgd.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tpn.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mdh.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://vxz.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://oix.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dhm.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhl.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://agk.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://bmw.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hco.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://maj.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pqi.xuanzx.com

[J06] 计算两时间之差
来源：http://yuy.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://pnj.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://jrf.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kgb.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://twd.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://gkp.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://vkp.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://jpa.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://vcy.chenlongwang.top

[J07] 比较两个日期
来源：http://hnj.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://iah.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jzx.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://ejj.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://njd.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rpq.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://izm.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ogk.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://jzn.shuidangran.top

[J08] 提取年月日与星期
来源：http://tqq.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jyf.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hon.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ejg.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gjh.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pxw.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pcm.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mlw.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jwa.cashguo.top

[J09] 时区处理
来源：http://qcg.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zbj.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qrs.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cjk.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hlu.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mpa.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://elk.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://nbe.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://snv.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://qqh.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yxv.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tpc.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ipe.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rfd.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egb.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jjz.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tjo.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://buk.chenlongwang.top

================================================================================
来源：http://gwk.haohaochexian.top

K. JSON 与序列化
来源：http://ffx.jiagoushi.top

================================================================================
来源：http://yvw.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://vfc.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hxw.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://olh.ivvv.top

JS:   JSON.stringify(obj)
来源：http://qaa.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://zzl.bjfxy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://txs.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://saq.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://xld.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://icm.havefunace.top

[K02] JSON 字符串转对象
来源：http://rzo.sufxvd.cn

Py:   json.loads(s)
来源：http://tdj.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://asi.nanxinkj.top

JS:   JSON.parse(s)
来源：http://fnz.ehwqpu.com

TS:   JSON.parse(s)
来源：http://avl.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zvt.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://wep.wangdashe.top

Ruby: JSON.parse(s)
来源：http://dap.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xor.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://tni.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vye.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kds.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wee.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fzn.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xzj.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kte.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://xpx.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yqg.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://bui.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bgj.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fpp.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ufs.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lyi.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jio.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pry.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://niw.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://emo.jinqigufen.top

[K05] 深拷贝对象
来源：http://fgl.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://xhv.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://dgb.fktsv.cn

JS:   structuredClone(obj)
来源：http://jhn.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://qoq.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://phq.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://htt.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://glz.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gpg.zycfv.cn

[K06] 解析 URL 查询串
来源：http://jwh.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://niq.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://guq.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zrg.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kuv.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jdh.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://dex.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://raz.yangfankeji.com


<!-- 参考信息 -->