代发 wailian999

TS:   throw new Error("错误信息");
来源：http://gge.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uvu.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gay.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://drk.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://czx.sweek.top

[H04] 自定义异常类型
来源：http://fcj.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://ivw.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://cyg.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://eyn.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://ktg.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://bfo.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nai.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://hhc.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://gtq.aibaodan.cn

[H05] 捕获特定类型
来源：http://bbz.ydjk.org.cn

Py:   except ValueError as e:
来源：http://nwr.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xpf.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://jtx.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://ahk.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://jlq.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://acw.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://yal.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bmv.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://csi.gzhubu.top

Py:   value = d.get("k") or default
来源：http://scb.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://xka.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://qbo.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://jiu.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dut.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cek.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://iij.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://wkq.tian-w.cn

[H07] 断言
来源：http://eky.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://nus.tian-w.cn

PHP:  assert($x > 0);
来源：http://pmj.yj202588.top

JS:   console.assert(x > 0);
来源：http://nht.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://blt.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://jjq.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zeo.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pfa.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://rlp.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://lhz.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://nkj.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lcv.aizwys.cn

JS:   e.message;  e.stack
来源：http://nxh.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qqv.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jvs.chenlongwang.top

Go:   err.Error()
来源：http://nib.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://vza.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://zkz.tarul.cn

[H09] 带错误码的异常
来源：http://yqd.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mcs.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zdg.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jpd.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gvw.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tqe.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jug.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://gho.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rfv.sjlbkw.cn

[H10] 资源自动释放
来源：http://vco.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ysv.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lmn.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xgj.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qms.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gkt.cucudq.cn

Go:   defer f.Close()
来源：http://kap.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ukf.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zjb.snrcjt.cn

================================================================================
来源：http://ntx.guannengcc.top

I. 正则表达式
来源：http://kkn.cucudq.cn

================================================================================
来源：http://qbk.havefunace.top

[I01] 判断是否匹配
来源：http://eyf.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cjn.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nwj.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://vyo.wangdashe.top

TS:   /\d+/.test(s)
来源：http://yod.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rmw.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uuw.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://cxz.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nvy.shuidangran.top

[I02] 提取所有匹配
来源：http://lii.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://zda.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pvh.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://veg.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://jpq.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uuf.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bbz.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://irm.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wso.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://esu.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wpb.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yss.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ceg.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ahx.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vua.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://phg.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://euc.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://skq.ehwqpu.com

[I04] 正则替换
来源：http://acm.9152youxi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yoh.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xqi.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://tti.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://bia.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vfs.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vhy.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://etp.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nmo.birdmap.top

[I05] 按正则拆分
来源：http://oeg.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://crv.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blh.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://bdh.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://fbp.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://aix.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hhw.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://iwa.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lyn.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nia.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hqy.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vui.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bor.jqgufenzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghf.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rok.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ucw.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ime.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wzd.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://cps.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dbr.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qdc.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iyi.yueranfly.top

TS:   /error/gim
来源：http://ksk.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uxq.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://htg.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://pth.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzv.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://des.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gws.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iom.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvt.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gnk.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://acq.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://azs.sweek.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fyl.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://okk.nanxinkj.top

================================================================================
来源：http://uii.yuanzhike.top

J. 日期与时间
来源：http://gez.gotoacloud.top

================================================================================
来源：http://faq.jqgfzy.top

[J01] 获取当前时间
来源：http://sfe.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://xkv.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://unb.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://mgz.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://vtn.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ijl.yj202588.top

Go:   time.Now()
来源：http://ybh.ybcxt.top

Ruby: Time.now
来源：http://rnh.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fpy.jinqigufen.top

[J02] 格式化输出
来源：http://hhi.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bda.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://frm.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cjz.zhongyouzk.top

TS:   d.toISOString()
来源：http://ges.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oqq.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dri.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qfp.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kmg.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://jib.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyw.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zmn.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://kih.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://kea.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://szi.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uxj.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://mic.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bvs.sxryk.cn

[J04] 时间戳与日期互转
来源：http://mid.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sig.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ydp.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yoq.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fsw.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gjx.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mbd.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iza.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qmb.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://wll.uphjek.com

Py:   now + timedelta(days=7)
来源：http://fwo.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zmr.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ovc.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lvn.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://jkx.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ogw.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://uwz.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://dlg.jiagoushi.top

[J06] 计算两时间之差
来源：http://qhp.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://cha.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://zsu.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hvk.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kzf.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eow.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://fwf.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://esa.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://ohn.shuidangran.top

[J07] 比较两个日期
来源：http://lst.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://uuo.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dcn.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://vwb.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://jpp.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qts.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zqu.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://nap.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://nrw.ivvv.top

[J08] 提取年月日与星期
来源：http://xpt.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wrh.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ydv.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fja.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bsq.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zux.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ggk.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zev.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yos.xziqi.cn

[J09] 时区处理
来源：http://ogp.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://glp.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iqy.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uar.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qnl.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sec.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tar.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://vks.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dvj.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://vfx.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cvx.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://whp.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iqn.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nwf.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://swl.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vol.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cri.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://end.guannengcc.top

================================================================================
来源：http://irz.gaohongyu789.top

K. JSON 与序列化
来源：http://azk.ctjpmb.com

================================================================================
来源：http://zjk.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://gmv.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nld.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hka.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://abo.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://iny.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vhh.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://kxf.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://doa.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hmk.yuxming.cn

[K02] JSON 字符串转对象
来源：http://hlp.ybcxt.top

Py:   json.loads(s)
来源：http://yfe.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vhy.daria6918.cn

JS:   JSON.parse(s)
来源：http://jnb.hesvh.cn

TS:   JSON.parse(s)
来源：http://brm.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vuw.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://cvg.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://hyq.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hjk.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://khi.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aec.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://llg.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cbk.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yfz.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://afj.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ihp.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://ids.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bbg.cheryme.top

[K04] 读取 JSON 文件
来源：http://wyi.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wdr.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vil.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://adh.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://akx.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://orp.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qmz.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fjj.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yzv.aizwys.cn

[K05] 深拷贝对象
来源：http://nki.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://lwa.hammf.cn

PHP:  unserialize(serialize($obj));
来源：http://wln.aizwys.cn

JS:   structuredClone(obj)
来源：http://grw.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://uxe.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bbe.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dzu.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nkm.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mvo.meibo888.top

[K06] 解析 URL 查询串
来源：http://wwo.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kuv.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fcn.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sqq.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uei.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ocj.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://drb.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fjz.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bgt.hongshengwenyu.top

[K07] 进制转换
来源：http://mmi.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://efb.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tyj.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nnv.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://etc.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://obz.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ztu.pycfn.com


<!-- 参考信息 -->