代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://pph.yueranfly.top

[H04] 自定义异常类型
来源：http://fji.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://vzm.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://roq.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://lak.52xcode.cn

TS:   class MyError extends Error {}
来源：http://lxj.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://tqp.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wfb.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://xqs.pycfn.com

C#:   class MyException : Exception {}
来源：http://xvj.52xcode.cn

[H05] 捕获特定类型
来源：http://tzk.epnwcf.com

Py:   except ValueError as e:
来源：http://kzx.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bvs.aizwys.cn

JS:   if (e instanceof TypeError) {}
来源：http://izg.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://ssx.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://xob.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qjd.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://tob.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tha.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://tse.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://lue.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://ljf.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://geu.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dlt.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://obr.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zbu.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://bzo.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://slx.cheryme.top

[H07] 断言
来源：http://mby.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://blh.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://plb.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://tqn.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://apc.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://wdj.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sbd.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://mga.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://sur.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://nab.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://zrt.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mwf.hfpthk.cn

JS:   e.message;  e.stack
来源：http://ehc.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vji.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mgp.shuidangran.top

Go:   err.Error()
来源：http://iok.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://noa.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://mwh.tian-w.cn

[H09] 带错误码的异常
来源：http://xpp.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ssx.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://edb.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://akj.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://boh.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ysu.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zpq.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://aob.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xjw.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://xmu.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pjs.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ayq.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fxu.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bnt.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xzn.sxryk.cn

Go:   defer f.Close()
来源：http://erv.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gvv.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sye.yvedp.cn

================================================================================
来源：http://vai.epnwcf.com

I. 正则表达式
来源：http://dhm.aibaodan.cn

================================================================================
来源：http://mrj.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://ifs.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aie.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://bgo.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://ref.zycfv.cn

TS:   /\d+/.test(s)
来源：http://ugi.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nlz.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ruy.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://ity.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://boc.cucudq.cn

[I02] 提取所有匹配
来源：http://ipe.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://cyn.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sbq.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gcr.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://iib.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jir.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ynq.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://mpl.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wan.guannengcc.top

[I03] 提取捕获分组
来源：http://vkf.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cpy.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pub.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rbx.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oux.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ifh.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eag.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cde.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oug.ppjwa.cn

[I04] 正则替换
来源：http://ljm.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qjm.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jux.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://yer.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://kev.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://nsf.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fai.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sqi.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eoe.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://hhq.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fmn.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://she.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://yhd.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://srl.jlsjyb.cn

Java: s.split("\\s*,\\s*")
来源：http://myu.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hti.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nae.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xjo.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jpe.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ife.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ivs.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tav.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqz.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tqh.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wpn.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://odx.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dlt.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://yab.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xvm.tianlin.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dcl.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vvh.316326.xyz

TS:   /error/gim
来源：http://xau.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nwd.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qcn.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://mzg.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gup.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://gpe.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mnj.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fvz.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://img.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wef.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rtj.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://drb.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://igi.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://glk.nwbrower.top

================================================================================
来源：http://jjq.snrcjt.cn

J. 日期与时间
来源：http://chn.hfpthk.cn

================================================================================
来源：http://ulx.fengsongda.top

[J01] 获取当前时间
来源：http://inz.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ulj.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://krc.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://zpo.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://qmt.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://chq.c1oappe.top

Go:   time.Now()
来源：http://edn.yj20258.top

Ruby: Time.now
来源：http://rds.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qlh.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://xot.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ycs.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dul.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ptm.yj20258888.top

TS:   d.toISOString()
来源：http://xoa.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hjj.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sin.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgx.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ypu.redwolf501.top

[J03] 字符串解析为日期
来源：http://gvv.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://psb.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qab.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://zqj.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://kgf.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://yke.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://stq.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://zjr.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pad.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://dhi.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hay.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://icp.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trn.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://yyd.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://apf.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yiv.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dgq.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rcc.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://crp.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://fju.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fsb.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qwt.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ndq.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://urq.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yoc.hfpthk.cn

Ruby: Time.now + 7 * 86400
来源：http://hxk.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://snk.tarul.cn

[J06] 计算两时间之差
来源：http://uvj.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://rlw.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://zni.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ete.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zhu.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ujs.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://dlm.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://jva.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://zoz.yonumen.top

[J07] 比较两个日期
来源：http://zaq.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://uhm.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wab.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://tiz.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tkp.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yav.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zaj.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://hud.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://mvj.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://dna.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rju.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sif.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://idg.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://smz.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sgq.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nwz.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vpz.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://drn.zhiwuduotai.top

[J09] 时区处理
来源：http://olu.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mvw.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hce.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://czw.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vbe.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qrc.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nlv.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xho.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tjy.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://xev.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qzb.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jua.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kvh.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fdh.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mqj.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kvh.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ffj.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nhb.tianlin.xyz

================================================================================
来源：http://pnw.jlsjyb.cn

K. JSON 与序列化
来源：http://cpv.jinqigfzy.top

================================================================================
来源：http://exc.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://xtb.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mvs.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jkc.yonumen.top

JS:   JSON.stringify(obj)
来源：http://bfm.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://kby.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dsm.yanxiufei.cn

Go:   json.Marshal(obj)
来源：http://nlf.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lzn.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cbi.xziqi.cn

[K02] JSON 字符串转对象
来源：http://nrb.zhengqikj.top

Py:   json.loads(s)
来源：http://jay.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hos.gotoacloud.top

JS:   JSON.parse(s)
来源：http://gss.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://kto.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ipn.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://ftg.smart0.xyz

Ruby: JSON.parse(s)
来源：http://nbg.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dti.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://vjj.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tix.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tff.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ell.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ppl.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://euv.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pct.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qle.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dnh.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://ema.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nwh.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://drz.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqh.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lsf.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vmz.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wuq.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gms.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eeq.zdbjq.cn

[K05] 深拷贝对象
来源：http://epr.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://vro.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://ryw.gotoacloud.top

JS:   structuredClone(obj)
来源：http://cri.yangfankeji.com

TS:   structuredClone(obj)
来源：http://dym.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://isc.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://enf.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iun.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eqt.hcnkem.com

[K06] 解析 URL 查询串
来源：http://wqb.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://you.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pdf.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://doe.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ktv.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ugy.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ayd.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fxr.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jxp.xylfe.cn

[K07] 进制转换
来源：http://zar.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cpd.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nrg.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://siv.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ifs.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aio.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mve.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kss.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tmg.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://ndr.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://koe.vqdsnc.cn


<!-- 参考信息 -->