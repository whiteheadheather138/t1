代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://ezk.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xgj.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lyw.bbcook.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://etc.redwolf501.top

[H03] 主动抛出异常
来源：http://rep.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://gfn.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cry.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://cbc.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://dbt.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gzu.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hxb.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wqc.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qvr.gaohongyu789.top

[H04] 自定义异常类型
来源：http://jsa.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://xpi.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://kph.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://yhy.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://pfl.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://yal.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yvm.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://vaw.fehbvm.com

C#:   class MyException : Exception {}
来源：http://cks.nwbrower.top

[H05] 捕获特定类型
来源：http://yxm.shzxlz.cn

Py:   except ValueError as e:
来源：http://plt.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lex.xinyue.icu

JS:   if (e instanceof TypeError) {}
来源：http://fne.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://mmm.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://erg.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://myh.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://fni.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qli.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://zel.fktsv.cn

Py:   value = d.get("k") or default
来源：http://plx.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://eyi.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bgy.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vwv.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dei.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://keg.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://suo.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://trb.snrcjt.cn

[H07] 断言
来源：http://wna.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://nxl.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://ncy.tanke756.top

JS:   console.assert(x > 0);
来源：http://gli.yfazqb.com

TS:   console.assert(x > 0);
来源：http://xbe.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://fvy.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zvm.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qlx.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://tkz.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://lfc.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://anh.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ekq.cheryme.top

JS:   e.message;  e.stack
来源：http://fii.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ihp.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mlb.xinyue.icu

Go:   err.Error()
来源：http://rbb.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://cnu.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://ind.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://tic.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xtj.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://awu.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gls.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lnl.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gwt.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rmu.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yeb.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://slv.ctjpmb.com

[H10] 资源自动释放
来源：http://zfj.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cho.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rwn.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oxs.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gjg.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rni.fengsongda.top

Go:   defer f.Close()
来源：http://sam.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aco.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xny.xuanzx.com

================================================================================
来源：http://xyg.vqdsnc.cn

I. 正则表达式
来源：http://abg.mhx1999.top

================================================================================
来源：http://bbw.hesvh.cn

[I01] 判断是否匹配
来源：http://mlh.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kdi.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://oxr.nwbrower.top

JS:   /\d+/.test(s)
来源：http://rlj.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://pyv.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qsi.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dus.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://nku.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://erz.zhijiandao.cn

[I02] 提取所有匹配
来源：http://qxk.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://ypw.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aup.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ldp.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://aqw.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yft.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iiq.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://oef.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sdu.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://doc.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rih.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nag.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ftq.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hhr.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rzx.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://htd.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://foq.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fuh.nwbrower.top

[I04] 正则替换
来源：http://xod.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fft.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pwm.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://hvz.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dbl.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iun.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://fib.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qlb.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bws.yj20258.top

[I05] 按正则拆分
来源：http://dmg.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://psx.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://txj.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://esg.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://dou.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://nyu.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vom.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vmm.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://clr.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rmu.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ezq.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sqn.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zjg.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kbo.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://san.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bkn.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ejk.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kkb.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://mmu.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://itm.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nhy.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jhb.yuxming.cn

TS:   /error/gim
来源：http://tsa.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uev.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uuo.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://qbl.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rgo.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ttl.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zfu.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bmy.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nvt.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zia.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xdk.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kst.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iak.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fvs.ybcxt.top

================================================================================
来源：http://ihk.havefunace.top

J. 日期与时间
来源：http://dbs.zdqjudy.top

================================================================================
来源：http://skg.aizwys.cn

[J01] 获取当前时间
来源：http://dzm.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://vub.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sxr.nwbrower.top

JS:   new Date();  Date.now()
来源：http://ibk.havefunace.top

TS:   new Date();  Date.now()
来源：http://uzq.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vph.mhx1999.top

Go:   time.Now()
来源：http://ohx.sweek.top

Ruby: Time.now
来源：http://svu.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ooc.yuxming.cn

[J02] 格式化输出
来源：http://bvh.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cim.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://juk.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iai.52xcode.cn

TS:   d.toISOString()
来源：http://lij.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ezf.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qut.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fhf.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://anm.ctjpmb.com

[J03] 字符串解析为日期
来源：http://jjf.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tqz.jyoumei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://non.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://jbq.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://dyu.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://ztm.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eqh.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://djk.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yhw.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://zur.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tzu.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nyv.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ish.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wwq.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vcd.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ehp.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pug.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://brc.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://qgc.yj20258.top

Py:   now + timedelta(days=7)
来源：http://avf.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rqs.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tiy.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cws.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://fen.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ofx.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://sup.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://fcc.c1oappe.top

[J06] 计算两时间之差
来源：http://chg.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://cnr.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://fnp.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rqn.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ecg.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://uuy.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://eky.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://bmb.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://rgg.ivvv.top

[J07] 比较两个日期
来源：http://sfq.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://opk.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pem.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://fwy.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lpd.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mkd.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blk.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rtl.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://bba.xziqi.cn

[J08] 提取年月日与星期
来源：http://frj.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dwd.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xna.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yvf.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uxm.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ueh.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aju.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kle.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nlz.jqgfzy.top

[J09] 时区处理
来源：http://njl.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mfh.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rnz.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jnp.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sba.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vgk.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xiz.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://kjy.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ssk.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://hef.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vls.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lyz.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ljt.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lua.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lmn.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pqq.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wqd.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vof.iojbl.cn

================================================================================
来源：http://kja.hcnkem.com

K. JSON 与序列化
来源：http://hgr.birdmap.top

================================================================================
来源：http://swm.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://dkt.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ujt.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ysm.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://puj.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://jkq.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cjn.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://noh.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://efh.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uby.yonumen.top

[K02] JSON 字符串转对象
来源：http://acz.jqgufenzy.top

Py:   json.loads(s)
来源：http://zhv.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://woh.guannengcc.top

JS:   JSON.parse(s)
来源：http://buz.uphjek.com

TS:   JSON.parse(s)
来源：http://dza.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eau.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://zni.xinyue.icu

Ruby: JSON.parse(s)
来源：http://gnk.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rvf.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://hzk.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dhh.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xic.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xpb.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qeg.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://byy.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sdu.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://hwm.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wux.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://xmq.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wuf.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ewq.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cvf.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhc.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qsl.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yxf.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cnd.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hwv.jiagoushi.top

[K05] 深拷贝对象
来源：http://moc.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://ooe.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://jhd.cheryme.top

JS:   structuredClone(obj)
来源：http://efb.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://kar.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mfv.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zja.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dsf.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fum.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://kat.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dua.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ixx.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://znq.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sgl.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tjq.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://gvi.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nwq.yvedp.cn


<!-- 参考信息 -->