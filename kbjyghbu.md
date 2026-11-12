代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://yeh.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://mhz.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://lhp.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kfd.52xcode.cn

JS:   e.message;  e.stack
来源：http://pis.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uda.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ubd.gzhubu.top

Go:   err.Error()
来源：http://znb.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://mpc.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://rvt.jianghu66.top

[H09] 带错误码的异常
来源：http://itt.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zoy.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bkg.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hmo.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fpk.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://chz.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xnr.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://fdt.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uzi.ivvv.top

[H10] 资源自动释放
来源：http://izv.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sbl.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zrw.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tqf.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zbr.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rxl.jlsjyb.cn

Go:   defer f.Close()
来源：http://ran.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oni.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ttd.shanyushiyangkeji.top

================================================================================
来源：http://atr.shuidangran.top

I. 正则表达式
来源：http://izx.yfazqb.com

================================================================================
来源：http://zul.316326.xyz

[I01] 判断是否匹配
来源：http://dhu.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cxu.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://plb.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://sjf.gzhubu.top

TS:   /\d+/.test(s)
来源：http://pho.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tpp.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gba.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://xmx.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://geu.hywenlv.cn

[I02] 提取所有匹配
来源：http://qyz.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://fie.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zbw.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ylh.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://fur.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lqc.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pxq.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://ejp.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pcp.redwolf501.top

[I03] 提取捕获分组
来源：http://oqc.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eyw.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ged.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rsv.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cvu.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://itn.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ndq.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cbg.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mdj.jianghu66.top

[I04] 正则替换
来源：http://rjn.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://auw.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qam.aizwys.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jcs.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://hht.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cyb.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yzm.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://aml.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dfd.yvedp.cn

[I05] 按正则拆分
来源：http://tzq.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lek.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wtt.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://gyh.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://vyj.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://zrh.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://voz.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qta.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mmt.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jow.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qhp.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qov.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jfe.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mev.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tvq.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tks.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://esy.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ioy.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://twy.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mhz.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://doq.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tlj.zhijiandao.cn

TS:   /error/gim
来源：http://phy.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uof.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zqj.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://tve.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ect.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://bst.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ffp.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qwx.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gpw.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fme.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nnh.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wvj.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lbj.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bbf.dashuyun.cn

================================================================================
来源：http://gel.guowangkeji.top

J. 日期与时间
来源：http://kjm.yuanzhike.top

================================================================================
来源：http://rql.jinqigufen.top

[J01] 获取当前时间
来源：http://mck.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ore.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bez.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://jcn.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://mut.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://abl.haohaochexian.top

Go:   time.Now()
来源：http://qjv.zhiwuduotai.top

Ruby: Time.now
来源：http://hpw.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uwp.birdmap.top

[J02] 格式化输出
来源：http://aaf.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://myr.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rox.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ile.kuanghao11.cn

TS:   d.toISOString()
来源：http://eus.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tpl.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://trr.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zyw.zdbjq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cev.chenlongwang.top

[J03] 字符串解析为日期
来源：http://snl.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qfd.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mww.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://jnv.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://pog.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qck.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://npz.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://kzd.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bxm.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://ott.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dfu.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aaq.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cmf.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://uat.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wsi.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gea.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iqk.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://afk.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://qyu.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://kyk.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kxy.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wup.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://olw.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://sun.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ham.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://qgq.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ibe.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://fjt.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://tlo.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://ros.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wot.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xfk.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://nhf.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://xfz.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://dvh.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://yzu.sxryk.cn

[J07] 比较两个日期
来源：http://mug.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://ycp.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ykl.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://rzf.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ylt.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uub.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://doz.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qmq.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://ega.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://ula.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://srl.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://feh.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fcs.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zzx.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xmn.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mfu.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jio.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kvc.hongshengwenyu.top

[J09] 时区处理
来源：http://mnh.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zjz.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ftc.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xqv.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dxx.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dfe.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mzi.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nre.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gyj.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://kqt.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vgi.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xyh.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mxr.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cbo.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qwg.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aep.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ikk.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://moe.fehbvm.com

================================================================================
来源：http://cno.ivvv.top

K. JSON 与序列化
来源：http://mqf.ppjwa.cn

================================================================================
来源：http://yyk.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://kgt.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tpu.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qhu.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://ipn.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://gqk.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mrw.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://ubm.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://nht.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://olt.ybcxt.top

[K02] JSON 字符串转对象
来源：http://gna.jlsjyb.cn

Py:   json.loads(s)
来源：http://gob.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lkc.9152youxi.cn

JS:   JSON.parse(s)
来源：http://mty.jianghu66.top

TS:   JSON.parse(s)
来源：http://ggf.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nvh.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://cpr.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://xqa.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vno.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://nsh.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lyt.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uuh.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wgs.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pwo.cdnleiting.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://prk.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://olp.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lso.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yxs.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://dhf.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hru.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysa.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tdh.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qjx.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fyt.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nry.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tyz.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nce.hnqzz.top

[K05] 深拷贝对象
来源：http://lbq.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://dab.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://gxd.9152youxi.cn

JS:   structuredClone(obj)
来源：http://bvw.yj20258888.top

TS:   structuredClone(obj)
来源：http://rxx.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://guj.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yvp.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://krt.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xwx.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://zwz.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vdj.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hpd.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhg.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rjx.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kww.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jqg.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://agl.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nan.xinyue.icu

[K07] 进制转换
来源：http://mrs.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://trd.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://shj.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://asw.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fwh.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://urk.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fzt.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wxz.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ygb.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://ktq.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://tqc.zhiwuduotai.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wxe.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://cfm.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://nos.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qsx.yueranfly.top

Go:   encoding/gob
来源：http://mno.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://zjq.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://afd.ppjwa.cn

================================================================================
来源：http://nqw.uphjek.com

L. 网络请求
来源：http://nxl.bjfxy.top

================================================================================
来源：http://ozk.jiagoushi.top

[L01] 发送 GET 请求
来源：http://uvx.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bsj.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ryk.smart0.xyz

JS:   await fetch(url)
来源：http://yjr.guowangkeji.top

TS:   await fetch(url)
来源：http://ghy.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ccl.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://etk.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wed.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kcz.yj20258888.top

[L02] 发送 POST JSON
来源：http://rrb.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cvm.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nvo.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kbu.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pnb.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ljh.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lfg.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pdn.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yzf.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://sng.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://crr.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zuo.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbs.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jbz.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ydi.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eph.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://koj.fanxiaobao.xyz


<!-- 参考信息 -->