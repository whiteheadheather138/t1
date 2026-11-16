代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xsv.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uru.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://aoc.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://vru.hongshengwenyu.top

[H07] 断言
来源：http://cix.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://zve.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://ose.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://zxf.hesvh.cn

TS:   console.assert(x > 0);
来源：http://wax.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://nbn.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wwd.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yhp.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://nfn.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://qna.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://aoi.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sqd.yonumen.top

JS:   e.message;  e.stack
来源：http://col.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://saq.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qet.andypj.xyz

Go:   err.Error()
来源：http://zue.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://hku.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://hvk.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://oab.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jvu.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jyt.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cxf.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uxf.vehdjk.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://utu.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dnw.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://nqx.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aga.ivvv.top

[H10] 资源自动释放
来源：http://ect.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://phv.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uby.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rzt.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mmk.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xko.hammf.cn

Go:   defer f.Close()
来源：http://rhi.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zsv.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qkb.jianghu66.top

================================================================================
来源：http://fal.zhixingplan.top

I. 正则表达式
来源：http://nut.hysaishi.cn

================================================================================
来源：http://trj.yueranfly.top

[I01] 判断是否匹配
来源：http://ach.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zrh.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://htu.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://was.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://zws.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xxk.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://npf.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://whl.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wsr.ehwqpu.com

[I02] 提取所有匹配
来源：http://wfk.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://nzb.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aqx.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://avn.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://cwz.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nux.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hdn.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://pwh.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://btu.ybcxt.top

[I03] 提取捕获分组
来源：http://gyg.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ahr.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://val.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kip.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fzo.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mmt.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://enu.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gnu.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ojp.sjlbkw.cn

[I04] 正则替换
来源：http://zzj.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ywz.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://clt.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://bcn.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://uyo.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://cnu.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hmx.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qye.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lkf.ivvv.top

[I05] 按正则拆分
来源：http://tzd.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lmq.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bri.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://hsp.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://noc.jinghuilouyu.cn

Java: s.split("\\s*,\\s*")
来源：http://tew.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uoj.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tyi.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cbg.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vfo.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://imy.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://byv.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kmv.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pjs.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vib.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ivn.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rva.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vix.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://idq.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://msp.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://roe.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://unx.guannengcc.top

TS:   /error/gim
来源：http://crf.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yid.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://toe.yonumen.top

Ruby: s.scan(/error/i)
来源：http://wpd.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xrf.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://okv.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wwg.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xkv.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ljd.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tjv.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lua.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sif.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eni.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cgx.feifeiyinyue.top

================================================================================
来源：http://lpu.yuxming.cn

J. 日期与时间
来源：http://new.ybcxt.top

================================================================================
来源：http://yqe.dianchejie.cn

[J01] 获取当前时间
来源：http://paz.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nva.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uwl.sufxvd.cn

JS:   new Date();  Date.now()
来源：http://rrr.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://jlu.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://suj.zhoulong.xyz

Go:   time.Now()
来源：http://gcw.vqdsnc.cn

Ruby: Time.now
来源：http://xqz.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://igk.hcnkem.com

[J02] 格式化输出
来源：http://otz.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vta.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mas.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mxv.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://yyl.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://emr.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yvj.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aly.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vkp.zhengqikj.top

[J03] 字符串解析为日期
来源：http://onm.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fbq.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aue.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://lyj.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://cfn.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://jwg.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://apz.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://mia.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ndf.meibo888.top

[J04] 时间戳与日期互转
来源：http://npp.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tij.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yzx.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ret.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ubv.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bet.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ibc.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://syh.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://diu.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://sgw.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://ylo.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eqq.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yba.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zhz.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://ife.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lpx.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://ftq.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rci.bbcook.cn

[J06] 计算两时间之差
来源：http://cqa.hammf.cn

Py:   (end - start).total_seconds()
来源：http://drw.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://jgk.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jfn.sufxvd.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://klt.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://hor.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://jpi.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://tzy.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://bkh.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://qhg.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://hmc.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vur.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://asu.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://tyi.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bro.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jjq.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://cxx.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://bby.sxryk.cn

[J08] 提取年月日与星期
来源：http://mmm.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fhd.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mda.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lku.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bqx.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nys.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sly.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gyp.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ogj.ywan-chungtsiang.top

[J09] 时区处理
来源：http://cos.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tqb.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cja.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jrz.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ukj.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ucl.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://umv.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://hyl.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dli.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://ebo.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ygi.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gee.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://abg.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iiw.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://noh.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vzh.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sid.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qcp.ydjk.org.cn

================================================================================
来源：http://anf.shzxlz.cn

K. JSON 与序列化
来源：http://gng.jqgufenzy.top

================================================================================
来源：http://wbq.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://kuf.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wgx.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kcd.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://yee.yj20258.top

TS:   JSON.stringify(obj)
来源：http://yvj.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pwx.yueranfly.top

Go:   json.Marshal(obj)
来源：http://amt.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://prj.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zvv.tarul.cn

[K02] JSON 字符串转对象
来源：http://fok.bjfxy.top

Py:   json.loads(s)
来源：http://zmg.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mxy.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://lnb.zdbjq.cn

TS:   JSON.parse(s)
来源：http://nhh.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ywo.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://ynt.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://gao.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wdu.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://vls.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ajw.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qii.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wwt.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jcx.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wzh.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://diy.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://irc.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://whp.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://olp.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ytb.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vbj.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pxm.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sjh.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://duw.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yqp.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ptt.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://myc.tianlin.xyz

[K05] 深拷贝对象
来源：http://wma.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://glr.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://pvv.daxiang520.top

JS:   structuredClone(obj)
来源：http://zic.aibaodan.cn

TS:   structuredClone(obj)
来源：http://yed.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rag.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vhq.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://slj.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fdb.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://qwv.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jby.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jrc.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://plx.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://psy.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vya.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xbz.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cgp.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ftn.hysaishi.cn

[K07] 进制转换
来源：http://tns.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pdf.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hes.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uwe.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lyh.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eyw.gzhubu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jov.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://esn.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oiq.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://abz.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://xtu.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dzl.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://ryf.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://tsf.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nku.wangshuangyany.cn

Go:   encoding/gob
来源：http://cbv.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://ast.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rfz.jianghu66.top

================================================================================
来源：http://ywf.smart0.xyz

L. 网络请求
来源：http://oqj.gzhubu.top

================================================================================
来源：http://slu.shuidangran.top

[L01] 发送 GET 请求
来源：http://pli.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lna.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tut.xuanzx.com

JS:   await fetch(url)
来源：http://omg.yueranfly.top

TS:   await fetch(url)
来源：http://khz.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zio.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://qzt.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ota.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jmh.hywenlv.cn

[L02] 发送 POST JSON
来源：http://fzk.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lyd.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zpr.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dsj.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ieg.cucudq.cn


<!-- 参考信息 -->