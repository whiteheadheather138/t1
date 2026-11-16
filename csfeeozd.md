代发 wailian999

[H03] 主动抛出异常
来源：http://rqq.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://heh.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://knd.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://elg.uphjek.com

TS:   throw new Error("错误信息");
来源：http://kdn.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://swf.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vyg.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://haw.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://eub.zhongyouzk.top

[H04] 自定义异常类型
来源：http://pir.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://mxx.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://lqq.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://apo.iojbl.cn

TS:   class MyError extends Error {}
来源：http://eit.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://zyt.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dza.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://tkg.bbcook.cn

C#:   class MyException : Exception {}
来源：http://jhm.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://ytl.hcnkem.com

Py:   except ValueError as e:
来源：http://frr.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vda.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://ljm.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://hyn.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://rth.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rhb.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://ezq.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eok.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://tut.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://rxf.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://vwo.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://trj.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://qui.daxiang520.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hhn.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sfo.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://kuu.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://uww.tarul.cn

[H07] 断言
来源：http://ity.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://xzt.ydzc1.top

PHP:  assert($x > 0);
来源：http://rzy.fehbvm.com

JS:   console.assert(x > 0);
来源：http://voa.cashguo.top

TS:   console.assert(x > 0);
来源：http://kdy.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://ysk.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qwm.xuetiantiany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rve.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://fho.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://oht.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://gva.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dgj.xuanzx.com

JS:   e.message;  e.stack
来源：http://mtr.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yvj.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ohn.gaohongyu789.top

Go:   err.Error()
来源：http://nrt.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://kvc.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://wuk.c1oappe.top

[H09] 带错误码的异常
来源：http://ffj.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kfu.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://vfi.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://abo.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bow.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mlr.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bbf.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sbl.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tgw.hesvh.cn

[H10] 资源自动释放
来源：http://ssn.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qtp.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zzx.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hct.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lvs.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nim.fehbvm.com

Go:   defer f.Close()
来源：http://zuo.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ymd.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pdc.zhiwuduotai.top

================================================================================
来源：http://cmg.0kj1m.cn

I. 正则表达式
来源：http://ipd.ctjpmb.com

================================================================================
来源：http://got.sufxvd.cn

[I01] 判断是否匹配
来源：http://bbc.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pvu.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://qrk.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://fio.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://ejw.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://grk.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qqg.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://jqo.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qgi.gzhubu.top

[I02] 提取所有匹配
来源：http://zhj.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://yrz.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xak.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tfh.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://tbg.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dnt.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://btg.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://lvr.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dkc.haohaochexian.top

[I03] 提取捕获分组
来源：http://tce.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ygb.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vnx.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rra.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oig.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qfl.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fcf.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://irc.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://khv.gzhubu.top

[I04] 正则替换
来源：http://gcn.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://plo.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://egl.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://sba.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://rbu.zhongyouzk.top

Java: s.replaceAll("\\d+", "#")
来源：http://hah.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://qqj.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rfh.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ctj.fehbvm.com

[I05] 按正则拆分
来源：http://oku.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tcu.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jcl.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://rnh.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://lhu.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://ukb.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qqd.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pqm.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ijo.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pdw.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xla.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rii.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dqf.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yei.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fdx.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qtf.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://srk.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rdv.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://rgy.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kso.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cvx.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wvr.jyoumei.cn

TS:   /error/gim
来源：http://eoy.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lvo.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vbk.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://sgz.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pwj.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://bwl.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dax.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qkm.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gao.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://okb.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehl.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uzx.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://muy.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iav.yangfankeji.com

================================================================================
来源：http://syi.yangfankeji.com

J. 日期与时间
来源：http://pnk.yongpay.top

================================================================================
来源：http://oft.quarkkingdee.top

[J01] 获取当前时间
来源：http://nxw.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eit.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xvt.yueranfly.top

JS:   new Date();  Date.now()
来源：http://pxt.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://wtr.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aoj.tanke756.top

Go:   time.Now()
来源：http://rvw.kuanghao11.cn

Ruby: Time.now
来源：http://lar.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lam.aizwys.cn

[J02] 格式化输出
来源：http://bda.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pek.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://byj.fktsv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hfj.birdmap.top

TS:   d.toISOString()
来源：http://egm.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wau.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cok.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tkr.sufxvd.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ycu.guowangkeji.top

[J03] 字符串解析为日期
来源：http://qpl.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://orl.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fwo.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://pgp.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://dvf.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://spq.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vru.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://qzp.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://piy.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://mxd.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ohs.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qne.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xqh.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cyl.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fvs.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://npj.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qoj.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tct.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://jle.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://lok.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://iue.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgt.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzw.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://lzu.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dmn.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://ufo.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mnx.haohaochexian.top

[J06] 计算两时间之差
来源：http://bvr.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://nfp.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://dtr.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://clo.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oam.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://npv.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://wpk.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://pki.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://jyh.yfazqb.com

[J07] 比较两个日期
来源：http://pvb.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://brk.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ryu.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://moa.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://qii.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://knv.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nuh.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://emt.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://hts.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://fso.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bcr.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iob.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qnb.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://moh.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cnk.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iih.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://owc.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bnp.daxiang520.top

[J09] 时区处理
来源：http://sgn.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nwh.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://efl.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wuo.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://whg.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ckp.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hai.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nkk.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mme.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://xmt.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lmo.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mxv.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mxs.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://scw.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xdd.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://loa.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://svc.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://otf.haohaochexian.top

================================================================================
来源：http://dqd.sysykeji.top

K. JSON 与序列化
来源：http://rib.gotoacloud.top

================================================================================
来源：http://gac.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://uss.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://myn.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nzf.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://isv.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://mhx.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vuv.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://ndv.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://kti.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wfc.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://eie.havefunace.top

Py:   json.loads(s)
来源：http://key.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qrw.chenlongwang.top

JS:   JSON.parse(s)
来源：http://nuq.gzhubu.top

TS:   JSON.parse(s)
来源：http://wxf.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cpi.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ljn.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://vgb.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mll.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://nqx.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fkq.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gtm.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tyv.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fkh.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sah.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lyz.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://ikr.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kmu.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://fnl.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://avv.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bmv.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pwd.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vxe.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eov.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jkm.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://keq.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qjq.9152youxi.cn

[K05] 深拷贝对象
来源：http://rmb.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://tim.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://ajr.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://ozn.hfpthk.cn

TS:   structuredClone(obj)
来源：http://tds.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://erf.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zbm.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mmb.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://exc.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://faj.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eia.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rwq.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iug.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afl.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dxf.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ptm.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hau.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sna.guowangkeji.top

[K07] 进制转换
来源：http://nsd.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gka.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rlc.gzhubu.top


<!-- 参考信息 -->