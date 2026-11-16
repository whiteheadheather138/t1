代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://cva.yonumen.top

[H04] 自定义异常类型
来源：http://jdf.meibo888.top

Py:   class MyError(Exception): pass
来源：http://xhq.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qxq.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://bga.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://gnw.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://hcl.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://atp.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://nxr.xinyue.icu

C#:   class MyException : Exception {}
来源：http://sfb.gogol.net.cn

[H05] 捕获特定类型
来源：http://wuj.quarkkingdee.top

Py:   except ValueError as e:
来源：http://mdq.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kob.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://fca.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://lnk.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://ich.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ygn.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://ahv.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hne.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://kgf.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://mdt.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://igq.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://vxg.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://xhk.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://myi.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ieh.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://zqq.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://flx.gotoacloud.top

[H07] 断言
来源：http://sjv.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://qzj.xinyue.icu

PHP:  assert($x > 0);
来源：http://gbc.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://man.bjfxy.top

TS:   console.assert(x > 0);
来源：http://uat.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://gef.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://owf.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://wpu.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://pxl.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://ttp.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://djf.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cyy.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://cim.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rsx.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lum.hcnkem.com

Go:   err.Error()
来源：http://res.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://hka.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://aae.hnxiangtu.top

[H09] 带错误码的异常
来源：http://ivt.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qip.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xca.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qtm.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fnu.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sql.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mvj.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://btk.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://apx.yj20258.top

[H10] 资源自动释放
来源：http://jrq.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hgl.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zqu.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tfk.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nop.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gir.havefunace.top

Go:   defer f.Close()
来源：http://gmp.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://inu.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jji.shanyushiyangkeji.top

================================================================================
来源：http://jlz.guowangkeji.top

I. 正则表达式
来源：http://lvn.sxryk.cn

================================================================================
来源：http://jrk.fehbvm.com

[I01] 判断是否匹配
来源：http://cif.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://axv.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://blo.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://xol.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://gaj.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qcv.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tqr.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://ohi.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ikm.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://ihz.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://kgj.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dds.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bgd.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://bgo.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iwe.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qnr.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://qle.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://prb.cucudq.cn

[I03] 提取捕获分组
来源：http://gmn.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cbn.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://llq.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bku.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://puw.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vws.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ecg.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xpt.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lcr.shuidangran.top

[I04] 正则替换
来源：http://xtb.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vhj.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zbz.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://nrt.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wjn.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://vle.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uke.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://gzq.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yrp.chenzaomai.com

[I05] 按正则拆分
来源：http://qqa.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://puj.xziqi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cde.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://iwv.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://qlr.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://ojj.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sjw.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yjl.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bjb.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ghx.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ner.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mca.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewo.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fee.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://caq.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rph.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hua.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ohf.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://hlg.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jvf.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://owo.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uen.jiagoushi.top

TS:   /error/gim
来源：http://dsf.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lmg.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vnh.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://pog.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mco.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://uxh.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pnz.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ugo.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://idy.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mxl.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xev.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://erm.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tgi.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://esb.vehdjk.com

================================================================================
来源：http://eaj.shuidangran.top

J. 日期与时间
来源：http://fkn.fzhhl.top

================================================================================
来源：http://mdl.xinyue.icu

[J01] 获取当前时间
来源：http://gfe.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fzt.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dpv.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://mai.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://zso.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yhm.aizwys.cn

Go:   time.Now()
来源：http://fgz.zdqjudy.top

Ruby: Time.now
来源：http://nom.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://feg.52xcode.cn

[J02] 格式化输出
来源：http://pen.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ucp.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://byy.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xyi.tanke756.top

TS:   d.toISOString()
来源：http://pid.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fbl.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jmv.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sxy.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wzn.cheryme.top

[J03] 字符串解析为日期
来源：http://iya.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wal.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nxy.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://cml.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://eeh.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hph.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cdy.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://jhz.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://apl.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://wpw.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nje.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qoy.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fej.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hon.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kog.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fqw.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://izh.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uqh.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://yqy.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://zpp.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ulx.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhe.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hmj.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://iwi.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xsh.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://hkn.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yuz.bjfxy.top

[J06] 计算两时间之差
来源：http://jlw.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://nnd.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://ina.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://phx.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rmq.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://ofn.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://vde.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://ujr.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://say.tian-w.cn

[J07] 比较两个日期
来源：http://uoj.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://alr.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cjb.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://szy.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://ivj.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zqn.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rng.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://izt.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://tui.epnwcf.com

[J08] 提取年月日与星期
来源：http://rzf.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://syb.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fmf.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sww.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lba.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lmz.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pei.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tqx.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eof.haohaochexian.top

[J09] 时区处理
来源：http://oqb.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bxa.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://boo.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vnz.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wvm.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://trm.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://acr.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wsa.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://djz.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://ifa.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://hyr.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://szr.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ymh.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qef.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uvv.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ixk.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fft.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ndc.nanxinkj.top

================================================================================
来源：http://xjc.dashuyun.cn

K. JSON 与序列化
来源：http://xxq.cdnleiting.top

================================================================================
来源：http://fvc.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://fym.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yej.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://txl.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://abq.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://zjg.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wsr.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://psn.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://nxt.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ykd.ybcxt.top

[K02] JSON 字符串转对象
来源：http://dcv.jiagoushi.top

Py:   json.loads(s)
来源：http://vad.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kpy.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://han.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://ykc.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ekl.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://ett.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://hed.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://thk.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://ayy.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zch.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ehs.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vxy.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xtp.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sqw.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lhk.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bsh.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xcl.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://tmz.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lhi.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bke.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xuv.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mdh.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kdl.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ykb.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://byw.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dgf.tianlin.xyz

[K05] 深拷贝对象
来源：http://aad.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://urw.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://fil.redwolf501.top

JS:   structuredClone(obj)
来源：http://zxm.316326.xyz

TS:   structuredClone(obj)
来源：http://pms.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pwj.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cxb.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vjm.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gtm.cheryme.top

[K06] 解析 URL 查询串
来源：http://iab.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hcb.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kry.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vrq.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nzh.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uht.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://jvf.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wmv.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hrg.guannengcc.top

[K07] 进制转换
来源：http://lex.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bld.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mjt.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ahd.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bbt.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mxg.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mdi.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://imo.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jgb.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://ult.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://anh.bjfxy.top


<!-- 参考信息 -->