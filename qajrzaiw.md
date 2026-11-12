代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qyf.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://lqh.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://ath.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://eia.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tnt.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://uym.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://une.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://ezj.aizwys.cn

Py:   value = d.get("k") or default
来源：http://pmz.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tda.nanxuanxn.top

JS:   obj?.a?.b;  d ?? default
来源：http://zlc.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://von.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lid.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pfp.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://utq.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://frs.yanxiufei.cn

[H07] 断言
来源：http://wny.jinqigufen.top

Py:   assert x > 0, "必须为正"
来源：http://pcd.zdbjq.cn

PHP:  assert($x > 0);
来源：http://pmd.cheryme.top

JS:   console.assert(x > 0);
来源：http://ydh.pycfn.com

TS:   console.assert(x > 0);
来源：http://fqu.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://tjq.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iqu.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://rlr.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://cns.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://njw.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://ail.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eme.zhixingplan.top

JS:   e.message;  e.stack
来源：http://qkp.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xfr.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ikq.cashguo.top

Go:   err.Error()
来源：http://qag.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://xyw.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://cij.zhoulong.xyz

[H09] 带错误码的异常
来源：http://gzx.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tuw.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ota.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mzt.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kmz.nwbrower.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vsq.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jju.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://kyb.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wjl.gzhubu.top

[H10] 资源自动释放
来源：http://yxf.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dns.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bsi.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gnp.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oqd.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pls.sjlbkw.cn

Go:   defer f.Close()
来源：http://joz.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xtd.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mpj.nwbrower.top

================================================================================
来源：http://hwm.zhixingplan.top

I. 正则表达式
来源：http://sld.sufxvd.cn

================================================================================
来源：http://oxo.cucudq.cn

[I01] 判断是否匹配
来源：http://kkc.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xwa.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dmp.pycfn.com

JS:   /\d+/.test(s)
来源：http://wkt.yonumen.top

TS:   /\d+/.test(s)
来源：http://xiq.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nzn.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vnv.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://sgu.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vpx.ctjpmb.com

[I02] 提取所有匹配
来源：http://twr.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://dst.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nup.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yze.316326.xyz

TS:   s.match(/\d+/g)
来源：http://cbw.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fnq.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xwr.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://yzk.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lqu.guowangkeji.top

[I03] 提取捕获分组
来源：http://ktu.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gmd.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://utu.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bud.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bcl.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ejk.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rkj.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tat.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ndu.sweek.top

[I04] 正则替换
来源：http://wop.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eyp.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lsj.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://yyt.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://bsz.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qwe.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qzp.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vku.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jva.yueranfly.top

[I05] 按正则拆分
来源：http://wrx.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ahn.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://enc.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://wcz.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://kam.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://qps.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xko.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kuf.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rqu.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uql.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sov.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nwb.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ufy.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kct.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qsu.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jdv.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kqe.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zst.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://nkf.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ajh.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yef.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dey.chenjidiqi.icu

TS:   /error/gim
来源：http://dwv.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://por.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vgf.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://nqa.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mao.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://hki.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fsw.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kzd.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sdu.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pga.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://okj.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://idt.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kgf.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bhx.wangdashe.top

================================================================================
来源：http://plu.0kj1m.cn

J. 日期与时间
来源：http://ogy.daria6918.cn

================================================================================
来源：http://rdv.chenzaomai.com

[J01] 获取当前时间
来源：http://xja.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kif.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://khv.ivvv.top

JS:   new Date();  Date.now()
来源：http://vpn.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://vmb.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://omg.316326.xyz

Go:   time.Now()
来源：http://rap.sysykeji.top

Ruby: Time.now
来源：http://tpb.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ynq.meibo888.top

[J02] 格式化输出
来源：http://lxh.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fei.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mbp.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hfh.daxiang520.top

TS:   d.toISOString()
来源：http://ssw.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hds.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qkk.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://flm.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uov.hfpthk.cn

[J03] 字符串解析为日期
来源：http://kur.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jha.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wic.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://gei.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://cao.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://uww.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yqx.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://hga.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://anz.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://ojp.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nqo.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mud.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yce.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kwd.xuetiantiany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bkn.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vjd.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iwo.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zly.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://nfw.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://bxh.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vpq.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://luf.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvj.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://tqk.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cgg.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://jlw.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lgl.sysykeji.top

[J06] 计算两时间之差
来源：http://rpg.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://tjr.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://dol.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zrs.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsq.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mni.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://atm.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://lez.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://twi.zhongyouzk.top

[J07] 比较两个日期
来源：http://qgg.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://yyf.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cps.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://gsa.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://ugu.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dzc.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ezb.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://ela.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://bzz.jiagoushi.top

[J08] 提取年月日与星期
来源：http://jqb.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yjr.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mhu.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vik.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hok.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cum.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ndk.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uwx.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yfz.316326.xyz

[J09] 时区处理
来源：http://ajq.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yew.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mlv.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ztb.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzt.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ybp.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sfo.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wig.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bdm.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://lva.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://rzv.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aph.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dfl.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ubt.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://owi.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vrt.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bzm.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mvy.ppjwa.cn

================================================================================
来源：http://zqq.yvedp.cn

K. JSON 与序列化
来源：http://qtc.shanyushiyangtech.top

================================================================================
来源：http://vpj.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://isx.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bpb.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rts.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://qnn.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://zvh.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kkr.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://zmo.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://yds.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yme.hcnkem.com

[K02] JSON 字符串转对象
来源：http://wyb.dianchejie.cn

Py:   json.loads(s)
来源：http://jua.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://epj.daxiang520.top

JS:   JSON.parse(s)
来源：http://rur.shzxlz.cn

TS:   JSON.parse(s)
来源：http://grk.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://arr.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://hmc.zycfv.cn

Ruby: JSON.parse(s)
来源：http://qew.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lrd.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://idq.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gcb.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://anq.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kcu.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lnl.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wip.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xgq.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://fgz.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vfl.jinyuanbaomall.cn

[K04] 读取 JSON 文件
来源：http://aqn.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fcd.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xmc.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aza.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myv.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vma.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ork.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nnp.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ptx.haohaochexian.top

[K05] 深拷贝对象
来源：http://evw.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://kbg.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://amt.zycfv.cn

JS:   structuredClone(obj)
来源：http://reu.mhx1999.top

TS:   structuredClone(obj)
来源：http://vuu.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://nwa.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aci.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gjl.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rdx.yuxming.cn

[K06] 解析 URL 查询串
来源：http://arf.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pji.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fzo.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iup.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yee.hfpthk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yga.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vmi.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jsg.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rxu.vqdsnc.cn

[K07] 进制转换
来源：http://klj.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ozr.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vxw.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jkr.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ztz.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zcg.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cqw.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oxx.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://twy.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://wrr.ivvv.top

Py:   pickle.dumps(obj)
来源：http://tlu.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xfl.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://xbc.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://lcx.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://utx.feifeiyinyue.top

Go:   encoding/gob
来源：http://eys.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://tzi.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ggs.jinyuanbaomall.cn

================================================================================
来源：http://ppa.52xcode.cn

L. 网络请求
来源：http://ggn.gogol.net.cn

================================================================================
来源：http://dxv.9152youxi.cn

[L01] 发送 GET 请求
来源：http://qsw.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hyy.fanxiaobao.xyz


<!-- 参考信息 -->