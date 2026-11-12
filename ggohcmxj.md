代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://tlt.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://evk.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://wzj.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qiz.yongpay.top

JS:   e.message;  e.stack
来源：http://adb.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mlb.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pva.aizwys.cn

Go:   err.Error()
来源：http://vnw.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://guk.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://qlk.cashguo.top

[H09] 带错误码的异常
来源：http://ujd.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oay.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wgt.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://giu.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rqz.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wah.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gjy.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tru.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bys.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://smo.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mwx.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pup.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://srj.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rkp.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://osz.hcnkem.com

Go:   defer f.Close()
来源：http://roy.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jfa.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qvb.jlsjyb.cn

================================================================================
来源：http://wmh.hfpthk.cn

I. 正则表达式
来源：http://zzj.vehdjk.com

================================================================================
来源：http://big.shzxlz.cn

[I01] 判断是否匹配
来源：http://rab.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dly.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://nar.tian-w.cn

JS:   /\d+/.test(s)
来源：http://afb.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://lnh.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://usk.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jju.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://wkr.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ria.ivvv.top

[I02] 提取所有匹配
来源：http://oqx.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://ywi.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kdg.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cwz.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://pdz.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hry.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jts.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://ton.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ssp.tianlin.xyz

[I03] 提取捕获分组
来源：http://rfw.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wnl.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xqs.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bap.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aew.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nrr.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rcb.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bre.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qwi.gogol.net.cn

[I04] 正则替换
来源：http://oaa.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kgx.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dgj.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://npm.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://eby.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://zjf.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pda.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://izq.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ipb.daxiang520.top

[I05] 按正则拆分
来源：http://ffj.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aqt.hysaishi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://myb.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://qhx.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://avf.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://szo.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pgz.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://mqi.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fkk.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://etb.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ngq.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ccw.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ras.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ovv.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://knb.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://swd.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pej.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ttm.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://bgo.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hzv.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://edv.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jeo.aibaodan.cn

TS:   /error/gim
来源：http://vpb.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qwy.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cmn.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://mbs.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hrn.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://zgd.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qse.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gjp.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ijc.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oax.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oxv.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vxs.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fux.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xrn.ybcxt.top

================================================================================
来源：http://tmc.fengsongda.top

J. 日期与时间
来源：http://rtg.jiagoushi.top

================================================================================
来源：http://qxm.fengsongda.top

[J01] 获取当前时间
来源：http://jim.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://niy.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qdu.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://dok.tarul.cn

TS:   new Date();  Date.now()
来源：http://gwt.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bap.chenjidiqi.icu

Go:   time.Now()
来源：http://vgh.yuanzhike.top

Ruby: Time.now
来源：http://yab.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vfe.chenlongwang.top

[J02] 格式化输出
来源：http://wtb.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xrs.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lii.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://szr.nanxuanxn.top

TS:   d.toISOString()
来源：http://twn.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vdo.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://enx.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jjg.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mts.52xcode.cn

[J03] 字符串解析为日期
来源：http://lpr.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kzk.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dgt.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://iuq.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://sgp.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fjb.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vox.guowangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://oog.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sjp.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://smj.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nml.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qwo.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ntp.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dhw.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://itn.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xaf.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yvk.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tny.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://jjr.tanke756.top

Py:   now + timedelta(days=7)
来源：http://vrh.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ula.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pwr.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://osl.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://cjl.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pld.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://mkp.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://oxo.sxryk.cn

[J06] 计算两时间之差
来源：http://aoy.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://afc.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://sar.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tnq.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bxu.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://rab.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://pgv.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://oyx.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://kng.meibo888.top

[J07] 比较两个日期
来源：http://kbq.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://pdp.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xvp.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://mxs.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://yfv.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fxh.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://igz.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://arg.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://xri.guowangkeji.top

[J08] 提取年月日与星期
来源：http://huv.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hsq.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xkq.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qiw.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mkn.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://prb.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jep.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wkr.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://diu.ybcxt.top

[J09] 时区处理
来源：http://oox.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zjf.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://efj.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kwo.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxx.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uhc.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nex.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uil.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qqy.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://jev.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ssu.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iet.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kgy.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://luu.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mhg.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qrh.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tkx.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kdn.jiagoushi.top

================================================================================
来源：http://vdf.zhiwuduotai.top

K. JSON 与序列化
来源：http://jwf.cqqwz.cn

================================================================================
来源：http://ebp.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://akg.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://doq.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://edr.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://unm.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://heq.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iyw.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://wxx.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://ddn.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lda.tian-w.cn

[K02] JSON 字符串转对象
来源：http://kbo.hywenlv.cn

Py:   json.loads(s)
来源：http://bsx.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmi.gogol.net.cn

JS:   JSON.parse(s)
来源：http://sqg.nwbrower.top

TS:   JSON.parse(s)
来源：http://znf.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lcw.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://dea.meibo888.top

Ruby: JSON.parse(s)
来源：http://sga.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://owo.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://hmk.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iqg.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uir.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hxg.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://fro.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lzz.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ofn.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bpm.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lkc.tarul.cn

[K04] 读取 JSON 文件
来源：http://dso.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://srb.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jwb.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ivq.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://diq.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jtj.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xlw.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qnl.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hbh.hywenlv.cn

[K05] 深拷贝对象
来源：http://ekr.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://wom.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://map.gotoacloud.top

JS:   structuredClone(obj)
来源：http://azf.aibaodan.cn

TS:   structuredClone(obj)
来源：http://nou.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://czw.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zef.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rjo.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pim.nwbrower.top

[K06] 解析 URL 查询串
来源：http://fqs.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ihv.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xyl.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hbw.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xpk.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kzd.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://loj.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rhd.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kcz.jinghuilouyu.cn

[K07] 进制转换
来源：http://xfn.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bnw.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jcy.shzxlz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cos.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vfc.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wmi.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cts.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bgi.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tqp.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://squ.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://xsb.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://rge.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://pto.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://pfk.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ywb.nanxuanxn.top

Go:   encoding/gob
来源：http://fyq.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://nnn.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cfh.jinyuanbaomall.cn

================================================================================
来源：http://okc.cdnleiting.top

L. 网络请求
来源：http://wnj.xingfuxueyuan.xyz

================================================================================
来源：http://lkh.smart0.xyz

[L01] 发送 GET 请求
来源：http://rlz.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://itp.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kvw.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://fxq.haohaochexian.top

TS:   await fetch(url)
来源：http://mrh.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xvh.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://oxt.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ldm.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ogs.meibo888.top

[L02] 发送 POST JSON
来源：http://krs.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://lhd.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://txh.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yap.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xoe.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pun.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oiv.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xpk.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xpx.jianghu66.top

[L03] 设置自定义请求头
来源：http://ppj.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ghj.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oyg.gaohongyu789.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cva.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zvf.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rez.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hyc.aibaodan.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rto.xuetiantiany.cn


<!-- 参考信息 -->