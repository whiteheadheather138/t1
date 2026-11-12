代发 wailian999

[H03] 主动抛出异常
来源：http://xfp.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://nbh.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mdb.yonumen.top

JS:   throw new Error("错误信息");
来源：http://cna.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://hww.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dfh.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bwo.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zyp.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gfp.uphjek.com

[H04] 自定义异常类型
来源：http://ouj.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://amq.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://bbk.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://mjc.sweek.top

TS:   class MyError extends Error {}
来源：http://yip.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://sfh.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ewo.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://vvp.aizwys.cn

C#:   class MyException : Exception {}
来源：http://ozj.sjlbkw.cn

[H05] 捕获特定类型
来源：http://ywc.yanxiufei.cn

Py:   except ValueError as e:
来源：http://xuf.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ars.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://nur.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://mkq.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://ezb.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lqu.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://wng.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://itm.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://qko.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://vuf.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://zgi.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://oqq.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cdh.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zby.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ggt.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://oge.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://myu.c1oappe.top

[H07] 断言
来源：http://mwr.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://bvi.cdnleiting.top

PHP:  assert($x > 0);
来源：http://xhr.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://hsi.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://dtn.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://hac.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pcj.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://mne.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://aoe.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://sok.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://ljb.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lqv.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://vbq.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gxt.chenzaomai.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jcc.shanyushiyangkeji.top

Go:   err.Error()
来源：http://zlc.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://cav.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://dnx.zycfv.cn

[H09] 带错误码的异常
来源：http://wkm.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ypi.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://zgi.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://crv.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nzo.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mry.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yfp.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tfj.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ogs.bbcook.cn

[H10] 资源自动释放
来源：http://uyt.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://wcn.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bhb.ivvv.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uuw.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qjn.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://avu.hcnkem.com

Go:   defer f.Close()
来源：http://rmm.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aif.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ixt.jinqigfzy.top

================================================================================
来源：http://ebh.fzhhl.top

I. 正则表达式
来源：http://puc.gaohongyu789.top

================================================================================
来源：http://hpp.ydzc1.top

[I01] 判断是否匹配
来源：http://qnp.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yhk.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://ayu.yj20258.top

JS:   /\d+/.test(s)
来源：http://vyj.guannengcc.top

TS:   /\d+/.test(s)
来源：http://yjs.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://itk.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nst.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://iib.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iyz.svipenyu.cn

[I02] 提取所有匹配
来源：http://nyk.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://anj.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rjy.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ljv.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://sit.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qgy.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wha.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://wcz.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zyl.cashguo.top

[I03] 提取捕获分组
来源：http://ovl.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rzt.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gmb.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://txn.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gcm.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mjx.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uhr.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pww.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kmv.daria6918.cn

[I04] 正则替换
来源：http://men.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nve.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bse.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://kfv.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hec.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://shv.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jok.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qsv.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://obt.nanxinkj.top

[I05] 按正则拆分
来源：http://cov.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://suj.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vfi.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://kdu.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://czf.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://vjq.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oqt.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://ura.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pkr.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hzg.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iiu.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blg.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgp.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vmw.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lqv.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sck.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tsa.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pza.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://obi.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kjp.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dal.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qho.uphjek.com

TS:   /error/gim
来源：http://lbz.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ezo.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yqb.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://oda.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oyg.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://dzz.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tce.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pxc.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cyt.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dlz.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rdf.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jbv.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gqs.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kla.chenzaomai.com

================================================================================
来源：http://swx.gogol.net.cn

J. 日期与时间
来源：http://yrp.ydjk.org.cn

================================================================================
来源：http://yvf.dashuyun.cn

[J01] 获取当前时间
来源：http://dat.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://rry.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gyf.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://zrg.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://gdv.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ckx.yonumen.top

Go:   time.Now()
来源：http://laa.shzxlz.cn

Ruby: Time.now
来源：http://mjb.xziqi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yle.xylfe.cn

[J02] 格式化输出
来源：http://wgq.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ypw.svipenyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bia.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://klk.hnxiangtu.top

TS:   d.toISOString()
来源：http://meh.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qgy.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qrq.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bvx.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jlx.sxryk.cn

[J03] 字符串解析为日期
来源：http://sae.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sfq.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qwk.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://slb.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://jtt.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://edu.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kad.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://gim.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ugn.bjfxy.top

[J04] 时间戳与日期互转
来源：http://chb.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://coa.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zun.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpm.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lvs.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bjy.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ylu.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bmi.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yai.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://zyn.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://kib.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://wfc.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ial.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zqi.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://los.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bby.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://thc.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://hue.uphjek.com

[J06] 计算两时间之差
来源：http://rlr.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://ekk.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://sjh.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nms.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xvq.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://rrv.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://ppj.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://zer.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://yfl.yj20258888.top

[J07] 比较两个日期
来源：http://rwg.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://kcq.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eno.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://jcz.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://ydx.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ydj.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://awr.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://jwc.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ekm.aizwys.cn

[J08] 提取年月日与星期
来源：http://gxm.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zjr.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qma.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mjl.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cjx.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xrn.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fbj.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ggt.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vzy.aizwys.cn

[J09] 时区处理
来源：http://rgu.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mvr.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tah.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fkd.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzr.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xbe.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yaf.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gth.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ymg.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://bgo.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lba.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xkw.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dfe.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ayg.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ldt.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vjf.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://akt.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://auk.ywan-chungtsiang.top

================================================================================
来源：http://wzo.quarkkingdee.top

K. JSON 与序列化
来源：http://jbk.jqgufenzy.top

================================================================================
来源：http://rih.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://gmq.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sie.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://glx.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://czh.cashguo.top

TS:   JSON.stringify(obj)
来源：http://vrd.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vgx.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://eqm.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://ajp.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://dbb.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://qrw.andypj.xyz

Py:   json.loads(s)
来源：http://jhf.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ivz.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://gjt.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://srh.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sma.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://dls.52xcode.cn

Ruby: JSON.parse(s)
来源：http://lfk.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zhz.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://gsc.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tva.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fpc.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://xwt.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dzm.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tvx.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tsl.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cls.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cfa.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://xgg.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kqj.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fpm.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dno.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ygj.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gxr.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lsn.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dcb.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yht.jqgfzy.top

[K05] 深拷贝对象
来源：http://kqk.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://lyh.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://dgj.dianchejie.cn

JS:   structuredClone(obj)
来源：http://jhi.meibo888.top

TS:   structuredClone(obj)
来源：http://xkh.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zwt.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hvt.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ink.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://tvm.hcnkem.com

[K06] 解析 URL 查询串
来源：http://mpj.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ifd.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dfl.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zgu.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qyj.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rkf.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ujv.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pur.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uun.tianlin.xyz

[K07] 进制转换
来源：http://ygk.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jhr.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jul.pengpengdd.cyou


<!-- 参考信息 -->