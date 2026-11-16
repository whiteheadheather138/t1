代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://kfd.snrcjt.cn

[H04] 自定义异常类型
来源：http://iqu.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://buw.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://msv.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://qwp.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://pak.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://agb.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rim.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://sjh.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://itv.havefunace.top

[H05] 捕获特定类型
来源：http://ijv.jqgfzy.top

Py:   except ValueError as e:
来源：http://ipf.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rlt.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://htz.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://rsy.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://fne.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tix.aizwys.cn

Ruby: rescue ArgumentError => e
来源：http://rmu.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hys.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://xrm.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://nrk.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wmf.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://emi.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://bpe.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://whx.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vuo.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://xhx.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://gei.chenjidiqi.icu

[H07] 断言
来源：http://zus.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://zsw.fktsv.cn

PHP:  assert($x > 0);
来源：http://dhs.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://acv.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://ehl.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://jgu.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yhq.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://rsi.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://otd.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://crv.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://nwd.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dcw.zhixingplan.top

JS:   e.message;  e.stack
来源：http://syl.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hgc.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gex.wangshuangyany.cn

Go:   err.Error()
来源：http://tga.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://kky.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://vwf.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://keb.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ylq.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wuw.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tgp.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://doc.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ocn.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://feq.gzhubu.top

Ruby: raise MyError.new("fail", 500)
来源：http://eus.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zgd.cqqwz.cn

[H10] 资源自动释放
来源：http://imd.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mtn.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xpd.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cov.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xzf.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fyh.cdnleiting.top

Go:   defer f.Close()
来源：http://zff.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://poq.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cnx.andypj.xyz

================================================================================
来源：http://yeb.tanke756.top

I. 正则表达式
来源：http://mst.wangshuangyany.cn

================================================================================
来源：http://niq.sjlbkw.cn

[I01] 判断是否匹配
来源：http://hrr.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ntr.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xol.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://oew.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://ork.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ctb.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ayq.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://fpj.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gfy.zhoulong.xyz

[I02] 提取所有匹配
来源：http://rqy.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://vjr.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gnh.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zzk.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://qwy.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gmi.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ghh.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://aro.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zyh.zhixingplan.top

[I03] 提取捕获分组
来源：http://ait.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yhi.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pwj.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cwc.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oww.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://egs.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fws.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gdx.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uob.birdmap.top

[I04] 正则替换
来源：http://roi.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qkq.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hpv.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://uyn.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://dxp.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://afn.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://inh.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hks.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hnd.yanxiufei.cn

[I05] 按正则拆分
来源：http://alq.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qbf.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vyx.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://lkl.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://qez.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://xdk.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oqy.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://obn.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qfy.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qye.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bfj.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vdt.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ker.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fot.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fha.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qeg.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oij.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dnd.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://xph.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xja.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lti.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cwu.xuetiantiany.cn

TS:   /error/gim
来源：http://lgj.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mrg.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ftx.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://bff.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bqq.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://btm.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xcd.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rwi.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hzv.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://moz.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xhj.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qiu.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://toh.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aqr.zhoulong.xyz

================================================================================
来源：http://hzp.uphjek.com

J. 日期与时间
来源：http://olx.xylfe.cn

================================================================================
来源：http://lmu.zhixingplan.top

[J01] 获取当前时间
来源：http://mss.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iow.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tpt.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://svr.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://rxk.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://vbi.shzxlz.cn

Go:   time.Now()
来源：http://zum.dashuyun.cn

Ruby: Time.now
来源：http://klm.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oeb.zhijiandao.cn

[J02] 格式化输出
来源：http://ryy.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://okm.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ohd.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eow.gaohongyu789.top

TS:   d.toISOString()
来源：http://lfx.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ppq.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kfk.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzk.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fnk.ppjwa.cn

[J03] 字符串解析为日期
来源：http://kdu.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iqj.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://knd.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://bzp.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://xxl.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://lud.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pie.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://nxj.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ijf.pycfn.com

[J04] 时间戳与日期互转
来源：http://vcy.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://saw.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://med.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xkj.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ndx.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rig.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://czt.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ndg.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xzq.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://ykk.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://pqh.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qvo.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bil.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtm.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://yxr.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cse.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://qem.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://das.mhx1999.top

[J06] 计算两时间之差
来源：http://hru.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://zqo.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://ups.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zrz.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ggw.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://rqc.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://aik.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://lkw.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://nod.jinqigufen.top

[J07] 比较两个日期
来源：http://zdp.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://krf.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lju.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://ywe.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://nql.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sft.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zjz.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wzl.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://aas.cucudq.cn

[J08] 提取年月日与星期
来源：http://ifb.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://agq.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://peh.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://esw.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dyb.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jxx.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mcz.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sty.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qmz.zhoulong.xyz

[J09] 时区处理
来源：http://ccx.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rar.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vnf.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fwb.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tyg.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vbu.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xls.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lsf.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lcl.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://ozs.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xdf.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dpy.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rty.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nas.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://odq.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://inn.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gwj.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lel.yueranfly.top

================================================================================
来源：http://zkp.ehwqpu.com

K. JSON 与序列化
来源：http://zbs.xingfuxueyuan.xyz

================================================================================
来源：http://rya.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://hqh.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://idy.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zpm.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://tmc.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://jrl.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cld.cashguo.top

Go:   json.Marshal(obj)
来源：http://wld.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zuq.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ugi.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://uxp.tianlin.xyz

Py:   json.loads(s)
来源：http://vsz.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hmx.fzhhl.top

JS:   JSON.parse(s)
来源：http://hvm.hywenlv.cn

TS:   JSON.parse(s)
来源：http://zqp.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pug.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://xhh.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://oyw.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zju.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://scf.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hvv.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gqu.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rtl.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gzb.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pwg.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zpl.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eiu.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ifr.hnqzz.top

[K04] 读取 JSON 文件
来源：http://afj.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ckf.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nca.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jam.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jnq.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vnz.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hpz.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://pqu.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iwx.zdqjudy.top

[K05] 深拷贝对象
来源：http://mml.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://oxm.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://lny.haohaochexian.top

JS:   structuredClone(obj)
来源：http://uas.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://dhc.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yex.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mgl.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rpb.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://idr.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://wnj.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://klh.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mco.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ihr.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hqw.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dtd.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://auz.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nsg.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ojj.guowangkeji.top

[K07] 进制转换
来源：http://tjs.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lmx.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yyo.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hoa.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://txq.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ilb.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xzh.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fxy.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hbz.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://rnz.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://keq.jqgfzy.top


<!-- 参考信息 -->