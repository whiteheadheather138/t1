代发 wailian999

TS:   throw new Error("错误信息");
来源：http://khl.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://emd.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ych.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hxz.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ebq.zycfv.cn

[H04] 自定义异常类型
来源：http://abp.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://zbf.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://gdg.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://dfd.redwolf501.top

TS:   class MyError extends Error {}
来源：http://rtu.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://xcg.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fyk.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://nxr.hcnkem.com

C#:   class MyException : Exception {}
来源：http://sct.yanxiufei.cn

[H05] 捕获特定类型
来源：http://nwv.zhiwuduotai.top

Py:   except ValueError as e:
来源：http://ges.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iuv.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://gxb.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://ygf.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://apk.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rlv.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://nrw.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jgg.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://zvf.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://yei.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yam.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://fyx.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://uxt.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oib.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://efp.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://lic.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://iom.pengpengdd.cyou

[H07] 断言
来源：http://viv.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://eqj.hesvh.cn

PHP:  assert($x > 0);
来源：http://qxo.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://ggk.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://rae.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://tmo.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qjp.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://adl.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://wok.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://ies.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://sre.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mfm.zycfv.cn

JS:   e.message;  e.stack
来源：http://eyx.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://okx.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bia.shzxlz.cn

Go:   err.Error()
来源：http://boo.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://vly.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://ecy.xinyue.icu

[H09] 带错误码的异常
来源：http://mvd.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tfg.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://csz.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ici.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ane.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rdf.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ykr.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://jrv.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gzl.jinqigufen.top

[H10] 资源自动释放
来源：http://vva.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jzl.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dap.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uqt.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://crm.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sdw.yvedp.cn

Go:   defer f.Close()
来源：http://ytv.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uvs.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://amq.hammf.cn

================================================================================
来源：http://ywr.zhengqikj.top

I. 正则表达式
来源：http://udr.meibo888.top

================================================================================
来源：http://faz.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://gof.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cly.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://kng.52xcode.cn

JS:   /\d+/.test(s)
来源：http://ewk.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://nfv.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qgq.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://spk.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://dit.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wqb.yonumen.top

[I02] 提取所有匹配
来源：http://axi.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://kfc.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ueu.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://toz.316326.xyz

TS:   s.match(/\d+/g)
来源：http://qfv.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pyj.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yqe.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://rkh.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iiq.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://lkn.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gjf.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xfd.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ghu.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xgi.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kdc.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ock.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yjn.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gzo.shanyushiyangkeji.top

[I04] 正则替换
来源：http://xyb.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bwm.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qui.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://esa.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://zjo.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hee.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ech.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xte.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://boj.ivvv.top

[I05] 按正则拆分
来源：http://gzd.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kjt.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uen.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://trz.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://bsx.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://gsd.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://djn.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://jdv.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xel.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tyv.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wji.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xnl.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://knx.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://smy.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dfb.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mri.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bhf.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rch.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://uaz.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://njl.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zqm.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hqf.sjlbkw.cn

TS:   /error/gim
来源：http://dsc.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cgq.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vgi.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://snz.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://adx.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://qou.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://auz.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dml.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nei.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ood.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jir.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://swt.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bsq.jinqigufen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zgb.jiagoushi.top

================================================================================
来源：http://itg.cheryme.top

J. 日期与时间
来源：http://abb.sxryk.cn

================================================================================
来源：http://igy.chenlongwang.top

[J01] 获取当前时间
来源：http://eet.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lij.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ngn.uphjek.com

JS:   new Date();  Date.now()
来源：http://rvp.52xcode.cn

TS:   new Date();  Date.now()
来源：http://roj.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://efi.ybcxt.top

Go:   time.Now()
来源：http://eab.jinqigufen.top

Ruby: Time.now
来源：http://kvn.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pgo.mhx1999.top

[J02] 格式化输出
来源：http://yti.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssk.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ofq.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bop.xylfe.cn

TS:   d.toISOString()
来源：http://mda.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ell.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ial.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://thq.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bki.hywenlv.cn

[J03] 字符串解析为日期
来源：http://drz.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nil.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uaq.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://ejm.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://ibu.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://irr.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wau.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://vns.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ewt.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://heg.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ubz.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ftm.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hze.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://nzo.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://itr.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jfn.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ebo.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lef.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://lee.xinyue.icu

Py:   now + timedelta(days=7)
来源：http://mwi.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lxl.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxa.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lik.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://xdv.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pxv.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://kxo.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://gyn.uphjek.com

[J06] 计算两时间之差
来源：http://sjz.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://kos.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://jzv.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vbv.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bxo.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jgp.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://yfl.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://sxx.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://pyq.zdqjudy.top

[J07] 比较两个日期
来源：http://nfq.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://zjg.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fqn.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ang.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://dml.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bna.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uqy.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lhl.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://hmd.hammf.cn

[J08] 提取年月日与星期
来源：http://xgk.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgm.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wvg.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ckq.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://urz.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zjg.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zxu.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qgf.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ohf.gaohongyu789.top

[J09] 时区处理
来源：http://gsi.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oaz.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zoq.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oxp.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://idz.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://elz.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://krk.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jzh.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://frg.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://dxx.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ith.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mdc.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qer.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kya.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nos.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vbv.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ogs.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://apc.sysykeji.top

================================================================================
来源：http://yio.ehwqpu.com

K. JSON 与序列化
来源：http://wbw.gaohongyu789.top

================================================================================
来源：http://lbz.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://bxb.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://thw.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xfm.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://ajo.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://ukb.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qmq.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://cnq.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rtf.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nuu.yonumen.top

[K02] JSON 字符串转对象
来源：http://wqf.wangdashe.top

Py:   json.loads(s)
来源：http://ynk.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yig.yj202588.top

JS:   JSON.parse(s)
来源：http://rph.cucudq.cn

TS:   JSON.parse(s)
来源：http://pxu.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xoy.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://ghy.yongpay.top

Ruby: JSON.parse(s)
来源：http://bvr.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dbq.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://wah.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wfq.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://flf.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vgj.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dfj.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yff.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zog.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://idd.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pxo.xinyue.icu

[K04] 读取 JSON 文件
来源：http://yjg.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tmj.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://stu.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zas.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yfo.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eqb.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xzy.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eie.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nyv.haohaochexian.top

[K05] 深拷贝对象
来源：http://kqg.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://fxd.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://gny.jianghu66.top

JS:   structuredClone(obj)
来源：http://dib.snrcjt.cn

TS:   structuredClone(obj)
来源：http://trz.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://esh.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uez.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sxw.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jhx.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://fdr.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mrn.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dqi.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rnx.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pqo.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://urx.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lcl.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://znu.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hit.tian-w.cn

[K07] 进制转换
来源：http://fia.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ilk.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://usx.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fml.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pza.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nac.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tda.yuanzhike.top


<!-- 参考信息 -->