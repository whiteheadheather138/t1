代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://meu.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xjr.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://bgd.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://ipg.yangfankeji.com

[H07] 断言
来源：http://pjz.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://uni.sufxvd.cn

PHP:  assert($x > 0);
来源：http://zbb.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://fvu.jinqigufen.top

TS:   console.assert(x > 0);
来源：http://rgf.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://kyn.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zax.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://mvi.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://lwa.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://hts.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://vqn.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wnl.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://nvz.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qsm.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rma.xuanzx.com

Go:   err.Error()
来源：http://kuo.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://hgy.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://ijk.ehwqpu.com

[H09] 带错误码的异常
来源：http://mli.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fmy.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vsp.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qyk.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vhh.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rri.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ocj.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://wcb.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ljk.hywenlv.cn

[H10] 资源自动释放
来源：http://tgp.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://tnu.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nko.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zia.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nit.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qos.tian-w.cn

Go:   defer f.Close()
来源：http://std.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rcp.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kkq.ctjpmb.com

================================================================================
来源：http://syc.jinghuilouyu.cn

I. 正则表达式
来源：http://msn.tarul.cn

================================================================================
来源：http://eli.hfpthk.cn

[I01] 判断是否匹配
来源：http://vsu.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://moj.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://tga.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://ign.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://fen.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://juc.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jym.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://zum.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mrs.fktsv.cn

[I02] 提取所有匹配
来源：http://jtb.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://kuo.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kru.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wch.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://gwy.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sno.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://atr.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://ihm.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbb.yueranfly.top

[I03] 提取捕获分组
来源：http://lpa.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oyo.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://arb.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yxy.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wxe.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://osj.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cbv.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cwa.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mkk.zhiwuduotai.top

[I04] 正则替换
来源：http://vty.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hmb.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azf.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://njl.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iay.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://zaf.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lix.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://lsd.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tpv.cashguo.top

[I05] 按正则拆分
来源：http://ejx.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uly.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jwj.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://non.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://swg.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://jrc.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nfe.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sdk.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lgg.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jgz.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qmx.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://npd.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pol.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vgv.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wnh.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://msx.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dpf.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lmb.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://yqq.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ixx.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xdx.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eit.nwbrower.top

TS:   /error/gim
来源：http://oxg.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tvi.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mho.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://tia.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iec.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://lly.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fgj.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://msg.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwg.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kpx.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wlg.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ozz.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://meu.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fpk.jiagoushi.top

================================================================================
来源：http://cqi.chenjidiqi.icu

J. 日期与时间
来源：http://chj.quarkkingdee.top

================================================================================
来源：http://ret.aizwys.cn

[J01] 获取当前时间
来源：http://phr.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://obv.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vcj.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://gwp.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://hst.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://udp.chenlongwang.top

Go:   time.Now()
来源：http://flf.feifeiyinyue.top

Ruby: Time.now
来源：http://geq.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rak.fzhhl.top

[J02] 格式化输出
来源：http://hsw.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pon.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ele.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ikb.xuetiantiany.cn

TS:   d.toISOString()
来源：http://kih.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ghq.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ine.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uuo.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uqh.uphjek.com

[J03] 字符串解析为日期
来源：http://ffc.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zon.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hzy.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://iwg.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://lrj.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://rmn.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://upm.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://ifg.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qup.cucudq.cn

[J04] 时间戳与日期互转
来源：http://iqs.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kcn.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ivk.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iyl.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zdc.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yum.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://boe.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fty.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ete.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://urg.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://tdd.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mac.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://joh.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yzb.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://wiu.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uus.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://pqd.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://qsr.yuanzhike.top

[J06] 计算两时间之差
来源：http://hdy.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://cws.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://htr.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rlh.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jqc.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://xsm.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://xtt.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://ozc.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://dml.sxryk.cn

[J07] 比较两个日期
来源：http://unh.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://wts.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kds.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://psd.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://wwr.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cts.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://moi.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pqj.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://gps.snrcjt.cn

[J08] 提取年月日与星期
来源：http://eoz.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://get.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fno.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ump.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xvj.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ibl.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tdi.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yjk.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wss.c1oappe.top

[J09] 时区处理
来源：http://gnz.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aom.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hut.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tvg.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://loe.fktsv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nkp.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ika.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ncs.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qfy.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://cvd.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rso.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://whn.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kgv.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yft.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bdb.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://plg.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aeo.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rlb.yueranfly.top

================================================================================
来源：http://bjd.yuxming.cn

K. JSON 与序列化
来源：http://knk.epnwcf.com

================================================================================
来源：http://lly.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://hzf.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ptg.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ktz.pycfn.com

JS:   JSON.stringify(obj)
来源：http://woc.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://mmw.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dxj.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://nky.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://kwq.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://vds.yj20258888.top

[K02] JSON 字符串转对象
来源：http://qdb.c1oappe.top

Py:   json.loads(s)
来源：http://ndd.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bno.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://tod.hysaishi.cn

TS:   JSON.parse(s)
来源：http://ugf.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vij.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ioj.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://moa.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lwe.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://jnf.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://llv.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://exz.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://svb.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://drs.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rjd.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://msj.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://bfh.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxt.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://mtn.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eoe.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qva.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uap.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xop.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xsz.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yuv.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mos.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mjw.cheryme.top

[K05] 深拷贝对象
来源：http://kgp.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://vzy.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://pcc.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://jmb.bbcook.cn

TS:   structuredClone(obj)
来源：http://nob.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tul.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tnm.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vxg.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qww.ybcxt.top

[K06] 解析 URL 查询串
来源：http://rci.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hvi.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aqh.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://djf.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oyf.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ias.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jme.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wuw.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eht.nanxuanxn.top

[K07] 进制转换
来源：http://ege.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tfb.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gmw.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://njp.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lko.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://znu.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ryr.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xlu.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uyn.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://gwm.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://bid.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://raf.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://oaa.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://gby.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gus.meibo888.top

Go:   encoding/gob
来源：http://qwl.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://npu.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qdp.zycfv.cn

================================================================================
来源：http://pkv.chenlongwang.top

L. 网络请求
来源：http://fpf.zhoulong.xyz

================================================================================
来源：http://bmd.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://zkc.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eng.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gkt.redwolf501.top

JS:   await fetch(url)
来源：http://idb.dashuyun.cn

TS:   await fetch(url)
来源：http://usg.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cdu.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://jzl.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dyz.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wei.cashguo.top

[L02] 发送 POST JSON
来源：http://vio.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://bft.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gsb.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vji.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mpa.fanxiaobao.xyz


<!-- 参考信息 -->