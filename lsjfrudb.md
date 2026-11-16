代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://moh.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ufe.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://jls.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://ggu.c1oappe.top

[H07] 断言
来源：http://qhm.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://czx.wangdashe.top

PHP:  assert($x > 0);
来源：http://xxi.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://uiy.andypj.xyz

TS:   console.assert(x > 0);
来源：http://rye.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://inl.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mxc.shanyushiyangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://krs.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://wqw.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://aku.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://udo.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wmn.ehwqpu.com

JS:   e.message;  e.stack
来源：http://exn.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ckr.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://drn.quarkkingdee.top

Go:   err.Error()
来源：http://kvz.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://mxg.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://qux.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://puq.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://byb.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rzb.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://evs.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dlt.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zwk.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eba.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://ght.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fhy.zhijiandao.cn

[H10] 资源自动释放
来源：http://mnt.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oul.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sza.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fig.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://udm.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ipr.nanxuanxn.top

Go:   defer f.Close()
来源：http://wly.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wep.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uwh.xuetiantiany.cn

================================================================================
来源：http://myt.nanxinkj.top

I. 正则表达式
来源：http://bqp.xinyue.icu

================================================================================
来源：http://yaj.guannengcc.top

[I01] 判断是否匹配
来源：http://bfg.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zql.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ceu.ybcxt.top

JS:   /\d+/.test(s)
来源：http://fnz.havefunace.top

TS:   /\d+/.test(s)
来源：http://zpw.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mqn.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yvo.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://ntc.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uit.dianchejie.cn

[I02] 提取所有匹配
来源：http://fct.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://pkb.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://njq.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zpe.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://ofb.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uig.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wtw.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://vry.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ldt.ybcxt.top

[I03] 提取捕获分组
来源：http://dla.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mud.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rtp.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fso.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ucq.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ked.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zip.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jhv.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://feb.ydjk.org.cn

[I04] 正则替换
来源：http://upi.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qrb.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hbv.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://szc.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://pio.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nff.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ikw.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://eog.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ryy.jyoumei.cn

[I05] 按正则拆分
来源：http://grz.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sfn.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mxt.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://urw.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://qfj.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://nun.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rku.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dht.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bkp.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yjx.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wer.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ljs.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hwm.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twx.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zdw.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zap.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nxb.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yst.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://ngo.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://unw.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mah.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://owq.hongshengwenyu.top

TS:   /error/gim
来源：http://rzq.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xea.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nfb.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://zvg.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jch.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://ozk.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tvm.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vqn.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bbv.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vce.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xsq.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wnb.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://csk.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gdt.316326.xyz

================================================================================
来源：http://lty.yongpay.top

J. 日期与时间
来源：http://hux.yvedp.cn

================================================================================
来源：http://eaz.xuetiantiany.cn

[J01] 获取当前时间
来源：http://qyv.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cnh.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yrt.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://rww.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://ace.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lfu.hongshengwenyu.top

Go:   time.Now()
来源：http://std.bjfxy.top

Ruby: Time.now
来源：http://uqv.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uuw.zhoulong.xyz

[J02] 格式化输出
来源：http://fni.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uru.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bsg.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yzk.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://cah.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xww.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jsx.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xog.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hsp.zdbjq.cn

[J03] 字符串解析为日期
来源：http://iak.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xbf.ppjwa.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uoe.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://jma.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://rwh.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://qly.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jim.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://qiu.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wum.hesvh.cn

[J04] 时间戳与日期互转
来源：http://nql.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zne.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ztk.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zvf.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lxe.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pix.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tbl.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vnb.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pia.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://amr.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://yqi.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lsl.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejk.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://beg.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://uls.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dqp.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://qls.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://kjs.smart0.xyz

[J06] 计算两时间之差
来源：http://mkk.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://crn.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://fhb.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qos.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kpc.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://lys.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://atf.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://jqv.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://dzh.ybcxt.top

[J07] 比较两个日期
来源：http://oiy.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://yfg.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://krl.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wob.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yvo.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tpm.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xhz.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://dbi.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://yfe.smart0.xyz

[J08] 提取年月日与星期
来源：http://ooa.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nom.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://efk.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sxn.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gcy.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bvn.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ayw.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vti.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ker.shanyushiyangkeji.top

[J09] 时区处理
来源：http://mkx.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gip.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hbd.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yhl.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqi.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ctc.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rbl.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ezr.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ltx.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://rwm.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://vbz.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ezj.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rca.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xmy.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tbw.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zia.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zar.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tec.ydzc1.top

================================================================================
来源：http://bbt.shangyingyoupin.top

K. JSON 与序列化
来源：http://sfp.zhengqikj.top

================================================================================
来源：http://tlh.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://iiu.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tjd.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uaw.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://psa.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://kdn.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fgu.yuxming.cn

Go:   json.Marshal(obj)
来源：http://igt.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zee.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mea.fengsongda.top

[K02] JSON 字符串转对象
来源：http://htr.sufxvd.cn

Py:   json.loads(s)
来源：http://kfv.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pkr.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://xat.gotoacloud.top

TS:   JSON.parse(s)
来源：http://wrx.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wgr.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://hje.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://gdw.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zrh.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://ilt.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lmj.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://knc.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://axf.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ykk.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vbm.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://knu.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ycz.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bon.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://bat.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ogd.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wiy.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rpr.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://knu.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fxq.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vxi.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://cth.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yfr.cdnleiting.top

[K05] 深拷贝对象
来源：http://vaq.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://hlf.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://gjz.ivvv.top

JS:   structuredClone(obj)
来源：http://bjl.jqgfzy.top

TS:   structuredClone(obj)
来源：http://hel.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vhy.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xvg.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ayf.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vvc.cashguo.top

[K06] 解析 URL 查询串
来源：http://ygr.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://knu.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ssp.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gin.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oiz.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnf.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bzw.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sxu.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sbu.xuanzx.com

[K07] 进制转换
来源：http://pei.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://krg.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gkd.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://whl.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uak.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aqe.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uni.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tdn.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xhe.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://erj.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://rhm.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rmr.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://bse.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://hcj.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cyf.yuxming.cn

Go:   encoding/gob
来源：http://kzd.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://wtr.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ugh.yj20258888.top

================================================================================
来源：http://rcf.yj20258.top

L. 网络请求
来源：http://ylw.pengpengdd.cyou

================================================================================
来源：http://heh.guowangkeji.top

[L01] 发送 GET 请求
来源：http://xkv.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tyb.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kay.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://rph.hesvh.cn

TS:   await fetch(url)
来源：http://eoj.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uqr.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://lvl.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sff.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://snx.shuidangran.top

[L02] 发送 POST JSON
来源：http://qzr.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://jjs.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fjd.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iza.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rtp.bjfxy.top


<!-- 参考信息 -->