代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://vjx.chenzaomai.com

[H04] 自定义异常类型
来源：http://ksw.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://fsp.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nbi.pycfn.com

JS:   class MyError extends Error {}
来源：http://ohu.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://vqa.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://vwh.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uke.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://fng.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://cyb.hcnkem.com

[H05] 捕获特定类型
来源：http://dot.hnqzz.top

Py:   except ValueError as e:
来源：http://bzu.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tov.daxiang520.top

JS:   if (e instanceof TypeError) {}
来源：http://bpn.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://mhr.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://uzy.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rod.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://sgj.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hwn.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://cho.daxiang520.top

Py:   value = d.get("k") or default
来源：http://qus.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://svo.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://cjc.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://xyt.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pyf.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tqu.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://nev.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://ttr.shanyushiyangtech.top

[H07] 断言
来源：http://xzb.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://gkt.yuxming.cn

PHP:  assert($x > 0);
来源：http://zxl.mhx1999.top

JS:   console.assert(x > 0);
来源：http://frp.aizwys.cn

TS:   console.assert(x > 0);
来源：http://joc.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://dbp.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hld.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://ijb.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://znj.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://ivz.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://khf.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://szy.cqqwz.cn

JS:   e.message;  e.stack
来源：http://zdo.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vds.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://skz.chenjidiqi.icu

Go:   err.Error()
来源：http://fch.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://smf.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://eop.wangdashe.top

[H09] 带错误码的异常
来源：http://jez.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xcm.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://grx.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kum.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://phs.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kkd.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gtz.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nde.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yzl.c1oappe.top

[H10] 资源自动释放
来源：http://nud.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://crf.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ahl.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qtw.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hfw.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmt.ivvv.top

Go:   defer f.Close()
来源：http://zti.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xgp.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://atc.yuanzhike.top

================================================================================
来源：http://rol.tian-w.cn

I. 正则表达式
来源：http://fcc.guowangkeji.top

================================================================================
来源：http://zgs.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://eia.yongpay.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ofh.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://gva.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://qmh.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://pqw.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xkc.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bid.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://abz.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://waa.yangfankeji.com

[I02] 提取所有匹配
来源：http://vva.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://whg.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fqg.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wwr.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://dts.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nzg.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qyd.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://yoh.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://klc.bjfxy.top

[I03] 提取捕获分组
来源：http://tys.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ewm.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tqy.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vjn.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yen.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://izj.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qec.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vxm.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wnc.ivvv.top

[I04] 正则替换
来源：http://yrr.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ltz.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mea.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://mdg.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://ibx.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dbv.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uhc.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vpq.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tus.cucudq.cn

[I05] 按正则拆分
来源：http://uub.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mav.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zcu.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://lxg.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://mng.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://ili.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eki.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://phf.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ngi.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jft.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jzu.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mya.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://png.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzr.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xyl.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jvz.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fiz.52xcode.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jbm.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://har.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ipv.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://caa.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xvc.tian-w.cn

TS:   /error/gim
来源：http://apv.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://spj.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tat.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://fux.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lvv.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://dkx.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://puj.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oto.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wco.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqu.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ocg.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gjb.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pms.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lqi.tanke756.top

================================================================================
来源：http://hpr.bbcook.cn

J. 日期与时间
来源：http://xco.jinyuanbaomall.cn

================================================================================
来源：http://ssm.bbcook.cn

[J01] 获取当前时间
来源：http://gmt.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://yit.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hlz.316326.xyz

JS:   new Date();  Date.now()
来源：http://sbb.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://lpk.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://chu.daxiang520.top

Go:   time.Now()
来源：http://ezw.chenzaomai.com

Ruby: Time.now
来源：http://anb.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fkg.jqgfzy.top

[J02] 格式化输出
来源：http://tfm.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oag.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cwj.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vza.ydjk.org.cn

TS:   d.toISOString()
来源：http://aql.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hxr.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zbm.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zse.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vds.bbcook.cn

[J03] 字符串解析为日期
来源：http://van.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cic.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bjq.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://txz.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://das.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://hzg.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://meo.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://icl.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bbw.yuxming.cn

[J04] 时间戳与日期互转
来源：http://yew.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ldd.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xnz.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qgr.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tcq.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://igx.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uyz.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lnx.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ybe.sweek.top

[J05] 时间加减（加 7 天）
来源：http://osl.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://tce.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ffg.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yaf.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtm.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://tcu.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aym.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://vpw.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kum.gogol.net.cn

[J06] 计算两时间之差
来源：http://xrt.pycfn.com

Py:   (end - start).total_seconds()
来源：http://wsk.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://zsk.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oeo.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rff.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://umz.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://tzi.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://yvj.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://eab.ppjwa.cn

[J07] 比较两个日期
来源：http://ihp.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://vvz.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ivw.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wgj.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://yud.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://abe.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nwg.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://wrs.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://xqe.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://etz.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mwl.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hfn.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vik.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qxi.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fck.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jbv.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tdd.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oxp.cdnleiting.top

[J09] 时区处理
来源：http://bpb.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jad.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qrs.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dfp.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xvo.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://upv.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eoz.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zaq.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rfs.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://alb.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iss.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aut.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jzv.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vrr.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://txq.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nff.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lkr.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pad.zhoulong.xyz

================================================================================
来源：http://bqm.aizwys.cn

K. JSON 与序列化
来源：http://cso.jqgfzy.top

================================================================================
来源：http://kme.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://npv.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://upc.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://imh.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://uwc.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://ana.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qne.smart0.xyz

Go:   json.Marshal(obj)
来源：http://fmr.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://spn.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xvj.xinyue.icu

[K02] JSON 字符串转对象
来源：http://kod.sweek.top

Py:   json.loads(s)
来源：http://vbb.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://itl.chenlongwang.top

JS:   JSON.parse(s)
来源：http://djr.gotoacloud.top

TS:   JSON.parse(s)
来源：http://akk.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://msy.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://nfs.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://ocq.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gty.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://tym.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yad.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://phk.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wbr.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hct.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vxl.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zla.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zjo.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gfa.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://zdn.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oso.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wcm.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vzs.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umn.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xyz.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ssx.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://kcj.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zbo.birdmap.top

[K05] 深拷贝对象
来源：http://ihz.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://uho.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://dsx.wangdashe.top

JS:   structuredClone(obj)
来源：http://bpg.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://ijx.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jca.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://njx.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sze.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tok.hcnkem.com

[K06] 解析 URL 查询串
来源：http://jzz.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://myb.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://afi.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://noo.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wek.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://soj.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nwf.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tur.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://alv.yj20258.top

[K07] 进制转换
来源：http://vjl.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zsj.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://trq.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://csz.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://csi.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tcu.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ojz.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qgw.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ewc.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://ypp.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://ccn.52xcode.cn


<!-- 参考信息 -->