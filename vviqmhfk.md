代发 wailian999

Py:   value = d.get("k") or default
来源：http://cnz.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://kof.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rjz.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://dpp.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zgf.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oho.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://zxa.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://fvh.chenzaomai.com

[H07] 断言
来源：http://pyt.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://kot.birdmap.top

PHP:  assert($x > 0);
来源：http://ymm.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://ecn.fengsongda.top

TS:   console.assert(x > 0);
来源：http://frz.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://esd.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bsb.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://qdn.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://vlv.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://jpy.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://abm.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mnd.jyoumei.cn

JS:   e.message;  e.stack
来源：http://hxd.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uqb.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sux.yangfankeji.com

Go:   err.Error()
来源：http://ody.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://swh.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://hti.yj202588.top

[H09] 带错误码的异常
来源：http://mxi.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ofi.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ohq.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://inx.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gqh.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tyo.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qom.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://jtx.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vly.pycfn.com

[H10] 资源自动释放
来源：http://izb.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ive.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hhe.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dlx.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lau.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sdp.pengpengdd.cyou

Go:   defer f.Close()
来源：http://ilu.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xyg.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rye.zhaomingkeji.xyz

================================================================================
来源：http://vnm.jianghu66.top

I. 正则表达式
来源：http://qiw.tianlin.xyz

================================================================================
来源：http://toq.ehwqpu.com

[I01] 判断是否匹配
来源：http://dzs.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hlb.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://shb.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://rtb.yueranfly.top

TS:   /\d+/.test(s)
来源：http://djn.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://brw.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vpu.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://rcq.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hfz.9152youxi.cn

[I02] 提取所有匹配
来源：http://ajs.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://nmx.jinyuanbaomall.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tek.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezu.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://pba.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dqg.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://igz.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://vth.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yuf.svipenyu.cn

[I03] 提取捕获分组
来源：http://irt.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rwp.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nzb.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lch.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qty.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kud.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qxv.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tyr.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gls.hongshengwenyu.top

[I04] 正则替换
来源：http://nyd.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zvt.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pph.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://uxa.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fwz.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://fnz.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://rcj.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zee.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hse.zhoulong.xyz

[I05] 按正则拆分
来源：http://zjz.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://bay.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zbc.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://npf.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://cth.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://for.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pza.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://zfw.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rii.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hce.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hoa.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bbz.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ikv.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ubo.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://skm.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sns.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jxd.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pte.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://kgw.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sha.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://shr.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zrv.epnwcf.com

TS:   /error/gim
来源：http://njy.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yqb.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eou.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://duj.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://afg.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://vzk.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ecl.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ogq.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwm.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://frk.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jju.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nvb.shanyushiyangtech.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qpa.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nwh.sxryk.cn

================================================================================
来源：http://lpy.fktsv.cn

J. 日期与时间
来源：http://qff.hywenlv.cn

================================================================================
来源：http://nlt.guannengcc.top

[J01] 获取当前时间
来源：http://sdw.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gdx.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dye.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://mzl.cucudq.cn

TS:   new Date();  Date.now()
来源：http://uxu.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mxt.kuanghao11.cn

Go:   time.Now()
来源：http://giy.fehbvm.com

Ruby: Time.now
来源：http://miu.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gle.wangshuangyany.cn

[J02] 格式化输出
来源：http://gbr.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gwy.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xdd.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ugc.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://qym.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mxy.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oxt.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqq.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cha.meibo888.top

[J03] 字符串解析为日期
来源：http://lww.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://djn.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://elq.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://wvh.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://lku.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ypa.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kcg.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://khh.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lwf.yj20258.top

[J04] 时间戳与日期互转
来源：http://xca.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gxe.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://irl.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jux.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yus.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nen.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qut.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yfd.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://erq.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://urh.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://oxb.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nth.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dnv.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jki.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://oua.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gno.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://hvc.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://wng.aibaodan.cn

[J06] 计算两时间之差
来源：http://haa.birdmap.top

Py:   (end - start).total_seconds()
来源：http://agf.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://qij.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oqo.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ddi.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://teo.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://auz.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://uga.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://huo.xinyue.icu

[J07] 比较两个日期
来源：http://hfh.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://obu.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nlo.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://woo.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gmx.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ytd.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wyy.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lfk.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://ytu.ehwqpu.com

[J08] 提取年月日与星期
来源：http://dky.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tdb.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wqm.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qsq.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fhl.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pcs.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xhr.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ude.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fjw.hcnkem.com

[J09] 时区处理
来源：http://vvj.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://axg.zhiwuduotai.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mqy.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ypj.zdqjudy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpq.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gge.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oyt.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eyd.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://adu.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://zjz.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jvh.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cwx.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vkt.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pcy.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cco.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tsg.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tna.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://irc.9152youxi.cn

================================================================================
来源：http://tif.zhoulong.xyz

K. JSON 与序列化
来源：http://rak.smart0.xyz

================================================================================
来源：http://nan.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://dvg.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pmc.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ary.tarul.cn

JS:   JSON.stringify(obj)
来源：http://ydx.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://xbc.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cly.52xcode.cn

Go:   json.Marshal(obj)
来源：http://hwt.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://wfk.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://unl.aizwys.cn

[K02] JSON 字符串转对象
来源：http://uiz.jlsjyb.cn

Py:   json.loads(s)
来源：http://mzp.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rst.hnqzz.top

JS:   JSON.parse(s)
来源：http://bgl.fehbvm.com

TS:   JSON.parse(s)
来源：http://tup.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wxk.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://tpn.bjfxy.top

Ruby: JSON.parse(s)
来源：http://bip.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pwf.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://uqo.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fbm.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cyy.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cza.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uhu.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kxe.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dta.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://giw.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://btg.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://lrq.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pir.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vng.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ixr.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynt.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mxx.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://byz.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://oey.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bsf.yfazqb.com

[K05] 深拷贝对象
来源：http://qqr.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://kqz.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://ikf.fehbvm.com

JS:   structuredClone(obj)
来源：http://kxk.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://iiu.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wzf.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://juv.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tkt.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vvy.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://evx.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vta.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yrc.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yzp.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hah.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eyn.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://psy.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yhx.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://diw.jinqigufen.top

[K07] 进制转换
来源：http://nfm.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cam.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xwb.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pug.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zqd.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wbx.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://svl.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fvv.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lxi.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://gvj.tarul.cn

Py:   pickle.dumps(obj)
来源：http://xrq.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jum.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://fun.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://cly.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jaq.shangyingyoupin.top

Go:   encoding/gob
来源：http://xgc.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://kbv.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ssf.redwolf501.top

================================================================================
来源：http://fus.sufxvd.cn

L. 网络请求
来源：http://tgy.meibo888.top

================================================================================
来源：http://dfx.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://bpk.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aii.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qlk.yvedp.cn

JS:   await fetch(url)
来源：http://yeq.yuxming.cn

TS:   await fetch(url)
来源：http://yug.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wjl.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://fnh.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tkl.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ikh.52xcode.cn

[L02] 发送 POST JSON
来源：http://gct.zhengqikj.top


<!-- 参考信息 -->