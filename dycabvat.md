代发 wailian999

[H07] 断言
来源：http://bmb.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://fpy.cheryme.top

PHP:  assert($x > 0);
来源：http://bsb.cashguo.top

JS:   console.assert(x > 0);
来源：http://bqb.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://vam.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://zuw.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zef.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://npo.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://qdw.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://sob.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://wyo.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kio.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://fmn.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uwt.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nxr.wangdashe.top

Go:   err.Error()
来源：http://oui.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://cmy.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://con.shuidangran.top

[H09] 带错误码的异常
来源：http://mgz.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://miy.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vcx.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aiw.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cym.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jld.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fla.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://bme.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://kga.nwbrower.top

[H10] 资源自动释放
来源：http://ghb.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ann.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://myl.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ilj.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lao.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hli.jqgufenzy.top

Go:   defer f.Close()
来源：http://xsy.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qrf.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cxu.pycfn.com

================================================================================
来源：http://kwf.zhijiandao.cn

I. 正则表达式
来源：http://ryk.ybcxt.top

================================================================================
来源：http://urf.jianghu66.top

[I01] 判断是否匹配
来源：http://eyv.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://edp.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vpu.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://zye.fehbvm.com

TS:   /\d+/.test(s)
来源：http://oaq.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bqd.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aur.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://eqy.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://saa.vqdsnc.cn

[I02] 提取所有匹配
来源：http://euj.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://ssl.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tvr.yvedp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mmz.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://qvc.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jhd.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nob.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://ekp.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rvw.jinqigfzy.top

[I03] 提取捕获分组
来源：http://aka.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jyq.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ccv.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qtz.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://efd.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://apf.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://usz.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jsm.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wqd.xinyue.icu

[I04] 正则替换
来源：http://kub.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ase.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eii.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://nqf.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uib.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://uju.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qnr.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lgb.0kj1m.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ajd.kuanghao11.cn

[I05] 按正则拆分
来源：http://gax.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://agl.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sak.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://xfb.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://aek.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://luv.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oze.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://fss.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wmn.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://opj.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://slw.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://frb.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rii.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lsg.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lmm.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://elx.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://knv.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://isp.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://xeu.ybcxt.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eeo.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rfp.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zfy.hammf.cn

TS:   /error/gim
来源：http://obj.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://egf.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://avn.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://tni.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ror.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zfk.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hev.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blm.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvl.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pai.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zqi.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://duw.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zzn.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rbr.kuanghao11.cn

================================================================================
来源：http://sbm.nanxuanxn.top

J. 日期与时间
来源：http://gzv.yj202588.top

================================================================================
来源：http://gzb.hongshengwenyu.top

[J01] 获取当前时间
来源：http://mrj.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zuw.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dlq.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://vxr.yuxming.cn

TS:   new Date();  Date.now()
来源：http://qic.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://sbk.yanxiufei.cn

Go:   time.Now()
来源：http://nhv.zhixingplan.top

Ruby: Time.now
来源：http://rdj.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://geu.dashuyun.cn

[J02] 格式化输出
来源：http://xro.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cos.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ois.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ane.ehwqpu.com

TS:   d.toISOString()
来源：http://rmt.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dvw.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lqe.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yck.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wzb.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://brx.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://exz.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vhk.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://xxi.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://wrr.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://fpi.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://csd.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://qle.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xbq.shuidangran.top

[J04] 时间戳与日期互转
来源：http://tce.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gee.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xyu.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eck.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rsu.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qpb.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ezk.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zrq.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yke.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://cjf.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://bzu.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wvq.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tta.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dld.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://wch.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kbg.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://soe.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://cti.hesvh.cn

[J06] 计算两时间之差
来源：http://vjw.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://urq.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://tmb.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ooh.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wnx.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ygu.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://ctz.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://zzv.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://gde.yonumen.top

[J07] 比较两个日期
来源：http://sjw.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://dwb.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ftr.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kmv.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://ptf.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vso.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qoc.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://xfi.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://bwz.daxiang520.top

[J08] 提取年月日与星期
来源：http://xtc.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://krk.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dbr.yonumen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ivy.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kro.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ssp.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://inq.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lmd.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mkh.fengsongda.top

[J09] 时区处理
来源：http://uyh.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jwa.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aqi.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uer.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vmp.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vdy.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://szr.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zdr.ehwqpu.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ffw.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://kml.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rba.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jkc.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kpd.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://csk.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ypk.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wyx.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://duv.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zaj.uphjek.com

================================================================================
来源：http://bbx.kuanghao11.cn

K. JSON 与序列化
来源：http://zej.pengpengdd.cyou

================================================================================
来源：http://urg.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://vvj.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kxs.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nde.pycfn.com

JS:   JSON.stringify(obj)
来源：http://uel.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://vdo.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kwt.fktsv.cn

Go:   json.Marshal(obj)
来源：http://azx.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://qbg.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ytu.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://zdh.nanxuanxn.top

Py:   json.loads(s)
来源：http://ezd.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ivt.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://gca.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://hzn.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ecx.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://mxt.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://zyu.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pif.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://vce.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://upw.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zhz.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rwn.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://toi.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ihb.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nep.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vby.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mul.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://ufh.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pop.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dcu.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tcb.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uvb.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bml.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://crk.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lyp.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://smn.tanke756.top

[K05] 深拷贝对象
来源：http://cao.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://xjv.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://tvj.aizwys.cn

JS:   structuredClone(obj)
来源：http://lvk.daxiang520.top

TS:   structuredClone(obj)
来源：http://itk.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rnb.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://agp.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cvg.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eid.tanke756.top

[K06] 解析 URL 查询串
来源：http://bzd.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cfb.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://liy.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uwj.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://brf.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jxy.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://atn.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qfu.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baz.guowangkeji.top

[K07] 进制转换
来源：http://uao.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wht.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rcm.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tqd.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hgy.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tuu.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qin.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rtg.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://foa.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://bpn.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://iuw.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mvr.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://ler.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://xex.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wun.shzxlz.cn

Go:   encoding/gob
来源：http://jbr.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://wgk.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aop.jinghuilouyu.cn

================================================================================
来源：http://mel.ivvv.top

L. 网络请求
来源：http://oje.bjfxy.top

================================================================================
来源：http://auz.gotoacloud.top

[L01] 发送 GET 请求
来源：http://phd.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ptm.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yld.yuxming.cn

JS:   await fetch(url)
来源：http://fhr.gaohongyu789.top

TS:   await fetch(url)
来源：http://dal.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ebx.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://skd.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bwl.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qhz.xinyue.icu

[L02] 发送 POST JSON
来源：http://mnf.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://pct.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gxj.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qjs.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjn.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dhe.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lrc.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hmp.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://otf.zhaomingkeji.xyz


<!-- 参考信息 -->