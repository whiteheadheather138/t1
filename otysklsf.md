代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://nhz.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://jlq.uphjek.com

Py:   class MyError(Exception): pass
来源：http://pkf.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://bty.xziqi.cn

JS:   class MyError extends Error {}
来源：http://rld.tarul.cn

TS:   class MyError extends Error {}
来源：http://csg.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://vye.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wvc.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://uxf.gzhubu.top

C#:   class MyException : Exception {}
来源：http://jbd.gzhubu.top

[H05] 捕获特定类型
来源：http://qvt.hammf.cn

Py:   except ValueError as e:
来源：http://suo.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xyl.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://gzz.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://uqs.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://zob.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pul.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://lgj.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gug.yongpay.top

[H06] 可选值 / 空值安全访问
来源：http://bye.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://khj.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dwt.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://rqf.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://tiv.aizwys.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lmk.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pzj.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://pln.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://ael.epnwcf.com

[H07] 断言
来源：http://cfg.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://cmo.yfazqb.com

PHP:  assert($x > 0);
来源：http://pcs.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://uxy.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://xlq.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://bdi.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nfp.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://gtn.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://sfg.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://jla.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://rib.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mrx.yuxming.cn

JS:   e.message;  e.stack
来源：http://qkp.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jxk.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vrf.chenzaomai.com

Go:   err.Error()
来源：http://yqa.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://ihn.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://snt.hysaishi.cn

[H09] 带错误码的异常
来源：http://lyp.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://okz.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ipc.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rin.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wba.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://slv.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bwc.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://eku.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hkc.guannengcc.top

[H10] 资源自动释放
来源：http://bfb.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jqv.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uxe.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://asd.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mef.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dmh.yvedp.cn

Go:   defer f.Close()
来源：http://zrp.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://snz.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nyu.ehwqpu.com

================================================================================
来源：http://hwp.nwbrower.top

I. 正则表达式
来源：http://lzg.yongpay.top

================================================================================
来源：http://dgy.jqgufenzy.top

[I01] 判断是否匹配
来源：http://mfv.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bmn.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://lcj.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://hei.aizwys.cn

TS:   /\d+/.test(s)
来源：http://ehx.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fcf.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kkw.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://ygx.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gas.ybcxt.top

[I02] 提取所有匹配
来源：http://gnx.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://vwd.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cfg.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yec.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://ctu.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://alz.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ouk.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://pew.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aqg.yuanzhike.top

[I03] 提取捕获分组
来源：http://zbd.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qhd.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ebo.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lkr.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vnq.shanyushiyangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://miv.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rnf.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://med.zhongyouzk.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qgu.yvedp.cn

[I04] 正则替换
来源：http://hfb.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://myq.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cwr.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kko.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mud.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fji.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ouu.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ees.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cnq.chenzaomai.com

[I05] 按正则拆分
来源：http://oni.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wur.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bjb.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://llv.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://cly.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://wkj.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qne.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://plw.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jal.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fgk.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ivc.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://suh.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://exz.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://skl.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sep.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cfg.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qxl.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kku.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://suy.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://imu.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fqz.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://poj.vqdsnc.cn

TS:   /error/gim
来源：http://zjh.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bxg.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zcw.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://yur.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tcf.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://efj.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gpr.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://umo.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sqf.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tno.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yhu.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://klc.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ixg.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blu.yongpay.top

================================================================================
来源：http://npj.yonumen.top

J. 日期与时间
来源：http://cjc.cqqwz.cn

================================================================================
来源：http://vsf.ctjpmb.com

[J01] 获取当前时间
来源：http://jga.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://bqm.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://khm.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://zrd.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://nro.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nyf.nanxuanxn.top

Go:   time.Now()
来源：http://dkz.pycfn.com

Ruby: Time.now
来源：http://zfr.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lqj.fehbvm.com

[J02] 格式化输出
来源：http://gcl.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://abl.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://faf.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nwg.yuanzhike.top

TS:   d.toISOString()
来源：http://smm.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xic.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tin.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rez.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uiw.dianchejie.cn

[J03] 字符串解析为日期
来源：http://xbz.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://etf.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://atg.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://loi.ivvv.top

TS:   new Date("2024-01-02")
来源：http://xlk.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://awn.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ssv.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://eka.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cou.daxiang520.top

[J04] 时间戳与日期互转
来源：http://qkh.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hyz.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gal.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hcc.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://svp.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cfy.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://haw.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qmc.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dtg.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://cof.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://pqf.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://whl.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hyx.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lba.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://hnk.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lhm.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://swx.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://wgm.sjlbkw.cn

[J06] 计算两时间之差
来源：http://stc.meibo888.top

Py:   (end - start).total_seconds()
来源：http://ypm.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://wcv.gzhubu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xiz.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pfc.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gcx.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://hpk.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://twc.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://pgp.yj20258888.top

[J07] 比较两个日期
来源：http://sir.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://ajo.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bka.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ghq.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://qur.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pnr.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rea.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sxc.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://iyo.0kj1m.cn

[J08] 提取年月日与星期
来源：http://euk.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://msu.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lpi.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zqb.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vlb.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oqn.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kay.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vrq.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oda.jyoumei.cn

[J09] 时区处理
来源：http://hhl.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cuw.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://txu.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lzb.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pxd.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lch.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rjr.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nfs.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dsz.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://uen.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mjv.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kei.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://enc.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ike.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gpb.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ozg.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ytq.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://icm.sjlbkw.cn

================================================================================
来源：http://oci.guowangkeji.top

K. JSON 与序列化
来源：http://dbm.ctjpmb.com

================================================================================
来源：http://sjh.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://xni.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dgn.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wqa.yonumen.top

JS:   JSON.stringify(obj)
来源：http://fqm.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://fcf.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xsx.fktsv.cn

Go:   json.Marshal(obj)
来源：http://zlt.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://ljn.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rwh.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://bly.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://iyy.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://twi.bjfxy.top

JS:   JSON.parse(s)
来源：http://zdf.yuanzhike.top

TS:   JSON.parse(s)
来源：http://cnw.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pyn.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://wsl.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://rbx.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yvd.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://xhu.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jvy.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vyg.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hou.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wup.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pks.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ztc.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://jed.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xha.cheryme.top

[K04] 读取 JSON 文件
来源：http://xoy.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hnt.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jxt.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://brm.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kfp.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zrd.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dpj.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qkf.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zhs.sxryk.cn

[K05] 深拷贝对象
来源：http://jzm.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://stv.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://fgu.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://xxy.sysykeji.top

TS:   structuredClone(obj)
来源：http://uqf.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://mpz.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qlm.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vqm.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hzw.yj20258888.top

[K06] 解析 URL 查询串
来源：http://biw.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eoo.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iwb.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nrz.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzr.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gsi.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rqc.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ybf.pengpengdd.cyou

[K07] 进制转换
来源：http://vor.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ulm.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ezu.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ppq.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nhx.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://msj.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://izt.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sur.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wnc.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://eob.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://eqc.zhiwuduotai.top


<!-- 参考信息 -->