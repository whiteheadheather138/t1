代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://kee.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eiy.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tmf.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rgj.yj202588.top

[H03] 主动抛出异常
来源：http://ywj.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://ofa.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dhy.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://yzn.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://evt.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yat.gotoacloud.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mqn.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://img.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://zoa.ctjpmb.com

[H04] 自定义异常类型
来源：http://fqv.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://yeq.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://gfq.epnwcf.com

JS:   class MyError extends Error {}
来源：http://unv.yonumen.top

TS:   class MyError extends Error {}
来源：http://enn.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://one.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tnx.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://bwj.yonumen.top

C#:   class MyException : Exception {}
来源：http://zhp.tianlin.xyz

[H05] 捕获特定类型
来源：http://qyy.aibaodan.cn

Py:   except ValueError as e:
来源：http://lvy.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oov.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://bzx.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://nsv.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://orc.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jwb.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://abl.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aun.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://nrd.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://soz.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://edt.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://wkx.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://rky.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tte.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nau.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://tyw.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://gwp.yfazqb.com

[H07] 断言
来源：http://yce.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://pyn.xylfe.cn

PHP:  assert($x > 0);
来源：http://vev.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://bwo.ivvv.top

TS:   console.assert(x > 0);
来源：http://wjk.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://ifl.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pze.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://klg.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://anz.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://kpq.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://rnp.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jyw.nanxinkj.top

JS:   e.message;  e.stack
来源：http://npn.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ewz.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ruh.xylfe.cn

Go:   err.Error()
来源：http://uuo.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://uuy.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://rmh.xinyue.icu

[H09] 带错误码的异常
来源：http://xqv.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://smk.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lct.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fkq.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uuj.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yct.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://srs.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lsu.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vxk.mhx1999.top

[H10] 资源自动释放
来源：http://tvi.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://duz.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fhu.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iia.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yqw.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vaq.zhijiandao.cn

Go:   defer f.Close()
来源：http://hgx.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wtk.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vmo.sjlbkw.cn

================================================================================
来源：http://iop.redwolf501.top

I. 正则表达式
来源：http://rnm.tianlin.xyz

================================================================================
来源：http://iwe.pycfn.com

[I01] 判断是否匹配
来源：http://ahz.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nsg.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://llz.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://fwz.sxryk.cn

TS:   /\d+/.test(s)
来源：http://dcq.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jmh.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://itj.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://csd.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sfn.tarul.cn

[I02] 提取所有匹配
来源：http://vok.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://zgv.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ocw.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xwh.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://plu.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ypo.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://icq.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://gzd.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ags.meibo888.top

[I03] 提取捕获分组
来源：http://gax.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kfa.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jld.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dck.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wua.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wzm.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xoq.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jmr.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oit.hnxiangtu.top

[I04] 正则替换
来源：http://gdw.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uxg.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wea.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dwa.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rzy.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://xpn.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://xww.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://edn.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ckt.fehbvm.com

[I05] 按正则拆分
来源：http://poh.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gfk.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jzx.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://fpg.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://nkl.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://ltn.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://slu.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://qze.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vie.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://guu.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xag.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zyo.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nnp.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xlv.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bdm.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iyo.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fvc.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jnt.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://npp.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://edx.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kot.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mqy.cashguo.top

TS:   /error/gim
来源：http://rbf.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qcz.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zif.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://wul.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uod.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://vzu.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zup.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wst.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vkk.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jps.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://hqn.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://auf.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vva.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ajg.sysykeji.top

================================================================================
来源：http://wyu.sysykeji.top

J. 日期与时间
来源：http://wdv.ehwqpu.com

================================================================================
来源：http://yfm.andypj.xyz

[J01] 获取当前时间
来源：http://hqp.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://per.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jgw.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://vly.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://mas.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://igc.jlsjyb.cn

Go:   time.Now()
来源：http://pkj.sufxvd.cn

Ruby: Time.now
来源：http://kie.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cgo.bjfxy.top

[J02] 格式化输出
来源：http://vxy.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pps.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wjl.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dvg.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://smo.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://khr.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qio.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oef.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wce.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://cmd.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zlq.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jcv.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://zbs.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://lth.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gzp.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uob.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://qgk.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nmd.cashguo.top

[J04] 时间戳与日期互转
来源：http://ebp.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mwh.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nxn.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://flz.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ywf.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mwm.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lyt.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ged.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://utj.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://rjf.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://tvp.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ewt.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://scs.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ofu.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://vxg.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ziy.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://zgq.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wav.hesvh.cn

[J06] 计算两时间之差
来源：http://bfl.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://pha.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://voe.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ptv.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://maf.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://ntv.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://ztx.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://pro.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://xmg.jqgfzy.top

[J07] 比较两个日期
来源：http://uxe.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://lil.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bju.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://cqn.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://sqm.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://udc.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xrg.fanxiaobao.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://kno.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://qwk.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://jcg.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://amb.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vnd.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zof.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zgj.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gyr.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jkp.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sik.yongpay.top

[J09] 时区处理
来源：http://eck.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://idt.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://evt.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jjw.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ius.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ces.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cxc.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fft.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cwx.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://vpb.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://slp.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pmo.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oti.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ydj.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ejd.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://juo.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://poi.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qea.sxryk.cn

================================================================================
来源：http://xze.hongshengwenyu.top

K. JSON 与序列化
来源：http://nlu.ivvv.top

================================================================================
来源：http://yax.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://zaa.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kmf.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://udf.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://ift.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://nuk.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ycg.hammf.cn

Go:   json.Marshal(obj)
来源：http://imz.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://jyy.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wzp.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://luf.xuanzx.com

Py:   json.loads(s)
来源：http://yeb.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mwn.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://vox.yj202588.top

TS:   JSON.parse(s)
来源：http://dkd.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rqn.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://yuy.hammf.cn

Ruby: JSON.parse(s)
来源：http://fhs.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ocl.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://jfd.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cuw.xylfe.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aqp.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lwv.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tyk.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bjv.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fyq.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://rtx.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lzv.bjfxy.top

[K04] 读取 JSON 文件
来源：http://aia.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pgn.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uck.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cym.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynh.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ptp.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fgf.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nmq.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vum.bbcook.cn

[K05] 深拷贝对象
来源：http://xqo.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://zqj.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://odt.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://zwr.gogol.net.cn

TS:   structuredClone(obj)
来源：http://pbq.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sqi.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ofw.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fqd.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wbg.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://ihu.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gat.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nnf.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bun.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qjh.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ici.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lre.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tct.zhoulong.xyz


<!-- 参考信息 -->