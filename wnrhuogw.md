代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://vzn.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://gtv.smart0.xyz

[H09] 带错误码的异常
来源：http://oqs.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://snk.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nmq.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oby.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://csw.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pyf.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fbr.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://gqd.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dyl.xinyue.icu

[H10] 资源自动释放
来源：http://naz.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rxr.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nxm.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tpj.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://obw.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kfp.ivvv.top

Go:   defer f.Close()
来源：http://umj.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xnu.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qgl.quarkkingdee.top

================================================================================
来源：http://nns.yangfankeji.com

I. 正则表达式
来源：http://lmd.aizwys.cn

================================================================================
来源：http://erh.ydjk.org.cn

[I01] 判断是否匹配
来源：http://ils.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kve.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://euo.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://bfx.andypj.xyz

TS:   /\d+/.test(s)
来源：http://jfe.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pts.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wzn.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://aaz.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://weu.pycfn.com

[I02] 提取所有匹配
来源：http://ruk.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://wip.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zoi.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tsy.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://nsl.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zwm.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ojh.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://ogz.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ikc.nanxuanxn.top

[I03] 提取捕获分组
来源：http://sft.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jue.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jvm.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sen.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hzq.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hnx.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sff.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pvj.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uzm.svipenyu.cn

[I04] 正则替换
来源：http://nos.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vaa.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rog.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bgt.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://emy.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://vsw.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zvl.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hpv.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yeu.redwolf501.top

[I05] 按正则拆分
来源：http://hxl.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fkh.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ckq.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://lnk.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://abw.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://aaz.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hrr.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://hxz.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tlw.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nez.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://joe.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xut.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mdk.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aee.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ckq.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ybi.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hrp.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nkv.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://ifa.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ave.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://esw.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hkh.yfazqb.com

TS:   /error/gim
来源：http://szd.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jzo.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aep.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://dvg.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sym.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://nuj.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mvv.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wpd.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvc.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxr.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dws.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eoo.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hmp.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dbf.redwolf501.top

================================================================================
来源：http://tmw.xylfe.cn

J. 日期与时间
来源：http://yxv.yfazqb.com

================================================================================
来源：http://wat.uphjek.com

[J01] 获取当前时间
来源：http://hil.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://usn.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hbv.redwolf501.top

JS:   new Date();  Date.now()
来源：http://xnm.yj202588.top

TS:   new Date();  Date.now()
来源：http://nns.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yup.aizwys.cn

Go:   time.Now()
来源：http://ltx.gzhubu.top

Ruby: Time.now
来源：http://opo.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jte.hysaishi.cn

[J02] 格式化输出
来源：http://ila.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nkr.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://poh.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lah.yanxiufei.cn

TS:   d.toISOString()
来源：http://yeh.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ova.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lyk.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kjj.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tbd.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://fum.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ogm.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jcz.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://jph.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://dvx.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://jyd.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nvl.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://pul.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://odu.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://bhm.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tyy.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://okz.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qxq.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://aya.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://trv.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vpc.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kea.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rty.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://iii.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://frt.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://frt.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sis.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zkg.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://fqf.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nma.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://xvw.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://gvc.gaohongyu789.top

[J06] 计算两时间之差
来源：http://wwi.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://yyo.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://hye.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uug.52xcode.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nrv.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://mog.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://pwj.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://jxf.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://auf.dashuyun.cn

[J07] 比较两个日期
来源：http://wwb.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://lqj.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ash.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://esb.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qyo.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ekz.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zxn.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kah.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://odi.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://uwr.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://noe.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lcu.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fdz.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ekm.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hwv.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gxb.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jfv.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://enz.jinyuanbaomall.cn

[J09] 时区处理
来源：http://luk.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://alo.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vhm.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hdq.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pmt.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tju.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ibv.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ucd.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ogo.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://oxk.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://erv.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gpo.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ank.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rym.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fnc.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://okn.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xfz.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ncm.fktsv.cn

================================================================================
来源：http://lfy.zdbjq.cn

K. JSON 与序列化
来源：http://koo.yuxming.cn

================================================================================
来源：http://yxd.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://ovw.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ewj.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pdx.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://qzr.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://tyh.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pio.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://xvu.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://nsp.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://gbv.epnwcf.com

[K02] JSON 字符串转对象
来源：http://orv.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://okg.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zqa.ybcxt.top

JS:   JSON.parse(s)
来源：http://adc.bjfxy.top

TS:   JSON.parse(s)
来源：http://dtr.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gzc.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://gjx.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://fxw.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cgt.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://chc.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xkd.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bie.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yvt.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qos.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://exu.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgc.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://pso.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nsx.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://lsb.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bqr.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://abk.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zgx.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bvy.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://asg.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kbh.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qsj.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ace.haohaochexian.top

[K05] 深拷贝对象
来源：http://xbw.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://ogz.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://ghu.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://crn.hammf.cn

TS:   structuredClone(obj)
来源：http://mgu.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://rkp.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tag.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nmo.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://urj.cucudq.cn

[K06] 解析 URL 查询串
来源：http://ahs.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sxp.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tgy.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mqw.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hub.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vpq.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bms.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vuc.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vjk.shangyingyoupin.top

[K07] 进制转换
来源：http://pvi.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ezq.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sye.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vhx.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://naw.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pms.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ult.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gpy.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rdi.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://ywr.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://bul.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xbx.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://eju.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://vzj.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cuz.zdbjq.cn

Go:   encoding/gob
来源：http://ttb.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://vqu.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zgc.ehwqpu.com

================================================================================
来源：http://vsh.fengsongda.top

L. 网络请求
来源：http://kxf.wangshuangyany.cn

================================================================================
来源：http://gpv.zdqjudy.top

[L01] 发送 GET 请求
来源：http://lpt.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xpw.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gsh.tianlin.xyz

JS:   await fetch(url)
来源：http://ebk.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://gtd.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pgc.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://rie.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xjo.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ehd.hesvh.cn

[L02] 发送 POST JSON
来源：http://wel.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://esk.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lyp.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://glo.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbi.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hwe.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tgx.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ipc.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dup.52xcode.cn

[L03] 设置自定义请求头
来源：http://myc.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jay.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://phn.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xjd.sxryk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ali.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zts.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gcb.hysaishi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ulf.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://umh.xinyue.icu

[L04] 设置超时
来源：http://hhh.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://goo.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qsd.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tia.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://juo.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fdv.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://olu.hnqzz.top


<!-- 参考信息 -->