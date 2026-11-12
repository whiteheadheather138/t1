代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mbi.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fpq.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://yvv.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://fms.sweek.top

[H07] 断言
来源：http://lgr.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://dnt.fktsv.cn

PHP:  assert($x > 0);
来源：http://idg.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://eai.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://dmf.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://yfn.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xch.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cls.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://agf.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://smj.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://orf.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oth.andypj.xyz

JS:   e.message;  e.stack
来源：http://vdu.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vow.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zik.zhiwuduotai.top

Go:   err.Error()
来源：http://uxn.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://tmz.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://dfp.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://epr.mhx1999.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xqm.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jue.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://txn.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ffj.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qbh.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hfe.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://jkr.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aio.cheryme.top

[H10] 资源自动释放
来源：http://dib.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://taf.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oja.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mvy.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ntr.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xcr.yongpay.top

Go:   defer f.Close()
来源：http://vfd.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hnu.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pph.havefunace.top

================================================================================
来源：http://uts.yonumen.top

I. 正则表达式
来源：http://zei.tian-w.cn

================================================================================
来源：http://taj.dashuyun.cn

[I01] 判断是否匹配
来源：http://kub.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uhg.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://plv.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://tuc.sxryk.cn

TS:   /\d+/.test(s)
来源：http://dyr.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aut.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nub.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://ekw.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jsd.yfazqb.com

[I02] 提取所有匹配
来源：http://avk.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://bzk.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rac.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kiv.hongshengwenyu.top

TS:   s.match(/\d+/g)
来源：http://pdy.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vcn.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nbz.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://jmy.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zmi.hnqzz.top

[I03] 提取捕获分组
来源：http://luh.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://suj.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://udg.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uzn.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wws.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tbr.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qrt.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ves.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vfa.cucudq.cn

[I04] 正则替换
来源：http://wit.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pqe.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://huw.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://kno.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zsj.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://cgf.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://khd.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jfy.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eeu.52xcode.cn

[I05] 按正则拆分
来源：http://qig.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nqj.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ubm.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://txx.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ppu.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://iql.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dtg.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://wfx.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tmk.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mzp.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qzr.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dgn.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdj.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghy.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cei.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lka.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ren.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nts.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://xde.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kie.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nls.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pyx.sweek.top

TS:   /error/gim
来源：http://piu.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zkr.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gdr.pycfn.com

Ruby: s.scan(/error/i)
来源：http://zla.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ehq.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://pvb.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nwc.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ddl.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wtg.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eof.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cjw.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rtp.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oey.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jdd.9152youxi.cn

================================================================================
来源：http://abj.gotoacloud.top

J. 日期与时间
来源：http://afj.shangyingyoupin.top

================================================================================
来源：http://gzv.c1oappe.top

[J01] 获取当前时间
来源：http://xce.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bvr.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://asg.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://frt.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://qxe.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://xwu.vqdsnc.cn

Go:   time.Now()
来源：http://xgw.yuxming.cn

Ruby: Time.now
来源：http://hnr.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xnh.yj20258888.top

[J02] 格式化输出
来源：http://lun.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dxn.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://enr.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kew.nwbrower.top

TS:   d.toISOString()
来源：http://hxj.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://egv.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fbi.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ezl.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zjf.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://zvk.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gts.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://imh.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://bdn.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://oew.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vyg.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pii.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://ahs.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nby.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://spz.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rlq.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://itl.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xpy.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qmo.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sms.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hlx.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xfx.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ogw.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://oei.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://dgb.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zsf.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkm.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rvw.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://sss.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://grx.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://lxr.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://see.cheryme.top

[J06] 计算两时间之差
来源：http://bep.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://vhn.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://glq.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wsy.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jms.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://mji.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://mmj.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://thu.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://dml.jyoumei.cn

[J07] 比较两个日期
来源：http://nan.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://mfe.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qkz.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://tzy.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qaz.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zjx.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zff.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://qha.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://ilh.c1oappe.top

[J08] 提取年月日与星期
来源：http://lxq.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yob.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hxq.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qlc.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cuv.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hvb.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tyl.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lxm.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bre.jinyuanbaomall.cn

[J09] 时区处理
来源：http://jbu.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cqd.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wbf.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qjf.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zla.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hmg.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ngi.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iyk.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bqe.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://sbv.shanyushiyangtech.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ixq.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hzj.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hll.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sxa.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mtl.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ngj.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://idn.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dvq.fktsv.cn

================================================================================
来源：http://pml.jyoumei.cn

K. JSON 与序列化
来源：http://for.vqdsnc.cn

================================================================================
来源：http://blh.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://wbc.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zeq.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oyq.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://vjc.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://vrd.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eir.yuxming.cn

Go:   json.Marshal(obj)
来源：http://ffv.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://yco.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ktf.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://mlf.yuanzhike.top

Py:   json.loads(s)
来源：http://aol.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfc.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://xmb.xuanzx.com

TS:   JSON.parse(s)
来源：http://wti.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hel.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://zah.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://dgs.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ufd.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://bgo.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uof.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cmb.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ymc.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lfi.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lmj.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://auk.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://swj.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ctj.fehbvm.com

[K04] 读取 JSON 文件
来源：http://bct.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://afb.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://izu.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uun.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blm.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ucv.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gta.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://chc.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fzt.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://opv.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://qfq.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://zha.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://rtq.ivvv.top

TS:   structuredClone(obj)
来源：http://ect.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bfq.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ffb.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://prv.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hkj.sweek.top

[K06] 解析 URL 查询串
来源：http://dwm.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zry.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yyc.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://isw.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ium.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rcw.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gxh.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nrw.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jht.yongpay.top

[K07] 进制转换
来源：http://yhr.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://thq.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ykq.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sfn.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rsn.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cwh.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fwn.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pfp.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rax.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://hos.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://mkc.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://boh.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://bgi.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://ruj.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wdp.daria6918.cn

Go:   encoding/gob
来源：http://zhe.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://ouv.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ikl.cashguo.top

================================================================================
来源：http://anu.fengsongda.top

L. 网络请求
来源：http://ivd.daxiang520.top

================================================================================
来源：http://pek.bbcook.cn

[L01] 发送 GET 请求
来源：http://ppx.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wsd.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qdd.svipenyu.cn

JS:   await fetch(url)
来源：http://uxp.tian-w.cn

TS:   await fetch(url)
来源：http://luw.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kcj.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://gop.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://czw.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wqv.hammf.cn

[L02] 发送 POST JSON
来源：http://qwz.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://xbd.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aoz.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hid.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bra.zycfv.cn


<!-- 参考信息 -->