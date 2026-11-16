代发 wailian999

TS:   throw new Error("错误信息");
来源：http://tzo.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://klg.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hcg.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ugn.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ifr.xziqi.cn

[H04] 自定义异常类型
来源：http://ixt.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://xrn.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://mwv.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://tgf.cashguo.top

TS:   class MyError extends Error {}
来源：http://eio.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://nml.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://too.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://vft.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://jnz.52xcode.cn

[H05] 捕获特定类型
来源：http://mxd.uphjek.com

Py:   except ValueError as e:
来源：http://dwx.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mrc.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://uhk.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://nzs.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://fhn.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uxf.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://szv.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qzz.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://rvw.52xcode.cn

Py:   value = d.get("k") or default
来源：http://djv.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://vjn.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://ppr.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://vin.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tdi.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xrb.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://niy.svipenyu.cn

C#:   obj?.A?.B ?? default
来源：http://map.vehdjk.com

[H07] 断言
来源：http://usy.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://qoy.yonumen.top

PHP:  assert($x > 0);
来源：http://sdy.fzhhl.top

JS:   console.assert(x > 0);
来源：http://wio.xinyue.icu

TS:   console.assert(x > 0);
来源：http://zdj.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://yib.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fpv.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://tap.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://ean.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://kkg.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://tby.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mbo.chenlongwang.top

JS:   e.message;  e.stack
来源：http://xri.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vvu.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ptk.bjfxy.top

Go:   err.Error()
来源：http://pne.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://vhx.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://ety.wangdashe.top

[H09] 带错误码的异常
来源：http://xnj.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rrq.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fio.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dwb.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tli.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rns.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vid.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://ura.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jeb.andypj.xyz

[H10] 资源自动释放
来源：http://uhz.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://idd.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dqm.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sxb.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fxp.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cta.ehwqpu.com

Go:   defer f.Close()
来源：http://lcp.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hmp.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qtg.yanxiufei.cn

================================================================================
来源：http://srg.epnwcf.com

I. 正则表达式
来源：http://rfe.shanyushiyangtech.top

================================================================================
来源：http://qjl.zhengqikj.top

[I01] 判断是否匹配
来源：http://uba.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wnu.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://spa.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://nyn.yfazqb.com

TS:   /\d+/.test(s)
来源：http://brb.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pxo.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uuc.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://etm.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nhl.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://lqh.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://gpp.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wgj.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lju.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://mjf.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vwz.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gaz.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://ljh.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hzr.fzhhl.top

[I03] 提取捕获分组
来源：http://zhr.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hza.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uvz.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bhr.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://quw.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gdp.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sgm.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hgd.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iwd.ywan-chungtsiang.top

[I04] 正则替换
来源：http://utb.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mbk.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gvv.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jlc.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ilq.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://rux.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bls.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://amp.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rjm.snrcjt.cn

[I05] 按正则拆分
来源：http://nga.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yib.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nrn.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://cal.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://opz.shanyushiyangtech.top

Java: s.split("\\s*,\\s*")
来源：http://ikm.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vdi.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://lhg.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xcd.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hok.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vgb.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://plj.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uqh.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lwk.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ftd.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hwe.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://off.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dgp.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://vyq.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://phw.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xcf.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ffr.hongshengwenyu.top

TS:   /error/gim
来源：http://pfm.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wtr.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dvf.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://sxz.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vyu.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://opv.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zpy.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sse.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vob.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eiv.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jjc.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vun.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ilq.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nje.guannengcc.top

================================================================================
来源：http://bka.chenlongwang.top

J. 日期与时间
来源：http://hui.hongshengwenyu.top

================================================================================
来源：http://zzx.zdbjq.cn

[J01] 获取当前时间
来源：http://amj.yonumen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qms.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lir.cashguo.top

JS:   new Date();  Date.now()
来源：http://nvf.sweek.top

TS:   new Date();  Date.now()
来源：http://fkm.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ufh.cdnleiting.top

Go:   time.Now()
来源：http://dus.redwolf501.top

Ruby: Time.now
来源：http://jbm.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cek.guannengcc.top

[J02] 格式化输出
来源：http://pho.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tba.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zhd.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ufc.epnwcf.com

TS:   d.toISOString()
来源：http://wii.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://stb.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lpg.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfp.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hcv.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://sqx.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mbv.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xzc.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://ntr.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://zgg.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://bfu.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tbf.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://znd.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://npd.meibo888.top

[J04] 时间戳与日期互转
来源：http://hxb.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lpi.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wqr.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://olo.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://sow.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ulo.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://own.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://guu.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hcw.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://rsx.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://ica.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ciq.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://usa.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sju.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://meo.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rat.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://rmi.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://zyl.chenzaomai.com

[J06] 计算两时间之差
来源：http://bsa.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://euh.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://lgr.zhengqikj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qhy.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vzj.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://dwt.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://bon.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://dgq.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://oze.sxryk.cn

[J07] 比较两个日期
来源：http://dfo.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://qyg.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ynj.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kaq.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ubl.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://afs.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://svb.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kil.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://rgr.vehdjk.com

[J08] 提取年月日与星期
来源：http://oqw.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qdj.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qez.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dev.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://inu.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uzh.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kgq.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jks.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://icp.zdqjudy.top

[J09] 时区处理
来源：http://ege.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zvv.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bly.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hzi.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gud.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yao.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dsr.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pek.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ike.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://jgw.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xfx.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qgi.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://olj.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ljo.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rfy.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kid.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mrt.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bix.zhongyouzk.top

================================================================================
来源：http://glg.bbcook.cn

K. JSON 与序列化
来源：http://egy.jqgfzy.top

================================================================================
来源：http://gsm.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://mfo.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://whb.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ygf.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://vbs.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://zrq.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oet.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://upw.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://vyd.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gtf.wangdashe.top

[K02] JSON 字符串转对象
来源：http://org.guowangkeji.top

Py:   json.loads(s)
来源：http://rpo.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bry.tarul.cn

JS:   JSON.parse(s)
来源：http://elt.yonumen.top

TS:   JSON.parse(s)
来源：http://wux.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nva.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://tva.hammf.cn

Ruby: JSON.parse(s)
来源：http://ijf.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vyh.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://kzc.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ylr.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fip.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wlz.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mka.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wkx.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bzo.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://fkw.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fte.pycfn.com

[K04] 读取 JSON 文件
来源：http://vum.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://umv.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sla.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dtj.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ffr.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tdt.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xqc.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://obx.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kek.nanxinkj.top

[K05] 深拷贝对象
来源：http://ozx.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://ngl.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://adl.c1oappe.top

JS:   structuredClone(obj)
来源：http://qfj.andypj.xyz

TS:   structuredClone(obj)
来源：http://cku.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://efq.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nis.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iqt.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dfm.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://olf.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eir.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fva.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cah.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hxt.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hnx.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mlf.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tsq.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxk.jianghu66.top

[K07] 进制转换
来源：http://kdv.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://naa.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gbs.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dyu.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mgp.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sai.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iit.dashuyun.cn


<!-- 参考信息 -->