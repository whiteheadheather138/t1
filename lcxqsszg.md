代发 wailian999

TS:   throw new Error("错误信息");
来源：http://gyn.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nem.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxv.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oqp.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jln.sxryk.cn

[H04] 自定义异常类型
来源：http://jre.havefunace.top

Py:   class MyError(Exception): pass
来源：http://xvx.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://jta.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://ktc.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://pad.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://crp.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tgb.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://njg.vehdjk.com

C#:   class MyException : Exception {}
来源：http://mub.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://mms.haohaochexian.top

Py:   except ValueError as e:
来源：http://xkj.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hsd.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://rjv.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://vfe.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://cis.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fsa.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://ogv.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tuz.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://ueq.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://wrs.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ekb.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qsy.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qcc.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oew.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ljs.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://rmz.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://rll.chenjidiqi.icu

[H07] 断言
来源：http://yzh.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://jff.pycfn.com

PHP:  assert($x > 0);
来源：http://ljz.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://blq.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://vcl.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://ohw.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ssd.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pck.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://xsl.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://lxg.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://env.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jjs.tanke756.top

JS:   e.message;  e.stack
来源：http://gyu.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qxl.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fgx.aibaodan.cn

Go:   err.Error()
来源：http://rbd.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://nua.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://ygl.hfpthk.cn

[H09] 带错误码的异常
来源：http://yow.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qcf.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ltg.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jjo.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tnq.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ztf.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qkb.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://qqj.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xti.hcnkem.com

[H10] 资源自动释放
来源：http://kcy.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hef.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hdw.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bja.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ofl.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mhz.yfazqb.com

Go:   defer f.Close()
来源：http://goj.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://auv.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://acx.fzhhl.top

================================================================================
来源：http://yoa.iojbl.cn

I. 正则表达式
来源：http://wyk.xuanzx.com

================================================================================
来源：http://qsl.zhengqikj.top

[I01] 判断是否匹配
来源：http://nsk.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yan.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://yjh.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://vtt.xuanzx.com

TS:   /\d+/.test(s)
来源：http://jza.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://puk.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wmo.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://mov.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bqw.tanke756.top

[I02] 提取所有匹配
来源：http://pjj.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://iua.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://scg.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jpz.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://osy.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gcs.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sjj.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://pzm.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://muy.yj202588.top

[I03] 提取捕获分组
来源：http://hsr.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qkf.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hjn.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://egv.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vbv.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qio.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lkh.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://erg.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://giu.hammf.cn

[I04] 正则替换
来源：http://zkn.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nkf.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rjo.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://loq.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zao.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://hsz.fktsv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zsl.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hrm.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://odi.nwbrower.top

[I05] 按正则拆分
来源：http://ylb.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ylh.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qai.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://ohp.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://nhq.shanyushiyangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://efz.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ppb.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://sfq.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://okq.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ihc.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pni.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hkq.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fuw.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://biq.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lli.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zgl.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hqy.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yvu.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://ldh.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://frl.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://flv.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://erk.daxiang520.top

TS:   /error/gim
来源：http://qgp.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://car.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nqe.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://jaf.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jii.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://klt.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rev.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pto.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iyd.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lkw.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gnr.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fts.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yoc.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nsq.gzhubu.top

================================================================================
来源：http://age.hesvh.cn

J. 日期与时间
来源：http://arr.haohaochexian.top

================================================================================
来源：http://aym.hnqzz.top

[J01] 获取当前时间
来源：http://jia.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://may.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gqx.daria6918.cn

JS:   new Date();  Date.now()
来源：http://yzy.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://rul.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ytt.andypj.xyz

Go:   time.Now()
来源：http://kjr.cdnleiting.top

Ruby: Time.now
来源：http://zsj.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kep.fehbvm.com

[J02] 格式化输出
来源：http://eyb.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txq.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rbd.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sne.tarul.cn

TS:   d.toISOString()
来源：http://xpf.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://krf.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kfy.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://obq.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ofi.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://kot.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gpe.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zwr.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://lgy.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://sfk.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ggt.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://stk.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://lkj.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hzi.xinyue.icu

[J04] 时间戳与日期互转
来源：http://ksk.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://czc.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lwv.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kbm.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kvk.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eof.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gah.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pjv.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lzu.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://ahf.yongpay.top

Py:   now + timedelta(days=7)
来源：http://fna.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://ext.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qyc.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kut.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://cpx.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zdf.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ysb.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ram.xuanzx.com

[J06] 计算两时间之差
来源：http://dar.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://wyl.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://txy.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zdn.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kii.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://ese.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://uza.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://qfw.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://wzl.gotoacloud.top

[J07] 比较两个日期
来源：http://obd.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://bbf.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qvv.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://qwp.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qpm.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qea.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://whg.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://pvb.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://eqx.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://whm.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pej.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://evv.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yep.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://idh.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yjc.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ars.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bpl.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ioj.cdnleiting.top

[J09] 时区处理
来源：http://qpg.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kfh.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://msm.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zim.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://upe.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lvi.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xgz.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zpy.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bvu.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://qwn.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dlu.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xeo.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rgx.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://igw.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://svw.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ieg.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kys.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uks.gaohongyu789.top

================================================================================
来源：http://ctx.yj20258888.top

K. JSON 与序列化
来源：http://kdx.tanke756.top

================================================================================
来源：http://zdp.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://ngw.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dku.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ztt.yonumen.top

JS:   JSON.stringify(obj)
来源：http://aps.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://llt.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qyn.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://qmq.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uhx.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vzk.guannengcc.top

[K02] JSON 字符串转对象
来源：http://waj.zhiwuduotai.top

Py:   json.loads(s)
来源：http://dzr.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pjq.fengsongda.top

JS:   JSON.parse(s)
来源：http://jon.cqqwz.cn

TS:   JSON.parse(s)
来源：http://wgj.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://irw.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://rtj.daxiang520.top

Ruby: JSON.parse(s)
来源：http://vwx.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lzs.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://bkn.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kzb.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hpk.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://gkx.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rcd.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nvd.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dri.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://khh.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gbe.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://wke.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://isa.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vmn.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oab.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oly.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pbg.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uwh.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nmt.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lny.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://cml.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://rle.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://xfy.yuanzhike.top

JS:   structuredClone(obj)
来源：http://bcd.cqqwz.cn

TS:   structuredClone(obj)
来源：http://zyx.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ezk.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cxm.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jrh.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zor.gzhubu.top

[K06] 解析 URL 查询串
来源：http://kbt.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yqs.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zod.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://plb.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jey.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tjn.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dyf.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gvy.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cme.andypj.xyz

[K07] 进制转换
来源：http://flr.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wnr.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ita.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrh.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://amq.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bjq.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ljh.tianlin.xyz


<!-- 参考信息 -->