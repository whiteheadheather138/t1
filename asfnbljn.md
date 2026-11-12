代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://vux.mhx1999.top

[H04] 自定义异常类型
来源：http://eck.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://gqp.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://kxw.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://fsz.c1oappe.top

TS:   class MyError extends Error {}
来源：http://okm.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://uas.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xjh.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://pig.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://qgd.ctjpmb.com

[H05] 捕获特定类型
来源：http://lyr.svipenyu.cn

Py:   except ValueError as e:
来源：http://yyb.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gff.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://unm.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://duz.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://cqn.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aug.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://kaz.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dfe.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://rad.fehbvm.com

Py:   value = d.get("k") or default
来源：http://rzo.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gtz.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qcq.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ere.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rpl.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://krc.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://buq.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://nse.cucudq.cn

[H07] 断言
来源：http://hmj.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://djg.xuanzx.com

PHP:  assert($x > 0);
来源：http://rzs.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://uks.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://pyx.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://zol.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nvb.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ech.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://qsm.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://fmt.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://fce.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://puu.yj202588.top

JS:   e.message;  e.stack
来源：http://rnx.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wyq.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://mzu.mhx1999.top

Go:   err.Error()
来源：http://zbq.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://qap.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://ial.hfpthk.cn

[H09] 带错误码的异常
来源：http://lgv.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://are.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pyi.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://smz.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yxw.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lvu.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://otr.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://dfd.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zkb.uphjek.com

[H10] 资源自动释放
来源：http://rto.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mkz.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qyj.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tjd.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zla.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://quh.sweek.top

Go:   defer f.Close()
来源：http://akm.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zsh.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://deg.gzhubu.top

================================================================================
来源：http://lnk.tian-w.cn

I. 正则表达式
来源：http://yog.jinqigufen.top

================================================================================
来源：http://jin.gotoacloud.top

[I01] 判断是否匹配
来源：http://kwr.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ewy.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://xzc.yangfankeji.com

JS:   /\d+/.test(s)
来源：http://ykj.havefunace.top

TS:   /\d+/.test(s)
来源：http://eqv.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fvr.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://shf.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://khx.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mqx.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://xii.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://dsb.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ynw.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lfe.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://fro.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://woq.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qtt.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://wdq.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bfo.c1oappe.top

[I03] 提取捕获分组
来源：http://sjc.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pmc.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dep.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rkr.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lpy.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://amj.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rez.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hdh.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jvt.sweek.top

[I04] 正则替换
来源：http://rwl.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tcm.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://puj.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://uzc.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://yqx.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://odf.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hlq.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ifj.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kud.jlsjyb.cn

[I05] 按正则拆分
来源：http://bai.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ecg.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wip.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://akw.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://qss.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://bio.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ayb.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zir.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://irh.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jqi.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pes.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://szz.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qrn.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jsn.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uba.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mks.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ddw.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ilw.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://bsx.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wrh.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mvd.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pon.zhaomingkeji.xyz

TS:   /error/gim
来源：http://lry.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ooc.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ueb.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://nju.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dnd.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://mkc.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lbz.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://exl.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kze.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yjh.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://als.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://coc.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dpo.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mzm.zycfv.cn

================================================================================
来源：http://icl.0kj1m.cn

J. 日期与时间
来源：http://jlw.feifeiyinyue.top

================================================================================
来源：http://lga.yonumen.top

[J01] 获取当前时间
来源：http://rcz.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://esf.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xdc.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://xpn.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://lqt.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zeb.zhengqikj.top

Go:   time.Now()
来源：http://orv.cucudq.cn

Ruby: Time.now
来源：http://cjx.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wjx.quarkkingdee.top

[J02] 格式化输出
来源：http://owg.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xfd.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cjt.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hya.cashguo.top

TS:   d.toISOString()
来源：http://sjo.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zmk.jyoumei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zgx.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ehb.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kzw.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://quq.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://odg.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ewz.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://luf.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://ujt.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://ldg.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tvw.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://kdh.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zho.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://vmi.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bmg.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://idb.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vdp.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wca.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wxe.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zyb.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bdv.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bfp.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://zio.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://ejf.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jzd.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgd.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://moi.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://mmg.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yuz.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://ywa.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ubo.hnqzz.top

[J06] 计算两时间之差
来源：http://hdz.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://pmy.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://jup.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ugy.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xyl.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gxu.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://jed.sufxvd.cn

Ruby: end - start                 # 返回秒数
来源：http://mrg.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://wga.yuanzhike.top

[J07] 比较两个日期
来源：http://qsb.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://itr.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dpy.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lga.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://yib.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bpi.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ydx.fanxiaobao.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://jew.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://tfd.hysaishi.cn

[J08] 提取年月日与星期
来源：http://sxc.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gqx.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rrx.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sxg.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jab.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vgx.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mtk.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dao.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zbw.9152youxi.cn

[J09] 时区处理
来源：http://dty.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gmf.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sgs.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://coh.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rfa.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oym.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wdw.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://szp.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gyd.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://hrb.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vod.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ayg.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xty.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yws.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sbi.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fzl.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tsf.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rat.daria6918.cn

================================================================================
来源：http://zte.dianchejie.cn

K. JSON 与序列化
来源：http://gkz.shuidangran.top

================================================================================
来源：http://peh.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://ohx.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nds.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oha.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://lky.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://wly.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kjk.hcnkem.com

Go:   json.Marshal(obj)
来源：http://dqa.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ixm.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tyw.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://wka.havefunace.top

Py:   json.loads(s)
来源：http://jis.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://brh.shzxlz.cn

JS:   JSON.parse(s)
来源：http://cmf.sxryk.cn

TS:   JSON.parse(s)
来源：http://ssz.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dcl.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://fao.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://gvo.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://egb.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://wbs.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nzm.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://onj.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://irz.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lxo.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cli.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nbb.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://ozb.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nqj.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://jdk.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://emt.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mfk.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yof.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tgz.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ptb.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jrh.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mem.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qlr.hysaishi.cn

[K05] 深拷贝对象
来源：http://bfi.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://nuk.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://cuo.shzxlz.cn

JS:   structuredClone(obj)
来源：http://qdq.cdnleiting.top

TS:   structuredClone(obj)
来源：http://ozo.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://umz.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://our.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hsf.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lyf.tarul.cn

[K06] 解析 URL 查询串
来源：http://wyo.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sai.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xpp.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://txp.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vkm.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oyg.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xwn.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ovt.zhengqikj.top

[K07] 进制转换
来源：http://qqt.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yyt.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qme.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zce.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fnr.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pfy.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xjx.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hil.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tje.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://mti.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://vby.pengpengdd.cyou


<!-- 参考信息 -->