代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://lbd.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://agq.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://cnn.sjlbkw.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bjo.aizwys.cn

JS:   e.message;  e.stack
来源：http://obb.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://amr.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oms.shzxlz.cn

Go:   err.Error()
来源：http://iul.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://lpl.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://sxe.aibaodan.cn

[H09] 带错误码的异常
来源：http://ubx.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xwf.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jck.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rvo.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zqr.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vll.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kzi.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://wwl.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://lyw.haohaochexian.top

[H10] 资源自动释放
来源：http://lyy.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nsw.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lht.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pcd.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mpp.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yip.yonumen.top

Go:   defer f.Close()
来源：http://gvs.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dnx.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bwk.yueranfly.top

================================================================================
来源：http://jtx.bbcook.cn

I. 正则表达式
来源：http://kgq.haohaochexian.top

================================================================================
来源：http://oak.gzhubu.top

[I01] 判断是否匹配
来源：http://tat.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fwy.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wpc.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://qlb.yonumen.top

TS:   /\d+/.test(s)
来源：http://got.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wzs.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://axh.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://pev.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://six.tanke756.top

[I02] 提取所有匹配
来源：http://zgl.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://vja.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ycd.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jow.birdmap.top

TS:   s.match(/\d+/g)
来源：http://otv.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mnk.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yim.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://ovv.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zyy.pengpengdd.cyou

[I03] 提取捕获分组
来源：http://rpa.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hjc.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wal.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zqx.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gmn.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wqb.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hcu.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zox.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://avl.yueranfly.top

[I04] 正则替换
来源：http://zhy.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hir.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tgs.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://cjy.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://rfe.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://neh.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://guw.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rly.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zsm.birdmap.top

[I05] 按正则拆分
来源：http://mas.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lum.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dqg.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://ojr.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://hqq.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://dki.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ugp.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://hvb.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uwm.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bwa.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ndo.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://huy.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dop.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xde.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uwh.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jai.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kdq.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nyo.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://thw.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ojb.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uqg.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xtp.yj202588.top

TS:   /error/gim
来源：http://mgl.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://loo.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ano.hammf.cn

Ruby: s.scan(/error/i)
来源：http://ean.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qbx.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://fih.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ptk.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ish.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nin.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oju.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://bsr.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zvn.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ywj.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://llo.fktsv.cn

================================================================================
来源：http://mva.cheryme.top

J. 日期与时间
来源：http://neu.ppjwa.cn

================================================================================
来源：http://niz.hesvh.cn

[J01] 获取当前时间
来源：http://pud.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://apg.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hlv.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://bjc.iojbl.cn

TS:   new Date();  Date.now()
来源：http://raa.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nyb.guannengcc.top

Go:   time.Now()
来源：http://ywb.hcnkem.com

Ruby: Time.now
来源：http://vfl.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rif.xuetiantiany.cn

[J02] 格式化输出
来源：http://sht.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chm.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gwf.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dgg.yfazqb.com

TS:   d.toISOString()
来源：http://zuw.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jmp.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ele.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fvi.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rab.hysaishi.cn

[J03] 字符串解析为日期
来源：http://lyk.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rai.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ukh.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://ygn.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://zuw.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ifn.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dvu.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://apy.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ooy.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://jjt.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://paa.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujr.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vhl.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lik.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ljv.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uir.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvr.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fnb.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://lcu.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://oia.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tby.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aqi.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pij.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://psu.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://edn.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://qsh.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://xzj.daria6918.cn

[J06] 计算两时间之差
来源：http://ffo.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://buw.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://lzp.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jlo.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hvj.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://yuz.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://bdk.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://enr.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://oox.hfpthk.cn

[J07] 比较两个日期
来源：http://ymi.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://jts.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://smm.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ttb.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://ooj.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cea.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hkt.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jak.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://onu.zhixingplan.top

[J08] 提取年月日与星期
来源：http://kzq.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://puw.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wvn.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dzn.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://txs.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wys.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ovo.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mrr.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ijv.gzhubu.top

[J09] 时区处理
来源：http://xsx.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ydr.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mfz.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okb.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kce.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://diq.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cyh.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kbe.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jia.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://hiz.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://byh.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ufs.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xlx.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ace.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ygn.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ykj.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ipl.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xif.quarkkingdee.top

================================================================================
来源：http://uly.hongshengwenyu.top

K. JSON 与序列化
来源：http://kxr.zhengqikj.top

================================================================================
来源：http://uug.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://cop.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jqx.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lht.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://vsl.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://bog.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mwu.316326.xyz

Go:   json.Marshal(obj)
来源：http://qnu.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://xqj.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://mxg.ydzc1.top

[K02] JSON 字符串转对象
来源：http://ymm.xuanzx.com

Py:   json.loads(s)
来源：http://rzs.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jco.chenlongwang.top

JS:   JSON.parse(s)
来源：http://pun.xziqi.cn

TS:   JSON.parse(s)
来源：http://inr.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mgm.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://qbj.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://uvl.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://puq.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://snx.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cgr.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lhr.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hhe.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://krb.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sgl.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://smh.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ijf.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://klg.hnqzz.top

[K04] 读取 JSON 文件
来源：http://iyt.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eie.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uqw.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bru.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emv.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bvg.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://skg.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ouy.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ryr.hysaishi.cn

[K05] 深拷贝对象
来源：http://ziz.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://whf.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://oot.jianghu66.top

JS:   structuredClone(obj)
来源：http://qlc.fengsongda.top

TS:   structuredClone(obj)
来源：http://gdf.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lja.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mks.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://odt.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://rqx.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://avo.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bjo.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kzn.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jua.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://voc.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qte.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://opd.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xis.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lca.zhijiandao.cn

[K07] 进制转换
来源：http://abv.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xbj.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zjg.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://apj.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ngt.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://byi.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rjt.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eey.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wzl.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://ccu.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://zdi.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uba.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://fbt.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://tfg.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ypk.fehbvm.com

Go:   encoding/gob
来源：http://hsq.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://wsp.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fst.yonumen.top

================================================================================
来源：http://oaq.fktsv.cn

L. 网络请求
来源：http://dxw.redwolf501.top

================================================================================
来源：http://caq.fehbvm.com

[L01] 发送 GET 请求
来源：http://gxi.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mcn.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pzb.bbcook.cn

JS:   await fetch(url)
来源：http://rqo.xuanzx.com

TS:   await fetch(url)
来源：http://uxr.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://otz.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://adw.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gxo.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bat.bbcook.cn

[L02] 发送 POST JSON
来源：http://ujf.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bvn.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vgo.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aup.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uqe.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://skv.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lhy.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aow.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zkv.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://avc.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zya.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://snb.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ztt.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fgz.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fni.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dxo.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://beb.gotoacloud.top


<!-- 参考信息 -->