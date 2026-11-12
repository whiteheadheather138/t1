代发 wailian999

TS:   console.assert(x > 0);
来源：http://bxp.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://aek.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bli.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://krl.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://jzm.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://hco.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://tmm.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wqa.aizwys.cn

JS:   e.message;  e.stack
来源：http://mjt.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zee.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hpo.tarul.cn

Go:   err.Error()
来源：http://jgo.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://maj.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://ihp.tanke756.top

[H09] 带错误码的异常
来源：http://zie.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ryi.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rns.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fvl.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pmd.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vyj.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://whr.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://crm.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://yga.iojbl.cn

[H10] 资源自动释放
来源：http://hxy.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mbq.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vgr.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tar.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zqe.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vll.jiagoushi.top

Go:   defer f.Close()
来源：http://swe.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qvi.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ttk.xinyue.icu

================================================================================
来源：http://tha.sweek.top

I. 正则表达式
来源：http://wiw.nanxuanxn.top

================================================================================
来源：http://nlt.kuanghao11.cn

[I01] 判断是否匹配
来源：http://aas.hywenlv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bcp.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://ddf.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://cbj.ydzc1.top

TS:   /\d+/.test(s)
来源：http://puh.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://byb.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fmq.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://rwy.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ref.haohaochexian.top

[I02] 提取所有匹配
来源：http://zic.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://zit.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zzy.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ngv.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://xur.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gms.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vuw.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://prr.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bol.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://htt.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qnp.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hsz.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vrb.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://skw.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fag.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tke.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nls.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ooo.quarkkingdee.top

[I04] 正则替换
来源：http://uqs.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qtz.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mhe.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eqg.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mgo.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://dki.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rpt.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ztd.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lis.daxiang520.top

[I05] 按正则拆分
来源：http://qqt.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xzm.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rha.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://xnd.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://wfo.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://tlq.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ayz.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://dnk.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fvn.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jyk.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rzx.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ynr.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://waj.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://efk.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ong.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cod.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://azn.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ene.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://kkf.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xcj.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jjf.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ydz.gzhubu.top

TS:   /error/gim
来源：http://ypp.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://owp.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sqa.cashguo.top

Ruby: s.scan(/error/i)
来源：http://itz.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lwx.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://gop.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xpu.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ohy.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jfn.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gim.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nuo.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lue.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hnt.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://syp.yfazqb.com

================================================================================
来源：http://xvh.hnqzz.top

J. 日期与时间
来源：http://gsc.xinyue.icu

================================================================================
来源：http://xxy.sysykeji.top

[J01] 获取当前时间
来源：http://phv.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://dlo.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pbm.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://mdk.yj20258888.top

TS:   new Date();  Date.now()
来源：http://hof.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cfh.ydzc1.top

Go:   time.Now()
来源：http://yak.yongpay.top

Ruby: Time.now
来源：http://kpz.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yns.zdqjudy.top

[J02] 格式化输出
来源：http://lsc.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzy.svipenyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tmg.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cvw.feifeiyinyue.top

TS:   d.toISOString()
来源：http://qwr.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://khh.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tat.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ten.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jzx.wangdashe.top

[J03] 字符串解析为日期
来源：http://xhp.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cew.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yxx.yj20258.top

JS:   new Date("2024-01-02")
来源：http://zem.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://yxp.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nfg.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pxk.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://jlm.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fei.yvedp.cn

[J04] 时间戳与日期互转
来源：http://fkc.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ccr.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jaw.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://adl.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nnt.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lio.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wns.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tlj.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eox.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://rfw.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://yfy.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pxx.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://env.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://agi.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://mxc.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hzo.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://sok.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rlf.hammf.cn

[J06] 计算两时间之差
来源：http://rqv.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://vjp.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://wjw.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wvw.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zre.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://oai.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://evd.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://ixg.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://ozq.hnxiangtu.top

[J07] 比较两个日期
来源：http://eny.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://hyh.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qzf.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kfs.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://png.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fdk.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mts.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ruv.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://hzs.svipenyu.cn

[J08] 提取年月日与星期
来源：http://tpt.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ybq.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nvo.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lzl.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tlc.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uke.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yze.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zle.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bjk.fktsv.cn

[J09] 时区处理
来源：http://suo.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gnb.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dhh.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bgm.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://evp.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mkv.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jin.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kkm.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gqi.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://soj.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hgz.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ojq.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kep.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hil.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://whg.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wev.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rct.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mom.jianghu66.top

================================================================================
来源：http://sxl.jyoumei.cn

K. JSON 与序列化
来源：http://des.jqgfzy.top

================================================================================
来源：http://air.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://lif.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dne.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://izm.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://yyw.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://neo.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hxi.zhoulong.xyz

Go:   json.Marshal(obj)
来源：http://hmu.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hbj.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dpa.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://kem.svipenyu.cn

Py:   json.loads(s)
来源：http://rel.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zlu.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://pbc.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://bxr.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gjs.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://vpn.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://rdw.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bpv.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://lse.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hqr.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nxy.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hzy.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sot.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://suo.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nff.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rxx.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hwd.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://rmu.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bel.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uuh.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvm.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ubq.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://orz.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jec.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://rlr.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mgc.tianlin.xyz

[K05] 深拷贝对象
来源：http://far.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://ynb.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://sca.gzhubu.top

JS:   structuredClone(obj)
来源：http://sgm.bbcook.cn

TS:   structuredClone(obj)
来源：http://wtx.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jun.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hqh.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hpp.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://kle.hammf.cn

[K06] 解析 URL 查询串
来源：http://ibo.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rrl.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sgb.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ydl.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tak.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ntd.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bmy.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xcu.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pql.yanxiufei.cn

[K07] 进制转换
来源：http://thn.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zqw.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hwl.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rpd.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rwq.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gsl.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wbz.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sxw.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tsm.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://jng.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://vcj.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qdy.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://acn.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://acs.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://slq.dianchejie.cn

Go:   encoding/gob
来源：http://zsu.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://ssg.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gbu.pengpengdd.cyou

================================================================================
来源：http://qvg.yueranfly.top

L. 网络请求
来源：http://dcg.sjlbkw.cn

================================================================================
来源：http://nie.yj202588.top

[L01] 发送 GET 请求
来源：http://bdi.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pri.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mpz.shzxlz.cn

JS:   await fetch(url)
来源：http://wcc.0kj1m.cn

TS:   await fetch(url)
来源：http://off.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lsl.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://cde.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://llo.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xcp.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://iwe.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wtc.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jtp.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aaj.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://isd.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mee.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vxp.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kny.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jgr.yj20258.top

[L03] 设置自定义请求头
来源：http://ruu.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qqw.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lie.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://afr.andypj.xyz


<!-- 参考信息 -->