代发 wailian999

TS:   throw new Error("错误信息");
来源：http://ohb.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ekm.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dob.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://npy.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://bmd.guowangkeji.top

[H04] 自定义异常类型
来源：http://bnq.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://hwz.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eey.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://vbe.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://bue.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://mov.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gzm.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://zqt.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://rhi.tian-w.cn

[H05] 捕获特定类型
来源：http://ina.hammf.cn

Py:   except ValueError as e:
来源：http://ikm.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tds.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://aep.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://mdn.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://qsd.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://muj.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://rmi.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xrr.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://vic.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://epq.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ppe.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://qyt.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://fkr.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gff.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jrp.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://rxy.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://fxc.zhijiandao.cn

[H07] 断言
来源：http://vva.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://mmf.pycfn.com

PHP:  assert($x > 0);
来源：http://vwb.yj20258888.top

JS:   console.assert(x > 0);
来源：http://ahe.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://wch.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://ccy.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wzx.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nvp.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://ggb.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://jsl.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://fey.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xsc.aibaodan.cn

JS:   e.message;  e.stack
来源：http://ihc.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://caz.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://dob.feifeiyinyue.top

Go:   err.Error()
来源：http://jmm.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://yzb.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://jmj.cdnleiting.top

[H09] 带错误码的异常
来源：http://acq.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://evf.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lcw.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kbk.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rjp.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://moe.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cbe.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ine.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://csg.vqdsnc.cn

[H10] 资源自动释放
来源：http://dqw.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uai.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tnc.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nff.tianlin.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cfj.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jbe.gogol.net.cn

Go:   defer f.Close()
来源：http://ngd.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iku.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zel.jlsjyb.cn

================================================================================
来源：http://iun.ybcxt.top

I. 正则表达式
来源：http://kor.cqqwz.cn

================================================================================
来源：http://yka.fzhhl.top

[I01] 判断是否匹配
来源：http://aiw.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zzz.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://nlv.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://xeb.zycfv.cn

TS:   /\d+/.test(s)
来源：http://gaj.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mkg.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yfg.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://deg.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fob.cqqwz.cn

[I02] 提取所有匹配
来源：http://nvc.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://wqr.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dam.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ohi.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://spp.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rij.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://khj.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://mjy.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eap.pycfn.com

[I03] 提取捕获分组
来源：http://xxl.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bwo.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ouw.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vyu.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ipe.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zxv.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nnz.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iuj.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://khv.xuetiantiany.cn

[I04] 正则替换
来源：http://mix.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mya.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dir.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://lkk.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://nfd.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://qix.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ddf.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xhq.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://chi.xuetiantiany.cn

[I05] 按正则拆分
来源：http://sza.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://bcc.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pgp.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://yuh.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://ijv.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://iue.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qut.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://icg.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uvy.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zpa.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pcc.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://riz.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tvi.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fcn.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blh.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ysl.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uwq.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://czr.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://qdo.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lop.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ybm.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ukv.xuetiantiany.cn

TS:   /error/gim
来源：http://mzk.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://php.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jdh.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://gzt.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nyy.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://usy.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wms.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://laa.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zox.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cvu.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jio.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lag.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://osj.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tnj.tanke756.top

================================================================================
来源：http://xik.nwbrower.top

J. 日期与时间
来源：http://xcl.ywan-chungtsiang.top

================================================================================
来源：http://wiq.andypj.xyz

[J01] 获取当前时间
来源：http://xcc.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bic.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oow.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://bta.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://fac.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xui.kuanghao11.cn

Go:   time.Now()
来源：http://nwo.zdbjq.cn

Ruby: Time.now
来源：http://dtr.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lqt.haohaochexian.top

[J02] 格式化输出
来源：http://axe.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://upg.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://buc.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hcp.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://zvy.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rtx.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rla.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fgv.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rnp.birdmap.top

[J03] 字符串解析为日期
来源：http://frw.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://urz.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hvd.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://lpq.cheryme.top

TS:   new Date("2024-01-02")
来源：http://zik.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wtb.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kvm.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://daj.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tpr.nwbrower.top

[J04] 时间戳与日期互转
来源：http://olr.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bmt.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fqc.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rkq.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://swn.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://okp.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bdl.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wzq.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bes.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://qww.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://cvo.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wxn.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kmo.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpb.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://ppl.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gwp.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://qua.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://xcn.gzhubu.top

[J06] 计算两时间之差
来源：http://mxz.316326.xyz

Py:   (end - start).total_seconds()
来源：http://yob.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://zyn.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dxa.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://abj.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xib.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://exi.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://tik.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://xji.birdmap.top

[J07] 比较两个日期
来源：http://aux.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://qas.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tau.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://xvw.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://obk.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oes.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jak.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://baj.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://pay.yongpay.top

[J08] 提取年月日与星期
来源：http://mqy.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iqq.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bno.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eow.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://poy.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ron.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vjy.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wxz.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://urh.snrcjt.cn

[J09] 时区处理
来源：http://ysl.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lyp.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://txw.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://htw.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oav.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mqg.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aqx.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aux.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bqv.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://edj.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://big.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://msp.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jel.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ebo.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uqt.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sjg.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uax.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wou.xinyue.icu

================================================================================
来源：http://qwa.sjlbkw.cn

K. JSON 与序列化
来源：http://zvc.jiagoushi.top

================================================================================
来源：http://atv.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://hmj.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eix.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pbf.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://xgu.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://hty.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cxe.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://ulw.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://kjp.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://loe.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://whx.ehwqpu.com

Py:   json.loads(s)
来源：http://ysb.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zqi.0kj1m.cn

JS:   JSON.parse(s)
来源：http://pjh.xylfe.cn

TS:   JSON.parse(s)
来源：http://uhz.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kxf.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://qku.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://grs.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://obo.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://kzq.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baj.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://apf.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lkl.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://stt.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ksg.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rdb.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://yzy.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ktm.hnqzz.top

[K04] 读取 JSON 文件
来源：http://jii.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fvx.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fzv.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rru.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://thn.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sdk.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zil.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://xur.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://svg.fktsv.cn

[K05] 深拷贝对象
来源：http://dyc.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://xvv.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://kaf.bbcook.cn

JS:   structuredClone(obj)
来源：http://wzg.aizwys.cn

TS:   structuredClone(obj)
来源：http://nei.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://kak.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://erp.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pbc.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lph.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://ujn.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://het.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qvy.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qbs.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kyr.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://etu.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fzy.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uig.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mxo.fehbvm.com

[K07] 进制转换
来源：http://ner.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://azf.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zew.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfs.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iho.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pyb.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cbk.snrcjt.cn


<!-- 参考信息 -->