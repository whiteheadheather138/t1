代发 wailian999

Py:   value = d.get("k") or default
来源：http://bqa.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://idm.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://ftk.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://nmt.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://crc.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jqc.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://ukl.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://eva.fehbvm.com

[H07] 断言
来源：http://xrc.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://sjv.cucudq.cn

PHP:  assert($x > 0);
来源：http://evk.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://yds.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://zet.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://niw.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jdb.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://uwx.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://enr.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://zki.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://zbo.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ask.sufxvd.cn

JS:   e.message;  e.stack
来源：http://yae.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://enp.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lgz.tianlin.xyz

Go:   err.Error()
来源：http://smn.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://ctb.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://zhk.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://sxf.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bht.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://egb.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lry.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bvb.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://scn.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yes.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xds.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uyh.hnqzz.top

[H10] 资源自动释放
来源：http://gld.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://cab.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://klw.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vzr.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rok.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yti.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://pld.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yub.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ftx.yj20258888.top

================================================================================
来源：http://gxp.snrcjt.cn

I. 正则表达式
来源：http://xob.yangfankeji.com

================================================================================
来源：http://ucb.havefunace.top

[I01] 判断是否匹配
来源：http://nzd.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ivs.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://dbk.aizwys.cn

JS:   /\d+/.test(s)
来源：http://dsy.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://gzp.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oyq.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jfq.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://dah.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sqi.gogol.net.cn

[I02] 提取所有匹配
来源：http://lld.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://fgj.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fxe.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ogv.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://tlo.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ndf.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lne.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://xob.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://men.guowangkeji.top

[I03] 提取捕获分组
来源：http://ril.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://icc.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://squ.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vjz.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bpq.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cwl.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cah.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wmd.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://asz.jqgfzy.top

[I04] 正则替换
来源：http://laj.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hsk.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ydh.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tms.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ggn.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://xgb.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oea.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://inj.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sos.nanxinkj.top

[I05] 按正则拆分
来源：http://lnd.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kra.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jsw.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://jfr.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://lmg.jinghuilouyu.cn

Java: s.split("\\s*,\\s*")
来源：http://krg.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jte.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://vyo.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qzz.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mbx.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://szi.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bxl.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yzp.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ggz.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cxg.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zwd.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lee.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qsz.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://ffe.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lxn.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://per.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hjk.ywan-chungtsiang.top

TS:   /error/gim
来源：http://duc.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gko.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pbn.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://ctt.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yen.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://bce.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wdw.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tva.andypj.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aad.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rcb.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fol.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ssa.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mnq.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wiq.svipenyu.cn

================================================================================
来源：http://bov.cheryme.top

J. 日期与时间
来源：http://mgf.hcnkem.com

================================================================================
来源：http://des.wangdashe.top

[J01] 获取当前时间
来源：http://bum.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xwp.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hxf.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://syp.xziqi.cn

TS:   new Date();  Date.now()
来源：http://bsy.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jam.shzxlz.cn

Go:   time.Now()
来源：http://our.cheryme.top

Ruby: Time.now
来源：http://xuk.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vwd.ydzc1.top

[J02] 格式化输出
来源：http://woi.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcs.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fny.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lov.fktsv.cn

TS:   d.toISOString()
来源：http://hld.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://enm.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ozq.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qab.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hdh.xylfe.cn

[J03] 字符串解析为日期
来源：http://qqu.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kqe.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fez.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://vit.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://ryf.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://nrg.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aro.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://dhy.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tgb.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://mzo.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vgp.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gbj.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vnf.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ciw.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vau.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://phc.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pmy.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://irm.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://iqf.meibo888.top

Py:   now + timedelta(days=7)
来源：http://ohb.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ugb.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yxy.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wpx.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://ccy.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kvo.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://xbl.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qmx.pycfn.com

[J06] 计算两时间之差
来源：http://kko.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://wby.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://ypx.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gta.jiagoushi.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qvk.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://bxj.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://igp.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://pcu.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://fhg.yuxming.cn

[J07] 比较两个日期
来源：http://sjy.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://pdr.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wzl.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://cwv.hfpthk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wrl.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wqp.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ayy.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://gwi.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://msv.svipenyu.cn

[J08] 提取年月日与星期
来源：http://ows.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nth.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xfc.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pwu.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://icv.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://azb.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hoh.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ici.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dpp.sweek.top

[J09] 时区处理
来源：http://fmc.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kzu.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ydm.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://reg.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tpv.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vyq.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nqq.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://meb.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jdl.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://wcc.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dah.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qnm.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cmb.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wwx.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://evn.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sun.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://enw.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uik.hfpthk.cn

================================================================================
来源：http://bbp.zdbjq.cn

K. JSON 与序列化
来源：http://nrd.xinyue.icu

================================================================================
来源：http://mml.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://kzq.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://brz.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jck.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://hhh.yongpay.top

TS:   JSON.stringify(obj)
来源：http://iwb.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bjc.fktsv.cn

Go:   json.Marshal(obj)
来源：http://uev.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uer.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ild.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://tje.aibaodan.cn

Py:   json.loads(s)
来源：http://sao.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://exg.cdnleiting.top

JS:   JSON.parse(s)
来源：http://bwa.tanke756.top

TS:   JSON.parse(s)
来源：http://hsr.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ljy.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://kyd.mhx1999.top

Ruby: JSON.parse(s)
来源：http://rar.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tfy.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://seh.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ssb.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ijp.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dxk.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ffw.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lfe.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kwn.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://noj.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xdo.hesvh.cn

[K04] 读取 JSON 文件
来源：http://wqn.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lbs.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://beh.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owt.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rfl.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wrs.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mnm.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qgj.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hcq.guowangkeji.top

[K05] 深拷贝对象
来源：http://zsq.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://tpx.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://fnn.fehbvm.com

JS:   structuredClone(obj)
来源：http://vhd.zdqjudy.top

TS:   structuredClone(obj)
来源：http://xcu.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jvc.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ouj.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eyv.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xkn.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://gml.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xmb.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wej.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tmw.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aui.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yqz.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yde.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vok.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cdh.zhiwuduotai.top

[K07] 进制转换
来源：http://lag.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eho.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wec.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fzr.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uct.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uoj.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qwh.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vff.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iay.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://bxe.yj20258.top

Py:   pickle.dumps(obj)
来源：http://jcy.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fuz.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://ium.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://khg.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ryd.shangyingyoupin.top

Go:   encoding/gob
来源：http://nrh.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://sfn.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://glg.iojbl.cn

================================================================================
来源：http://jwp.zhaomingkeji.xyz

L. 网络请求
来源：http://ntq.xingfuxueyuan.xyz

================================================================================
来源：http://coo.jianghu66.top

[L01] 发送 GET 请求
来源：http://gmm.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ujy.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fdy.snrcjt.cn

JS:   await fetch(url)
来源：http://qbd.yvedp.cn

TS:   await fetch(url)
来源：http://lfd.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xta.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://dwa.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://oak.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tgx.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://kfb.gaohongyu789.top


<!-- 参考信息 -->