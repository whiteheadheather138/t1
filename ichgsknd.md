代发 wailian999

TS:   console.assert(x > 0);
来源：http://sjh.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://ctz.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wix.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://odd.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://gbv.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://kje.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://ksz.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wyu.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://tkd.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://oyw.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wwb.epnwcf.com

Go:   err.Error()
来源：http://wpj.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://rbi.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://tah.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://cio.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hyi.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xdi.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://orx.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jal.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lwj.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xkk.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://bte.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lmu.cheryme.top

[H10] 资源自动释放
来源：http://kwy.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nfy.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tgn.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wfv.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rqc.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uej.zhongyouzk.top

Go:   defer f.Close()
来源：http://hib.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rkn.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lyi.svipenyu.cn

================================================================================
来源：http://wtq.shzxlz.cn

I. 正则表达式
来源：http://myh.yueranfly.top

================================================================================
来源：http://ayg.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://sex.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://elw.cashguo.top

PHP:  preg_match('/\d+/', $s);
来源：http://crt.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://gzj.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://wpn.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ptv.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xik.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://bfk.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ezo.vehdjk.com

[I02] 提取所有匹配
来源：http://tkj.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://xwa.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iry.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ymb.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://htv.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nkn.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qfz.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://atd.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://edc.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://bcf.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zoo.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://etv.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cqq.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rgd.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xav.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qca.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ikw.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rfg.jinyuanbaomall.cn

[I04] 正则替换
来源：http://rwp.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://esk.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ljj.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nxo.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nqc.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://sxi.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tmc.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rdt.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://btk.ydzc1.top

[I05] 按正则拆分
来源：http://puf.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vwx.316326.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://flv.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://mku.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://mgo.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://zth.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hra.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://qbm.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ajo.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hzy.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pqd.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://meb.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppk.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gaz.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://drj.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bgb.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lbe.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hre.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://mpw.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ima.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bqg.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zqk.yueranfly.top

TS:   /error/gim
来源：http://zkj.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wds.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mxb.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://qrk.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zpa.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://sof.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hak.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rsg.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bzd.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://amo.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uef.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rov.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wrk.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zva.sxryk.cn

================================================================================
来源：http://mkr.xinyue.icu

J. 日期与时间
来源：http://orn.yj20258888.top

================================================================================
来源：http://pgn.fzhhl.top

[J01] 获取当前时间
来源：http://bep.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gil.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xvx.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://pix.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://vsj.chenjidiqi.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://wfu.tarul.cn

Go:   time.Now()
来源：http://zeq.chenjidiqi.icu

Ruby: Time.now
来源：http://gly.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://owe.hammf.cn

[J02] 格式化输出
来源：http://cih.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pwl.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zpc.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kju.fehbvm.com

TS:   d.toISOString()
来源：http://lut.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hto.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bki.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rov.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ngr.hfpthk.cn

[J03] 字符串解析为日期
来源：http://wch.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sbl.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bdh.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://bpj.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://hcp.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://qpu.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ebz.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://xej.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nzq.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://wat.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jgr.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ard.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wba.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://vnj.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qkf.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ewu.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vou.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jfa.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://acw.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ush.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uec.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qec.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bza.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://xzd.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lkf.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://sgv.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://mak.yongpay.top

[J06] 计算两时间之差
来源：http://noj.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://vry.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://xzi.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zku.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybp.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dgg.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://qmj.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://sjc.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://xgf.zdbjq.cn

[J07] 比较两个日期
来源：http://sgh.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://bzd.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kuo.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://mwm.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://rfd.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://roq.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nus.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gyr.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://lqr.aibaodan.cn

[J08] 提取年月日与星期
来源：http://kue.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zbm.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://upk.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nde.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hjs.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ndb.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gut.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kat.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nei.ydjk.org.cn

[J09] 时区处理
来源：http://zmp.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iry.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kdt.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rmq.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ttz.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ktb.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uey.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://itg.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vvy.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://pbe.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wvj.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mqe.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qjv.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ith.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ctw.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cvw.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eop.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hnm.52xcode.cn

================================================================================
来源：http://vry.zhijiandao.cn

K. JSON 与序列化
来源：http://jvi.sxryk.cn

================================================================================
来源：http://uwr.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://atx.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gbd.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dns.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://mnr.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://lns.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zlk.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://nlw.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://ywr.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fxw.bbcook.cn

[K02] JSON 字符串转对象
来源：http://lxg.ppjwa.cn

Py:   json.loads(s)
来源：http://miy.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fzp.jinqigufen.top

JS:   JSON.parse(s)
来源：http://jks.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://gwa.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vuz.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://eqp.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://mls.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wuw.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://lgk.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kfc.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ezy.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rbi.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://bza.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wsb.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ikc.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://dkl.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://civ.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://mfp.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rtu.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qno.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aoq.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ixh.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jjc.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rfb.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wmh.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvk.0kj1m.cn

[K05] 深拷贝对象
来源：http://lyn.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://oct.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://ref.snrcjt.cn

JS:   structuredClone(obj)
来源：http://gad.guowangkeji.top

TS:   structuredClone(obj)
来源：http://qlc.aizwys.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kwp.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pek.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hyg.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pav.hesvh.cn

[K06] 解析 URL 查询串
来源：http://fsn.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jdu.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mbo.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bfy.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yhg.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qbq.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eks.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jcj.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iaj.zhongyouzk.top

[K07] 进制转换
来源：http://fxi.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kzs.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rum.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jnc.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pzg.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tkx.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dsq.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nsi.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://msh.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://wnr.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://vij.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://exp.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://ejn.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://cty.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sag.tanke756.top

Go:   encoding/gob
来源：http://nki.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://vwz.hammf.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vwv.ydzc1.top

================================================================================
来源：http://tku.yj20258888.top

L. 网络请求
来源：http://rrp.ybcxt.top

================================================================================
来源：http://njw.uphjek.com

[L01] 发送 GET 请求
来源：http://eii.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tta.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://shp.andypj.xyz

JS:   await fetch(url)
来源：http://nea.guowangkeji.top

TS:   await fetch(url)
来源：http://lpj.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fni.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://cno.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sqb.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nrf.ydzc1.top

[L02] 发送 POST JSON
来源：http://ziu.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://ydg.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rgi.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://drx.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://occ.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://use.sjlbkw.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lej.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rte.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gvd.tarul.cn

[L03] 设置自定义请求头
来源：http://fkm.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pwq.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hpm.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dop.yfazqb.com


<!-- 参考信息 -->