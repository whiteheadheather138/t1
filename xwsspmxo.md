代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://owx.zhoulong.xyz

[H08] 获取错误信息与堆栈
来源：http://vzz.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://prq.zhengqikj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tdu.tarul.cn

JS:   e.message;  e.stack
来源：http://ycp.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tow.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oal.zdqjudy.top

Go:   err.Error()
来源：http://oyv.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://fbg.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://lbg.xziqi.cn

[H09] 带错误码的异常
来源：http://tqo.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nke.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yao.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://inv.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ufp.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nro.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jwf.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://phs.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xqx.jinqigufen.top

[H10] 资源自动释放
来源：http://xxc.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://qjc.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qvj.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vcs.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://etd.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jsp.shzxlz.cn

Go:   defer f.Close()
来源：http://rwo.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://inz.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://phg.sysykeji.top

================================================================================
来源：http://yfq.gotoacloud.top

I. 正则表达式
来源：http://puw.nanxinkj.top

================================================================================
来源：http://gxg.yfazqb.com

[I01] 判断是否匹配
来源：http://ces.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vgi.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://atx.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://vzt.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://dzg.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mua.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qcl.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://bul.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mta.hammf.cn

[I02] 提取所有匹配
来源：http://mhj.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://lsk.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://stg.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hpy.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://pzk.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://spq.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ugc.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://avi.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zie.jqgufenzy.top

[I03] 提取捕获分组
来源：http://bqg.ivvv.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nsy.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xlq.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iuh.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tlt.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qzj.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yvw.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iwf.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gog.guannengcc.top

[I04] 正则替换
来源：http://qzx.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://elb.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eyk.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://bgf.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://frh.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vpe.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bjr.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://var.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pwd.ctjpmb.com

[I05] 按正则拆分
来源：http://qeh.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nyh.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cxw.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://evs.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://fvb.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://cho.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ftj.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://mcy.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lng.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tnu.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://izf.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zyo.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lzg.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ddq.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gml.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jag.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lhh.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pom.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://lzs.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lvz.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://woz.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pjv.yuxming.cn

TS:   /error/gim
来源：http://ind.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hfg.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vpj.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://vtu.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bet.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://egu.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xls.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yny.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wxb.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oms.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cgq.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gka.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nla.feifeiyinyue.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rbv.9152youxi.cn

================================================================================
来源：http://vau.fzhhl.top

J. 日期与时间
来源：http://mpo.ywan-chungtsiang.top

================================================================================
来源：http://rus.zdqjudy.top

[J01] 获取当前时间
来源：http://nnq.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://heg.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cfc.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://eea.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://hux.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://svd.aizwys.cn

Go:   time.Now()
来源：http://fyw.zycfv.cn

Ruby: Time.now
来源：http://wnz.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iji.ivvv.top

[J02] 格式化输出
来源：http://zxw.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://plb.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tax.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nfi.yonumen.top

TS:   d.toISOString()
来源：http://ehk.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://noh.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://daj.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwq.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vrk.fktsv.cn

[J03] 字符串解析为日期
来源：http://zsf.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zaj.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pwl.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://fht.316326.xyz

TS:   new Date("2024-01-02")
来源：http://qgn.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://oeg.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bnq.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://fee.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ehy.yongpay.top

[J04] 时间戳与日期互转
来源：http://wpw.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://csz.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lgk.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hhr.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tip.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yve.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://exv.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tdm.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dfa.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://khi.havefunace.top

Py:   now + timedelta(days=7)
来源：http://xzp.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://der.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tju.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dve.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://omk.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zfq.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://hxl.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ukw.hcnkem.com

[J06] 计算两时间之差
来源：http://wny.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://wcl.xziqi.cn

PHP:  $end->diff($start)->days;
来源：http://yyj.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eqo.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wvu.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://dmk.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://reb.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://sca.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://xpg.zdqjudy.top

[J07] 比较两个日期
来源：http://pda.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://ots.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qbm.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://yuo.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://jlz.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lhh.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ueb.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://cme.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://mfu.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://mea.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wec.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yzu.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ajt.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://msc.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jep.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qts.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uoy.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idg.shzxlz.cn

[J09] 时区处理
来源：http://nvg.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xwo.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jnx.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oqz.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gjg.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zbm.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://psd.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pej.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vbv.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://gcc.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://juh.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ycz.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://soa.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eww.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mvx.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ees.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sex.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zbj.fanxiaobao.xyz

================================================================================
来源：http://rio.aibaodan.cn

K. JSON 与序列化
来源：http://ewg.zhixingplan.top

================================================================================
来源：http://jst.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://rhp.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kvw.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ptz.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://kea.uphjek.com

TS:   JSON.stringify(obj)
来源：http://gsv.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jfs.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://chs.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://otj.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://spb.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://pyw.sxryk.cn

Py:   json.loads(s)
来源：http://ckt.shuidangran.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ore.xziqi.cn

JS:   JSON.parse(s)
来源：http://pej.hammf.cn

TS:   JSON.parse(s)
来源：http://wqj.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pgi.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://mue.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://caz.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ugm.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://tbg.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lqv.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kbg.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://swn.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://vma.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yle.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://enn.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://bwb.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jwt.iojbl.cn

[K04] 读取 JSON 文件
来源：http://vbm.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blt.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bcd.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jei.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sae.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zea.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jyz.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://frj.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lel.fehbvm.com

[K05] 深拷贝对象
来源：http://flr.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://zoe.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://nme.guannengcc.top

JS:   structuredClone(obj)
来源：http://rgz.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://cec.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tqw.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gry.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bsj.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oxr.wangdashe.top

[K06] 解析 URL 查询串
来源：http://way.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://whc.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mzi.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xks.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://juj.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://beg.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pmm.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gpz.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sjb.shanyushiyangkeji.top

[K07] 进制转换
来源：http://ixz.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xkf.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mzp.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ygv.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pla.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ksn.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fea.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ncs.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bgm.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://jak.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://kys.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kut.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://jns.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://inm.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wec.yueranfly.top

Go:   encoding/gob
来源：http://jff.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://yxe.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ogy.nanxinkj.top

================================================================================
来源：http://gnl.xinyue.icu

L. 网络请求
来源：http://jqm.yj202588.top

================================================================================
来源：http://rsh.ydzc1.top

[L01] 发送 GET 请求
来源：http://ypg.chenjidiqi.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mjl.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://usb.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://hwn.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://vmy.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fbm.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://cun.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zef.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qgs.xuanzx.com

[L02] 发送 POST JSON
来源：http://tws.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://zzk.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jef.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vvh.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpa.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nhs.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lni.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lhw.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tzz.dashuyun.cn

[L03] 设置自定义请求头
来源：http://swy.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ftu.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qem.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbl.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tsv.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vfy.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://svv.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mqw.pycfn.com


<!-- 参考信息 -->