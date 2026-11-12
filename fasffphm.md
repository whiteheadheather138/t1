代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://fkv.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://umi.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gpc.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ghw.andypj.xyz

[H03] 主动抛出异常
来源：http://qhi.sweek.top

Py:   raise ValueError("错误信息")
来源：http://hrv.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bjb.sweek.top

JS:   throw new Error("错误信息");
来源：http://bjz.pycfn.com

TS:   throw new Error("错误信息");
来源：http://pzc.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zwx.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bbe.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gtt.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vmm.chenlongwang.top

[H04] 自定义异常类型
来源：http://apd.birdmap.top

Py:   class MyError(Exception): pass
来源：http://hte.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://gga.ybcxt.top

JS:   class MyError extends Error {}
来源：http://odw.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://rli.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://pwy.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://alq.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://mee.iojbl.cn

C#:   class MyException : Exception {}
来源：http://dxp.ydjk.org.cn

[H05] 捕获特定类型
来源：http://gae.kuanghao11.cn

Py:   except ValueError as e:
来源：http://rao.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nbn.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://ink.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://exb.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://otv.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pgd.cashguo.top

Ruby: rescue ArgumentError => e
来源：http://vbt.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uvf.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://ofv.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://glw.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://zyv.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://blw.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://sds.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qja.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wkh.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://cdg.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://cdp.guowangkeji.top

[H07] 断言
来源：http://gpq.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://uot.yj20258.top

PHP:  assert($x > 0);
来源：http://jgo.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://xmy.bbcook.cn

TS:   console.assert(x > 0);
来源：http://sdt.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://xso.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pvi.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qeu.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://xxc.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://blc.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://muw.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jhx.ppjwa.cn

JS:   e.message;  e.stack
来源：http://chm.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xie.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mxw.hywenlv.cn

Go:   err.Error()
来源：http://zwo.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://ifv.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://dok.jinqigfzy.top

[H09] 带错误码的异常
来源：http://hty.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tsa.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://buz.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cuk.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gok.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kdl.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ogc.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://zty.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://pwm.shangyingyoupin.top

[H10] 资源自动释放
来源：http://xic.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jfy.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bma.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ypt.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://txe.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hfe.yj20258.top

Go:   defer f.Close()
来源：http://nwq.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vra.jinyuanbaomall.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mad.haohaochexian.top

================================================================================
来源：http://pnl.hongshengwenyu.top

I. 正则表达式
来源：http://ifm.shuidangran.top

================================================================================
来源：http://wqx.fzhhl.top

[I01] 判断是否匹配
来源：http://two.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aky.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://sdl.fengsongda.top

JS:   /\d+/.test(s)
来源：http://tcr.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://kiz.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jsl.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lwj.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://raf.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://onv.zdbjq.cn

[I02] 提取所有匹配
来源：http://slu.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://okw.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gqc.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uqw.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://sqc.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gnw.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qnc.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://zjr.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lto.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://rsx.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oka.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://beo.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fsj.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jjc.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qgc.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tzd.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vhn.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ipv.wangshuangyany.cn

[I04] 正则替换
来源：http://efd.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hvx.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://obt.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://dbn.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://gjm.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://ttz.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rra.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://eke.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ekt.jinqigufen.top

[I05] 按正则拆分
来源：http://xei.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uay.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bgl.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://czd.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://odi.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://lvm.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rev.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://ilc.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sma.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xxq.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uyz.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cnm.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jkn.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://njl.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://udy.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mci.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bum.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bzd.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://zey.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tdp.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ypn.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iwm.kuanghao11.cn

TS:   /error/gim
来源：http://ywf.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qqr.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xht.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://gki.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aau.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://bcw.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aha.bjfxy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gsw.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://odg.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yna.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gqw.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ygz.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cae.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jcd.chenjidiqi.icu

================================================================================
来源：http://cld.xinyue.icu

J. 日期与时间
来源：http://spn.shanyushiyangkeji.top

================================================================================
来源：http://ktu.aibaodan.cn

[J01] 获取当前时间
来源：http://pgr.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mux.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dww.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://odm.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://pei.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eag.zhijiandao.cn

Go:   time.Now()
来源：http://znm.c1oappe.top

Ruby: Time.now
来源：http://wjs.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eae.chenlongwang.top

[J02] 格式化输出
来源：http://erl.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kwt.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hwp.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://osc.zdbjq.cn

TS:   d.toISOString()
来源：http://hxp.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://akh.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eid.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbc.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://esd.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://qog.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yjw.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://roq.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://xps.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://mbd.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://qhf.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://frg.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://bav.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xjd.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://kwh.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zit.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://foj.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ykt.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kpc.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://svp.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tbt.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xdw.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qwl.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://ulz.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://nup.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tyk.ppjwa.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ajd.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nkv.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://shj.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://azg.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://rhx.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://nap.tian-w.cn

[J06] 计算两时间之差
来源：http://qup.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://fkv.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://uyl.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://par.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wtv.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://sgl.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://avx.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://ecg.yuxming.cn

C#:   (end - start).TotalSeconds
来源：http://xkn.hcnkem.com

[J07] 比较两个日期
来源：http://frv.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://zna.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lsh.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://ipg.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bei.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pxm.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rxp.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xza.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://hzr.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://vba.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ywi.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eic.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vhf.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bem.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kzr.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ytt.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xyh.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tkt.0kj1m.cn

[J09] 时区处理
来源：http://yyh.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vgu.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yaq.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ocz.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://efj.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uoa.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rgg.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kla.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nay.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://uqm.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ctl.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://udi.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fuj.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rkj.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mjd.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pfs.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ngf.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pkt.xylfe.cn

================================================================================
来源：http://nok.yonumen.top

K. JSON 与序列化
来源：http://chc.svipenyu.cn

================================================================================
来源：http://wzt.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://iqb.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xbm.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uwc.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://vct.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://vkk.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hop.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://glp.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://xhq.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ryi.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://ahl.xuanzx.com

Py:   json.loads(s)
来源：http://gfn.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ryg.jqgfzy.top

JS:   JSON.parse(s)
来源：http://vrw.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://hfv.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bnl.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://tus.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://spu.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://evr.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://amr.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://usi.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://myc.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tzg.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dle.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://asr.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gqx.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://fdh.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qqv.52xcode.cn

[K04] 读取 JSON 文件
来源：http://ptp.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://avj.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cxt.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbt.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lwc.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nok.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sol.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kfi.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ymf.vehdjk.com

[K05] 深拷贝对象
来源：http://qpj.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://mfh.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://uny.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://gqw.vehdjk.com

TS:   structuredClone(obj)
来源：http://nny.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qxr.svipenyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pek.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://urp.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://obo.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://uiz.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zpg.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fxz.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vfj.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqc.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ncu.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vkx.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://myk.meibo888.top


<!-- 参考信息 -->