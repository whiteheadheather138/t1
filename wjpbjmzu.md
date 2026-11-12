代发 wailian999

JS:   e.message;  e.stack
来源：http://sun.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ble.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://obv.andypj.xyz

Go:   err.Error()
来源：http://urb.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://kbc.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://gmj.havefunace.top

[H09] 带错误码的异常
来源：http://edc.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dyu.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://hoa.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iai.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uvy.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wqy.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jlb.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://gpr.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://thf.redwolf501.top

[H10] 资源自动释放
来源：http://hni.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kgi.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gkp.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fkv.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://smu.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qlg.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://usc.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://trt.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ldm.aizwys.cn

================================================================================
来源：http://ymp.nanxuanxn.top

I. 正则表达式
来源：http://scx.fanxiaobao.xyz

================================================================================
来源：http://ymo.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://erp.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fci.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://biw.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://joa.yj20258888.top

TS:   /\d+/.test(s)
来源：http://vtj.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pdv.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nrr.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://qta.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rdx.zdqjudy.top

[I02] 提取所有匹配
来源：http://egj.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://kql.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yvb.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://prj.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://ifp.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vje.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iav.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://qou.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jsu.fehbvm.com

[I03] 提取捕获分组
来源：http://rql.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wdu.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gct.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dgq.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mlu.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vul.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jej.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ejf.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hip.dashuyun.cn

[I04] 正则替换
来源：http://qre.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ebk.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://isc.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pih.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hfp.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zdd.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ywk.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://doc.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rlv.gogol.net.cn

[I05] 按正则拆分
来源：http://trc.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hnk.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zpy.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://xql.sjlbkw.cn

TS:   s.split(/\s*,\s*/)
来源：http://ntn.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://pwc.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zaz.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://sxw.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gti.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://goc.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xbk.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fqz.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nda.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bib.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aof.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jci.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gqv.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nsb.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://qfw.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wmo.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mdx.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://njw.xinyue.icu

TS:   /error/gim
来源：http://yfi.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ufl.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jyd.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://yge.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zbq.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://taa.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yot.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dfj.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ubb.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wtu.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oll.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rdv.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ndz.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iiq.feifeiyinyue.top

================================================================================
来源：http://lti.jlsjyb.cn

J. 日期与时间
来源：http://otc.zhijiandao.cn

================================================================================
来源：http://gkn.ydjk.org.cn

[J01] 获取当前时间
来源：http://ilt.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nra.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zoq.tarul.cn

JS:   new Date();  Date.now()
来源：http://kvi.yj202588.top

TS:   new Date();  Date.now()
来源：http://dbx.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sqf.redwolf501.top

Go:   time.Now()
来源：http://jnd.uphjek.com

Ruby: Time.now
来源：http://ald.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xyy.yj20258888.top

[J02] 格式化输出
来源：http://vom.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yan.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ymn.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ekz.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://wfg.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kxx.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xlb.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rqt.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awq.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://zzn.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hym.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dmj.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://com.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://qvz.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://znu.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rvx.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://mgd.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aun.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://gjc.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lmj.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hrb.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lja.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fzp.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nfl.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hsn.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lut.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qjm.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://wfh.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://xlr.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nec.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqs.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ylm.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://nxb.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gio.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://fdr.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://uca.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://qfx.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://ook.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://xas.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://agf.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://asw.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://jwk.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://gek.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://lvo.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://rpq.cqqwz.cn

[J07] 比较两个日期
来源：http://lqx.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://xlz.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hid.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yvs.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rci.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ujr.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cxg.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uhq.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://uak.gotoacloud.top

[J08] 提取年月日与星期
来源：http://uqf.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://icq.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zzu.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://adm.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zsq.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fir.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ujj.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bcq.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hdc.cheryme.top

[J09] 时区处理
来源：http://jau.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jkd.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eka.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jeu.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wnv.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bgl.jyoumei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ete.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://oxc.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cmw.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://dhd.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://afq.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xqj.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dzr.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yvu.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xks.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qtc.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jyb.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ymt.yj20258.top

================================================================================
来源：http://nya.kuanghao11.cn

K. JSON 与序列化
来源：http://zvi.ehwqpu.com

================================================================================
来源：http://qtd.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://rmn.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ngl.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qdm.sweek.top

JS:   JSON.stringify(obj)
来源：http://yan.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://lat.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cax.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://oua.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://nvu.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fcx.smart0.xyz

[K02] JSON 字符串转对象
来源：http://ibc.gaohongyu789.top

Py:   json.loads(s)
来源：http://ywx.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://svi.gzhubu.top

JS:   JSON.parse(s)
来源：http://wdl.birdmap.top

TS:   JSON.parse(s)
来源：http://cdu.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zdr.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://rsy.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://zgn.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ofd.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://dax.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fdw.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ifu.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://kxk.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dml.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rtl.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mkp.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://yam.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yaa.uphjek.com

[K04] 读取 JSON 文件
来源：http://qbf.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vzt.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://okx.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rgh.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rcd.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gkp.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gho.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hqj.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://upp.yanxiufei.cn

[K05] 深拷贝对象
来源：http://sjk.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://snj.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://loo.yongpay.top

JS:   structuredClone(obj)
来源：http://poa.hywenlv.cn

TS:   structuredClone(obj)
来源：http://bot.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eya.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hie.daria6918.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kdo.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rmx.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://bah.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eil.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iuy.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kfs.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://urw.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yog.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://obz.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nlc.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://veo.ehwqpu.com

[K07] 进制转换
来源：http://uix.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ldp.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nai.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dwo.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tyg.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uof.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://glq.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zjf.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pef.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://aju.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://shw.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vvj.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://wwp.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://bvk.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vhn.xylfe.cn

Go:   encoding/gob
来源：http://lww.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://zrp.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xwe.hcnkem.com

================================================================================
来源：http://eqr.vqdsnc.cn

L. 网络请求
来源：http://ahl.zycfv.cn

================================================================================
来源：http://azv.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://ybk.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ldx.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ujz.yuxming.cn

JS:   await fetch(url)
来源：http://jhz.hcnkem.com

TS:   await fetch(url)
来源：http://xry.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://krx.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://xal.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://shs.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lvy.tian-w.cn

[L02] 发送 POST JSON
来源：http://kic.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://xjs.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cfi.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zvf.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kui.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mtf.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://naw.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aiv.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://evy.c1oappe.top

[L03] 设置自定义请求头
来源：http://uuh.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ujk.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bhu.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nge.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pih.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jhf.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vkp.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pby.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lvy.yfazqb.com

[L04] 设置超时
来源：http://job.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://boq.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wai.kuanghao11.cn


<!-- 参考信息 -->