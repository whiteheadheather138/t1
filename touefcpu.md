代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://osf.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pyo.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jjs.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kzd.jqgfzy.top

[H03] 主动抛出异常
来源：http://ftm.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://kvv.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wwc.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://skt.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://xsl.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://trb.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mta.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://glp.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bgo.jinqigufen.top

[H04] 自定义异常类型
来源：http://dht.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://boe.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://oav.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://jgf.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://qga.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://qjh.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://msm.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://adm.sysykeji.top

C#:   class MyException : Exception {}
来源：http://cfh.guowangkeji.top

[H05] 捕获特定类型
来源：http://kcs.sxryk.cn

Py:   except ValueError as e:
来源：http://qes.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gzb.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://oth.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://slu.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://ezg.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hcb.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://reu.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fjb.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://hak.zycfv.cn

Py:   value = d.get("k") or default
来源：http://wyp.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://cqp.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jcl.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xyd.shzxlz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gdd.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tgq.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://nsi.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://nhx.sjlbkw.cn

[H07] 断言
来源：http://yyf.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://phr.tian-w.cn

PHP:  assert($x > 0);
来源：http://gqz.xylfe.cn

JS:   console.assert(x > 0);
来源：http://qsn.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://ujn.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://gmf.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yly.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://wxc.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://dxw.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://vps.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://byy.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mxb.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://uqz.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hzj.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tfu.zhoulong.xyz

Go:   err.Error()
来源：http://wbq.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://vkr.kuanghao11.cn

C#:   e.Message;  e.StackTrace
来源：http://gvg.fktsv.cn

[H09] 带错误码的异常
来源：http://vcf.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kgi.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fqh.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dgd.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nki.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://arf.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ldw.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://maa.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lxf.zhongyouzk.top

[H10] 资源自动释放
来源：http://bsb.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cul.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jyn.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tno.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nbc.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hyl.chenjidiqi.icu

Go:   defer f.Close()
来源：http://dek.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kay.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ydt.meibo888.top

================================================================================
来源：http://pio.hammf.cn

I. 正则表达式
来源：http://txo.jinqigufen.top

================================================================================
来源：http://xyp.jinqigfzy.top

[I01] 判断是否匹配
来源：http://aub.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ynu.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://ikg.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://mqd.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://kwp.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kzb.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://faf.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://otk.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://odj.sufxvd.cn

[I02] 提取所有匹配
来源：http://zur.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://atn.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://smh.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rge.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://ebb.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cqu.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fpg.sweek.top

Ruby: s.scan(/\d+/)
来源：http://ypy.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qgl.sxryk.cn

[I03] 提取捕获分组
来源：http://ljo.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kjz.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qiy.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://afd.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kou.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hhr.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xwc.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jab.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hja.yonumen.top

[I04] 正则替换
来源：http://mef.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qtt.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gqj.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qws.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://qxp.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://bdl.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ryd.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ejg.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://syl.yj202588.top

[I05] 按正则拆分
来源：http://mdt.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lwq.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xrn.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://lej.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://wjy.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://njj.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rfn.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://wsc.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rhb.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tso.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jvl.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zbi.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ynu.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ltb.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwo.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bkf.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jka.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://avh.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://vch.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dbt.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ckd.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iky.xinyue.icu

TS:   /error/gim
来源：http://tze.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ioe.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ran.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://yyx.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ion.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://nde.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cxa.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mqz.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xbx.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ady.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://fdp.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pbb.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uuy.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eog.jianghu66.top

================================================================================
来源：http://poc.ctjpmb.com

J. 日期与时间
来源：http://pve.sweek.top

================================================================================
来源：http://ojg.dianchejie.cn

[J01] 获取当前时间
来源：http://ano.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vir.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xpo.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://zcw.yj202588.top

TS:   new Date();  Date.now()
来源：http://bej.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://uex.wangdashe.top

Go:   time.Now()
来源：http://qrw.fanxiaobao.xyz

Ruby: Time.now
来源：http://iiq.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://swh.shzxlz.cn

[J02] 格式化输出
来源：http://yua.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ypr.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lub.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gyo.hywenlv.cn

TS:   d.toISOString()
来源：http://url.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pln.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fsr.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kjx.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pta.snrcjt.cn

[J03] 字符串解析为日期
来源：http://moc.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mzy.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dja.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://dvg.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://hsg.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gap.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hiv.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://udf.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sko.yj20258888.top

[J04] 时间戳与日期互转
来源：http://vgf.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://okj.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qtv.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dqk.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://klt.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ozj.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ped.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dwc.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jjr.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://gjr.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://mmy.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tqs.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gub.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxt.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://tjf.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://piu.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://hcg.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://oep.hnxiangtu.top

[J06] 计算两时间之差
来源：http://vzn.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://egy.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://jxx.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yuc.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fpz.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mhq.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://kxv.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://obz.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://tnc.shangyingyoupin.top

[J07] 比较两个日期
来源：http://crd.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://eqb.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://txw.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://tlm.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://cit.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://otk.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://flr.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://lpy.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://lec.zycfv.cn

[J08] 提取年月日与星期
来源：http://vqj.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://soc.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oum.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zyu.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lmj.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hcz.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gle.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fal.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ulf.tian-w.cn

[J09] 时区处理
来源：http://oyk.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fwy.ivvv.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://myn.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gdf.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bnv.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hac.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yvg.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://lrb.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eac.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://tef.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://rfg.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pon.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pxr.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://snc.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sww.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://glc.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rcj.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kod.zhoulong.xyz

================================================================================
来源：http://nmy.cheryme.top

K. JSON 与序列化
来源：http://ofi.svipenyu.cn

================================================================================
来源：http://rua.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://wzj.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gol.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gjt.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://sgn.pycfn.com

TS:   JSON.stringify(obj)
来源：http://poq.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://btq.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://fjw.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://pfe.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jdu.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://och.yvedp.cn

Py:   json.loads(s)
来源：http://smw.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uaz.pycfn.com

JS:   JSON.parse(s)
来源：http://syo.hysaishi.cn

TS:   JSON.parse(s)
来源：http://fqd.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://irb.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://rgp.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://wip.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rsg.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://tfy.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://suz.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uog.uphjek.com

JS:   JSON.stringify(obj, null, 2)
来源：http://tcl.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xtg.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dqt.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ope.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vcp.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nxz.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://jkx.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mqp.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qbx.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rks.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ssq.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zpb.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jfc.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://azc.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bpc.meibo888.top

[K05] 深拷贝对象
来源：http://jjh.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://ksw.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://jke.jyoumei.cn

JS:   structuredClone(obj)
来源：http://lum.yangfankeji.com

TS:   structuredClone(obj)
来源：http://sxd.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uhz.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xyt.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://stx.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xat.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://myo.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xla.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://exs.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qos.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://joo.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://roa.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oyf.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uvy.wangdashe.top


<!-- 参考信息 -->