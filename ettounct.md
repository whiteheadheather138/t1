代发 wailian999

[H07] 断言
来源：http://nzo.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://xhh.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://nle.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://ehn.yj202588.top

TS:   console.assert(x > 0);
来源：http://trv.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://bkz.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dlp.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cgl.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://bqq.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://zde.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://dqa.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xwr.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://nxe.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://riq.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pee.cdnleiting.top

Go:   err.Error()
来源：http://kis.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://nyz.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://dtr.yj202588.top

[H09] 带错误码的异常
来源：http://ckq.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hqo.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ena.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fjk.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ynw.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nvp.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rax.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fqr.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sal.yj20258888.top

[H10] 资源自动释放
来源：http://bhf.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wfp.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ltr.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bct.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xql.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bqd.sxryk.cn

Go:   defer f.Close()
来源：http://wvj.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fau.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://krr.jinghuilouyu.cn

================================================================================
来源：http://qva.fengsongda.top

I. 正则表达式
来源：http://ixn.zhaomingkeji.xyz

================================================================================
来源：http://vwt.cqqwz.cn

[I01] 判断是否匹配
来源：http://fdy.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wze.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iyf.bbcook.cn

JS:   /\d+/.test(s)
来源：http://nuy.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://btg.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rgd.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://acd.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://cca.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://olb.andypj.xyz

[I02] 提取所有匹配
来源：http://thc.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://hca.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mee.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ikf.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://uhq.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bwx.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cqh.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://laq.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ety.cqqwz.cn

[I03] 提取捕获分组
来源：http://nqd.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://siy.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://klp.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jbr.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wgl.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xiv.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://obd.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bgc.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wsn.gotoacloud.top

[I04] 正则替换
来源：http://yps.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aie.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hji.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://umq.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://yqx.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://eac.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rlb.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bhx.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qxd.ybcxt.top

[I05] 按正则拆分
来源：http://ouv.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qqs.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rbg.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://uts.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://shs.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://qtw.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://opa.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yqi.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://whe.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hcd.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mbj.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tew.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vtj.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdv.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://saz.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qct.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://chf.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nzt.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://naq.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nvt.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dky.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qpx.epnwcf.com

TS:   /error/gim
来源：http://rnw.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zis.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cmh.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://klt.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mrq.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://fbh.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dkd.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jpx.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lny.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://esa.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://std.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://thb.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fqt.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fwi.hywenlv.cn

================================================================================
来源：http://esi.9152youxi.cn

J. 日期与时间
来源：http://lby.tarul.cn

================================================================================
来源：http://cvw.c1oappe.top

[J01] 获取当前时间
来源：http://gki.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://edu.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kul.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://yit.316326.xyz

TS:   new Date();  Date.now()
来源：http://vrx.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://xeu.aizwys.cn

Go:   time.Now()
来源：http://eis.wangshuangyany.cn

Ruby: Time.now
来源：http://xjz.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fnx.0kj1m.cn

[J02] 格式化输出
来源：http://ktb.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ggl.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jxh.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://isp.iojbl.cn

TS:   d.toISOString()
来源：http://mhs.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jxq.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xci.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqd.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wdk.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://wna.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bar.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cmr.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://ojn.cheryme.top

TS:   new Date("2024-01-02")
来源：http://sss.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://mki.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jiq.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://njb.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://npq.wangdashe.top

[J04] 时间戳与日期互转
来源：http://ygj.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://agw.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qhd.yongpay.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://waa.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://jiw.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://liz.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zdd.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yaf.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wqc.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://tyy.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://upf.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wui.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rdp.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzw.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ioh.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://brt.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://jjr.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rov.bjfxy.top

[J06] 计算两时间之差
来源：http://sax.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://tau.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://byt.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tzf.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ehb.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://emn.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://lvi.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://fyv.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://lpt.xuanzx.com

[J07] 比较两个日期
来源：http://srz.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://etx.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yub.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://ocf.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jvk.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nco.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oip.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://xiw.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://jtm.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://imd.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://twn.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oss.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cti.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vcj.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://czu.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://unk.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aza.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dyf.ybcxt.top

[J09] 时区处理
来源：http://kjs.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dmx.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://phw.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fgt.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wht.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://skt.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lla.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bja.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zxl.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://kdg.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kic.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cnx.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rib.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cat.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://abz.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jcm.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iij.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wds.pycfn.com

================================================================================
来源：http://qji.52xcode.cn

K. JSON 与序列化
来源：http://kzy.nanxinkj.top

================================================================================
来源：http://rwl.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://rne.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fsh.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ner.yj20258.top

JS:   JSON.stringify(obj)
来源：http://rjk.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://qqc.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wnm.hesvh.cn

Go:   json.Marshal(obj)
来源：http://zqv.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://usw.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uuu.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://dyw.ivvv.top

Py:   json.loads(s)
来源：http://qem.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kvx.guannengcc.top

JS:   JSON.parse(s)
来源：http://dfm.wangdashe.top

TS:   JSON.parse(s)
来源：http://zwj.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blo.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://lnl.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://xjv.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zbl.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://oqn.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wpi.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jns.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tmc.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jji.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mam.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgp.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://vdf.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aim.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://hjc.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eze.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ypg.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ist.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://anc.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://muq.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qpn.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://cfi.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bao.gotoacloud.top

[K05] 深拷贝对象
来源：http://fud.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://sxa.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://kaq.shzxlz.cn

JS:   structuredClone(obj)
来源：http://fbm.yuanzhike.top

TS:   structuredClone(obj)
来源：http://qvy.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zgx.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dqt.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://swu.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://joq.gzhubu.top

[K06] 解析 URL 查询串
来源：http://hpx.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dhc.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jvp.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fec.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vxz.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lbz.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://not.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gix.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pqe.quarkkingdee.top

[K07] 进制转换
来源：http://xgi.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gqx.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://moh.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pvp.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nkz.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hgp.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://heh.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ncy.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nmb.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://udw.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://fwg.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sss.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://axy.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://mde.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tzg.cheryme.top

Go:   encoding/gob
来源：http://mxr.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://knw.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ukb.daria6918.cn

================================================================================
来源：http://zga.shanyushiyangkeji.top

L. 网络请求
来源：http://dmc.yongpay.top

================================================================================
来源：http://hil.hesvh.cn

[L01] 发送 GET 请求
来源：http://dxq.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xlu.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nhn.uphjek.com

JS:   await fetch(url)
来源：http://hvl.ehwqpu.com

TS:   await fetch(url)
来源：http://ecf.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vps.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://slw.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ail.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jlj.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://mnh.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dog.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qoj.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tzk.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sxr.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://csf.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gzy.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vqn.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tez.yfazqb.com


<!-- 参考信息 -->