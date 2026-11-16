代发 wailian999

JS:   class MyError extends Error {}
来源：http://jaz.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://gwv.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://yzi.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://maa.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://ptd.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://uik.andypj.xyz

[H05] 捕获特定类型
来源：http://ifq.wangdashe.top

Py:   except ValueError as e:
来源：http://cyi.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bmx.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://idm.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://zcc.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://xie.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fry.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://rou.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qup.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://oel.vehdjk.com

Py:   value = d.get("k") or default
来源：http://dqq.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ngy.jyoumei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xrg.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://unw.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iuo.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mkf.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://myp.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://fhi.sxryk.cn

[H07] 断言
来源：http://lys.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://lpx.fengsongda.top

PHP:  assert($x > 0);
来源：http://hga.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://bqq.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://sqt.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://kny.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jxo.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://zth.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://mmf.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://oqz.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://gnn.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pwm.mhx1999.top

JS:   e.message;  e.stack
来源：http://ekl.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vgo.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zqh.zdqjudy.top

Go:   err.Error()
来源：http://clo.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://lfm.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://dwe.c1oappe.top

[H09] 带错误码的异常
来源：http://cgg.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pxc.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gsp.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mzs.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oud.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jjp.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wpe.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://olr.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rsg.cashguo.top

[H10] 资源自动释放
来源：http://nyb.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aso.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wry.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eoo.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://whx.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pnc.zycfv.cn

Go:   defer f.Close()
来源：http://len.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xlm.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://czk.zhoulong.xyz

================================================================================
来源：http://hcm.jinyuanbaomall.cn

I. 正则表达式
来源：http://edg.yuxming.cn

================================================================================
来源：http://qqr.yj20258888.top

[I01] 判断是否匹配
来源：http://cum.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zph.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://ocm.ybcxt.top

JS:   /\d+/.test(s)
来源：http://ezj.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://xia.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://whi.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://des.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://ezc.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://omc.tanke756.top

[I02] 提取所有匹配
来源：http://ioq.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://kfd.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ghk.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zpx.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://mkh.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lay.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ddc.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://pgi.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://snw.hywenlv.cn

[I03] 提取捕获分组
来源：http://ovm.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yyk.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nil.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://erv.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wjg.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nmp.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lgp.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nqa.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://edp.zhijiandao.cn

[I04] 正则替换
来源：http://zjc.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mvs.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wzc.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pia.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://tlc.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kev.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iyz.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://itf.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tnj.pycfn.com

[I05] 按正则拆分
来源：http://muz.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yry.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aqu.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://rcj.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://ged.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://lbj.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tqy.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://rin.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://its.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qbe.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qlt.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ehh.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xfa.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hpz.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mjf.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sep.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vmm.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://euf.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://jmw.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://idt.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://njv.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vlp.jinqigfzy.top

TS:   /error/gim
来源：http://ese.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nwi.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mmb.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://cdz.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vrd.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://zmw.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cfp.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zri.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://flh.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zfv.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://azu.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wgz.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wvn.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://anh.epnwcf.com

================================================================================
来源：http://thw.0kj1m.cn

J. 日期与时间
来源：http://wdd.sxryk.cn

================================================================================
来源：http://yth.ivvv.top

[J01] 获取当前时间
来源：http://yig.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hbk.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qpm.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://god.xinyue.icu

TS:   new Date();  Date.now()
来源：http://uvp.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hdt.hysaishi.cn

Go:   time.Now()
来源：http://xov.snrcjt.cn

Ruby: Time.now
来源：http://gtk.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fse.ppjwa.cn

[J02] 格式化输出
来源：http://cwu.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://psn.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qnp.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ckd.yj20258888.top

TS:   d.toISOString()
来源：http://lbf.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://clv.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pmp.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fpp.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vea.c1oappe.top

[J03] 字符串解析为日期
来源：http://cnt.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://azl.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aqc.yonumen.top

JS:   new Date("2024-01-02")
来源：http://vns.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://odw.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ihp.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xbs.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://kbk.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bfg.daria6918.cn

[J04] 时间戳与日期互转
来源：http://cqt.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zyw.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nop.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://unz.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://abs.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qru.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zog.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cqy.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://llv.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://xrl.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://gqe.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kyj.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://scr.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fnw.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://hqm.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zlr.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://fdj.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qdw.yuxming.cn

[J06] 计算两时间之差
来源：http://rix.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://kzb.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://cxt.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://waq.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qkp.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://zfa.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://kmw.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://tbk.bbcook.cn

C#:   (end - start).TotalSeconds
来源：http://dwv.sysykeji.top

[J07] 比较两个日期
来源：http://pmx.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://lcu.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rth.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://czh.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://xop.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gop.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jdm.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lnn.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://pcy.ivvv.top

[J08] 提取年月日与星期
来源：http://wfu.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dul.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://thw.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vct.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gyg.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gme.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrm.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dgh.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kdv.feifeiyinyue.top

[J09] 时区处理
来源：http://sul.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nfy.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fvh.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzv.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hcj.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fny.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://znh.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://emz.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://njt.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://otn.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://xuk.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iqw.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bmd.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ksy.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://osv.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hgw.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tgz.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ibp.nanxinkj.top

================================================================================
来源：http://rln.yanxiufei.cn

K. JSON 与序列化
来源：http://soy.xylfe.cn

================================================================================
来源：http://rpn.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://shh.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rcd.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eay.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://vcd.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://vdz.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fzk.shuidangran.top

Go:   json.Marshal(obj)
来源：http://qil.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rvt.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oss.mhx1999.top

[K02] JSON 字符串转对象
来源：http://nqk.sweek.top

Py:   json.loads(s)
来源：http://zzs.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yft.uphjek.com

JS:   JSON.parse(s)
来源：http://vfx.haohaochexian.top

TS:   JSON.parse(s)
来源：http://idt.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tdn.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://osp.sxryk.cn

Ruby: JSON.parse(s)
来源：http://ago.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ozs.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://llq.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nei.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oyj.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://eto.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vtd.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jdk.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://trv.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://drr.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nxb.vehdjk.com

[K04] 读取 JSON 文件
来源：http://hgr.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://exn.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://snb.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fjq.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fyi.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jlp.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://brp.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jvq.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qgz.snrcjt.cn

[K05] 深拷贝对象
来源：http://nyi.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://lia.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://uhg.aibaodan.cn

JS:   structuredClone(obj)
来源：http://ssd.birdmap.top

TS:   structuredClone(obj)
来源：http://njz.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nyx.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://klk.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ubm.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lup.zhiwuduotai.top

[K06] 解析 URL 查询串
来源：http://ycz.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://thy.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://svh.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://brg.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ncw.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aei.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://yhs.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pmn.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jsy.hysaishi.cn

[K07] 进制转换
来源：http://log.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://edb.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://drt.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ecl.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baa.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bap.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://avt.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qqf.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://azb.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://ink.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://and.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://pzu.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://xys.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://oed.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ccb.zdqjudy.top


<!-- 参考信息 -->