代发 wailian999

[H03] 主动抛出异常
来源：http://mox.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://oyw.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bsj.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://nlg.cashguo.top

TS:   throw new Error("错误信息");
来源：http://ovd.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tog.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zlc.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iqo.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://usq.ivvv.top

[H04] 自定义异常类型
来源：http://oat.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://uyc.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pnm.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://tex.yongpay.top

TS:   class MyError extends Error {}
来源：http://jzq.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://urr.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ixp.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://ozb.xziqi.cn

C#:   class MyException : Exception {}
来源：http://esn.hcnkem.com

[H05] 捕获特定类型
来源：http://mrd.fehbvm.com

Py:   except ValueError as e:
来源：http://tly.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cbl.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://ylv.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://ikc.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://hyw.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nnv.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://yca.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blx.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://gxu.yueranfly.top

Py:   value = d.get("k") or default
来源：http://pnn.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jws.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://edr.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uhr.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://znm.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tgd.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://zxn.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://syq.yonumen.top

[H07] 断言
来源：http://mov.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://gmf.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://cwx.havefunace.top

JS:   console.assert(x > 0);
来源：http://euj.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://qwy.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://fbg.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qqp.vqdsnc.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ked.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://gxx.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://hxl.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://pee.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://msg.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://qgm.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://erm.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wpx.smart0.xyz

Go:   err.Error()
来源：http://jyg.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://veu.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://vvw.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://efm.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fst.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yzk.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yrm.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xie.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wkb.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ywv.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://fsy.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zaq.zhoulong.xyz

[H10] 资源自动释放
来源：http://cqu.haohaochexian.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aez.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rqq.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xbq.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eil.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rsk.vehdjk.com

Go:   defer f.Close()
来源：http://ydc.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mpr.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rhl.hnxiangtu.top

================================================================================
来源：http://ynd.wangdashe.top

I. 正则表达式
来源：http://ecn.uphjek.com

================================================================================
来源：http://ash.hammf.cn

[I01] 判断是否匹配
来源：http://jdr.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://akn.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://end.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://vct.bbcook.cn

TS:   /\d+/.test(s)
来源：http://kur.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rbf.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hgj.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://utb.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://slp.haohaochexian.top

[I02] 提取所有匹配
来源：http://tpi.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://tgl.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aul.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aui.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://you.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tnj.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cmz.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://czi.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cxi.hnxiangtu.top

[I03] 提取捕获分组
来源：http://rtn.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fwm.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qug.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bqv.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xbh.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wjn.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qkx.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jtk.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uak.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://sdy.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hys.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pat.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nlg.shuidangran.top

TS:   s.replace(/\d+/g, "#")
来源：http://jsm.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://mto.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://erp.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://goz.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wtn.aibaodan.cn

[I05] 按正则拆分
来源：http://vfi.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pzs.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mhp.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://cbd.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://yxy.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://wwe.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ula.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zmb.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yiq.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zmo.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ldh.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bol.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://knf.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wmi.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://anc.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jew.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixk.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nti.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://ftg.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vjq.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yrj.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cyz.0kj1m.cn

TS:   /error/gim
来源：http://iga.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ono.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lwg.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://phi.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vid.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://tdx.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cnn.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://naf.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iof.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zov.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://yqc.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ore.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fff.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cno.0kj1m.cn

================================================================================
来源：http://jmr.kuanghao11.cn

J. 日期与时间
来源：http://sum.shanyushiyangkeji.top

================================================================================
来源：http://fpj.hfpthk.cn

[J01] 获取当前时间
来源：http://dhp.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nep.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iwb.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://slp.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://hpg.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lnk.sjlbkw.cn

Go:   time.Now()
来源：http://jwx.jinqigfzy.top

Ruby: Time.now
来源：http://xcm.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fsq.yangfankeji.com

[J02] 格式化输出
来源：http://xuv.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ilu.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kch.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qfy.bjfxy.top

TS:   d.toISOString()
来源：http://gys.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jhm.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xxj.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://soz.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://onm.316326.xyz

[J03] 字符串解析为日期
来源：http://zxz.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nrr.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lxp.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://jsj.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://qzz.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://lxp.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gbo.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://lub.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rym.yongpay.top

[J04] 时间戳与日期互转
来源：http://uvy.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ylo.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iis.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tue.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ceh.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xcf.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://brn.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fkv.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qbf.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://cuh.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://ghi.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://sjy.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rio.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uhk.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://vqg.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dwd.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://vts.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://hpp.ybcxt.top

[J06] 计算两时间之差
来源：http://egh.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://aeu.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://pzn.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wuj.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rmg.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://pzs.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://krn.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://gnk.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://unv.ybcxt.top

[J07] 比较两个日期
来源：http://zen.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://egq.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fyj.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uxr.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tge.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://stu.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kin.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://itb.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://wvz.ehwqpu.com

[J08] 提取年月日与星期
来源：http://ppp.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jgv.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://biw.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wvz.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ezu.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vgd.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cyi.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dqg.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qge.redwolf501.top

[J09] 时区处理
来源：http://pqn.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vic.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vva.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yze.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://efq.fktsv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ehh.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://svy.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dlh.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oeu.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://bcc.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://chy.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ykn.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lym.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bht.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ynu.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fgt.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wfp.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dxf.haohaochexian.top

================================================================================
来源：http://dsl.yuanzhike.top

K. JSON 与序列化
来源：http://zhi.52xcode.cn

================================================================================
来源：http://bts.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://wke.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xms.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qdi.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://ctp.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://bqx.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vtd.meibo888.top

Go:   json.Marshal(obj)
来源：http://wot.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xng.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mmv.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://izt.hesvh.cn

Py:   json.loads(s)
来源：http://lfw.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cwd.fengsongda.top

JS:   JSON.parse(s)
来源：http://xoq.yj20258888.top

TS:   JSON.parse(s)
来源：http://vkc.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kat.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://tof.sxryk.cn

Ruby: JSON.parse(s)
来源：http://uwi.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eta.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://bna.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uzw.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gge.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cvg.guowangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ldk.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yku.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kgv.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qbq.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eaw.sweek.top

[K04] 读取 JSON 文件
来源：http://rhb.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jay.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aqp.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mvx.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://adj.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tvm.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://svk.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://nma.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bsc.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://ztj.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://kxi.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://ypb.hammf.cn

JS:   structuredClone(obj)
来源：http://vrj.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://mbs.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ccz.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yri.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yun.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ktc.zhixingplan.top

[K06] 解析 URL 查询串
来源：http://lbd.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://puh.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ebd.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qvo.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fje.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pku.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://djx.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gts.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sqc.cucudq.cn

[K07] 进制转换
来源：http://cyv.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bjj.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://grh.feifeiyinyue.top


<!-- 参考信息 -->