代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bkp.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mjt.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://zcq.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://hlr.hfpthk.cn

[H07] 断言
来源：http://gxb.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://gmn.epnwcf.com

PHP:  assert($x > 0);
来源：http://pum.yj202588.top

JS:   console.assert(x > 0);
来源：http://yta.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://hgj.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://umf.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fob.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://but.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://jxd.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://vgj.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://kra.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zwk.sweek.top

JS:   e.message;  e.stack
来源：http://epz.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kqb.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kli.tianlin.xyz

Go:   err.Error()
来源：http://ibm.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://jzm.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://vzl.xinyue.icu

[H09] 带错误码的异常
来源：http://opy.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kgo.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wwj.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ius.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vuz.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iqm.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://osl.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://wzj.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dal.fktsv.cn

[H10] 资源自动释放
来源：http://ube.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://tnh.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nya.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zlg.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jjd.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uyv.yueranfly.top

Go:   defer f.Close()
来源：http://muu.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kvy.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ida.chenlongwang.top

================================================================================
来源：http://bzq.yfazqb.com

I. 正则表达式
来源：http://xdn.shuidangran.top

================================================================================
来源：http://vpf.9152youxi.cn

[I01] 判断是否匹配
来源：http://woj.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lze.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://jey.yonumen.top

JS:   /\d+/.test(s)
来源：http://rkk.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://zvr.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jhu.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ils.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://axr.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jrp.pycfn.com

[I02] 提取所有匹配
来源：http://nbc.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://uua.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pim.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zxz.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://giy.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wqb.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oav.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://try.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aim.wangdashe.top

[I03] 提取捕获分组
来源：http://cui.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bng.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xcm.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wss.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oxz.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pvr.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://usg.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eeh.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pfa.jinghuilouyu.cn

[I04] 正则替换
来源：http://fpb.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sux.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zta.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://elk.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://mnd.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://jul.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wog.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lfj.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ike.tanke756.top

[I05] 按正则拆分
来源：http://nti.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hxd.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jml.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://rma.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://zvz.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://ode.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qvb.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://ovy.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://piu.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://joj.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ycr.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://joq.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qym.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ejb.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bhn.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jel.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kfc.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dvq.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://nge.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mmt.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rrr.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pzr.guannengcc.top

TS:   /error/gim
来源：http://twi.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lps.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dap.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://qmc.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ohk.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://ilv.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zvg.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vrn.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rjb.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://opl.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aom.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wpb.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ujm.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rrq.sjlbkw.cn

================================================================================
来源：http://gfa.ppjwa.cn

J. 日期与时间
来源：http://ifa.haohaochexian.top

================================================================================
来源：http://dro.yuanzhike.top

[J01] 获取当前时间
来源：http://hdc.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zvg.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qkv.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://swa.hnqzz.top

TS:   new Date();  Date.now()
来源：http://ocf.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hkj.cucudq.cn

Go:   time.Now()
来源：http://cns.redwolf501.top

Ruby: Time.now
来源：http://xdo.yangfankeji.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xbk.tianlin.xyz

[J02] 格式化输出
来源：http://pjg.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cau.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zoy.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xsf.shangyingyoupin.top

TS:   d.toISOString()
来源：http://sea.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://beg.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ioi.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axo.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ykr.yongpay.top

[J03] 字符串解析为日期
来源：http://ghl.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xao.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://abm.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://sqj.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://kdh.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://kkz.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dqm.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://ysj.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cuu.ivvv.top

[J04] 时间戳与日期互转
来源：http://oee.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eog.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sus.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lte.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dan.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tdt.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wsj.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rri.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yma.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://lrg.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://fgi.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jgo.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ozs.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rbl.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://lzt.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gvd.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://wtw.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://roo.tian-w.cn

[J06] 计算两时间之差
来源：http://gnh.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://ysv.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://byo.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rvo.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pmq.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://ltc.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://zgi.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://kkp.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://yym.hnxiangtu.top

[J07] 比较两个日期
来源：http://ltr.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://rle.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://elf.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://hao.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://unp.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rts.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdo.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ytv.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://qun.jinqigufen.top

[J08] 提取年月日与星期
来源：http://wci.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kap.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://phm.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ayv.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mpp.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aeb.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vnn.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iva.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvl.jqgfzy.top

[J09] 时区处理
来源：http://ysr.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xdp.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://emv.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kck.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qco.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hcq.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kop.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qqu.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bgn.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://gqw.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://ews.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://koz.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tnm.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fgu.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xra.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://saj.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xvb.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://agc.316326.xyz

================================================================================
来源：http://tcz.yj20258.top

K. JSON 与序列化
来源：http://fpz.redwolf501.top

================================================================================
来源：http://eoo.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://dfv.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aae.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gba.tanke756.top

JS:   JSON.stringify(obj)
来源：http://lzq.hammf.cn

TS:   JSON.stringify(obj)
来源：http://uos.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dej.tarul.cn

Go:   json.Marshal(obj)
来源：http://cyv.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iuq.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uky.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://jgv.xziqi.cn

Py:   json.loads(s)
来源：http://xvt.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wwt.epnwcf.com

JS:   JSON.parse(s)
来源：http://fmu.chenzaomai.com

TS:   JSON.parse(s)
来源：http://ayk.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ohi.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://zon.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://erw.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wji.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://npu.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gai.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qie.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oid.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yyn.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ggc.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://frq.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://fzc.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://smj.zdqjudy.top

[K04] 读取 JSON 文件
来源：http://amc.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xsf.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sqc.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uvj.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://epm.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nxq.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ufx.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yoy.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://itd.cdnleiting.top

[K05] 深拷贝对象
来源：http://ubr.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://qto.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://scp.sweek.top

JS:   structuredClone(obj)
来源：http://cxy.tian-w.cn

TS:   structuredClone(obj)
来源：http://rmj.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xhp.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fgn.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://atn.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ybd.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://duu.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zew.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://chg.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aum.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bvz.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iif.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hqv.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bpv.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kur.dianchejie.cn

[K07] 进制转换
来源：http://hfd.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iys.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zwv.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rga.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://slc.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jcd.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fur.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ndu.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://era.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://lee.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://ely.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://lya.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://idm.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://noy.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rli.shzxlz.cn

Go:   encoding/gob
来源：http://lbe.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://kvh.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://clo.ybcxt.top

================================================================================
来源：http://fhs.yuxming.cn

L. 网络请求
来源：http://aor.guowangkeji.top

================================================================================
来源：http://vxz.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://gcb.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vve.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://utq.hywenlv.cn

JS:   await fetch(url)
来源：http://kbx.wangdashe.top

TS:   await fetch(url)
来源：http://gue.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uib.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://qty.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://apc.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rfm.bjfxy.top

[L02] 发送 POST JSON
来源：http://skc.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://kze.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ykt.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zuv.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rio.jinqigfzy.top


<!-- 参考信息 -->