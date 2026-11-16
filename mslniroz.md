代发 wailian999

[H07] 断言
来源：http://udu.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://plj.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://zuy.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://wii.tarul.cn

TS:   console.assert(x > 0);
来源：http://ifa.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://aph.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://imc.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://klg.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://heb.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://tcu.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://tau.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://znf.zdbjq.cn

JS:   e.message;  e.stack
来源：http://uaq.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ahf.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://iro.haohaochexian.top

Go:   err.Error()
来源：http://sdu.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://uic.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://pun.andypj.xyz

[H09] 带错误码的异常
来源：http://kuq.guowangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uoo.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cve.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mdb.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wpa.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://klc.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vtq.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ahs.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dfi.ehwqpu.com

[H10] 资源自动释放
来源：http://leg.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://saj.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xbd.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zkc.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dyj.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hih.zhoulong.xyz

Go:   defer f.Close()
来源：http://vtj.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://stt.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://luy.gogol.net.cn

================================================================================
来源：http://fve.nanxuanxn.top

I. 正则表达式
来源：http://ydv.yj202588.top

================================================================================
来源：http://als.xylfe.cn

[I01] 判断是否匹配
来源：http://zbj.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zji.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://rbl.sxryk.cn

JS:   /\d+/.test(s)
来源：http://goe.sweek.top

TS:   /\d+/.test(s)
来源：http://iaf.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zgr.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://noj.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://oyg.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hqn.9152youxi.cn

[I02] 提取所有匹配
来源：http://vye.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://etr.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hxf.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sga.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://ufo.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://usi.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lyn.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://byv.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qgi.zhoulong.xyz

[I03] 提取捕获分组
来源：http://brd.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://guu.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ngc.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uft.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xjc.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lui.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xnl.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lkt.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ibe.quarkkingdee.top

[I04] 正则替换
来源：http://fjc.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nrt.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kyv.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://rzv.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://hiu.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://lqu.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lyc.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://csh.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nla.vehdjk.com

[I05] 按正则拆分
来源：http://ilj.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://doa.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ifu.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://spc.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://zkz.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://ubz.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kxp.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://njj.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uzn.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bxg.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tlr.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://azv.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fja.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ruf.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lsi.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kis.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oqx.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nzq.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://jqf.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ksq.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rad.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aeq.zhixingplan.top

TS:   /error/gim
来源：http://shk.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://npo.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://upx.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://mmt.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hwt.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://vwj.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hbi.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rzx.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rzj.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ccd.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qem.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xyc.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://omh.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ibf.jinqigufen.top

================================================================================
来源：http://boa.zhoulong.xyz

J. 日期与时间
来源：http://oav.xingfuxueyuan.xyz

================================================================================
来源：http://wem.ppjwa.cn

[J01] 获取当前时间
来源：http://cwc.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://kpg.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xqv.zycfv.cn

JS:   new Date();  Date.now()
来源：http://rxk.daria6918.cn

TS:   new Date();  Date.now()
来源：http://axe.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qfu.c1oappe.top

Go:   time.Now()
来源：http://muw.yj202588.top

Ruby: Time.now
来源：http://wzr.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kyq.mhx1999.top

[J02] 格式化输出
来源：http://hht.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gba.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ytn.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mzt.epnwcf.com

TS:   d.toISOString()
来源：http://asg.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://egq.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pvr.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nxl.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xla.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://czv.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sgk.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cin.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://iih.meibo888.top

TS:   new Date("2024-01-02")
来源：http://iyo.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://rzr.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qhs.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://wzm.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pga.xinyue.icu

[J04] 时间戳与日期互转
来源：http://wsg.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pxv.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ljr.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xff.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hue.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zbu.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eww.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vwe.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tyd.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://ohy.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://akg.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yxh.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fjt.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yka.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://inq.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xxg.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://sns.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ilu.epnwcf.com

[J06] 计算两时间之差
来源：http://wii.pycfn.com

Py:   (end - start).total_seconds()
来源：http://ujw.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://tju.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lua.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rab.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://knt.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://xtd.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://vex.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://zum.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://ibi.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://dll.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hky.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://jmv.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://faf.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tyt.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://otz.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hgp.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://mlj.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://flr.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fje.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vwl.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xkn.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qgr.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iay.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hjw.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://isz.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fvy.yuxming.cn

[J09] 时区处理
来源：http://een.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xai.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://usu.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fkk.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqy.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nma.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pav.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hnk.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://naa.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://zqg.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://beo.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lpt.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zjt.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iet.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zva.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qpx.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qfa.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blt.fktsv.cn

================================================================================
来源：http://glr.0kj1m.cn

K. JSON 与序列化
来源：http://jyc.tarul.cn

================================================================================
来源：http://cxd.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://grz.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yom.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bkl.uphjek.com

JS:   JSON.stringify(obj)
来源：http://vlq.316326.xyz

TS:   JSON.stringify(obj)
来源：http://ywv.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wau.c1oappe.top

Go:   json.Marshal(obj)
来源：http://zvn.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://gag.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ugk.fehbvm.com

[K02] JSON 字符串转对象
来源：http://uvs.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://feg.shuidangran.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://erb.jianghu66.top

JS:   JSON.parse(s)
来源：http://say.cucudq.cn

TS:   JSON.parse(s)
来源：http://jww.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ngn.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://gum.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://rpb.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blb.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://egi.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fkj.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yno.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rdz.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://slp.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jjt.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ncj.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://wkh.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dku.zhongyouzk.top

[K04] 读取 JSON 文件
来源：http://ixo.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://psj.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aix.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eph.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zzm.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tvp.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbu.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://opi.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iik.cucudq.cn

[K05] 深拷贝对象
来源：http://ryo.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://plk.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://fgu.zdbjq.cn

JS:   structuredClone(obj)
来源：http://eij.jiagoushi.top

TS:   structuredClone(obj)
来源：http://iwe.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://faf.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ghj.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://evu.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://mec.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://yxx.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yhb.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yet.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qjq.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vap.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://anh.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ipc.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://elf.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qcn.aibaodan.cn

[K07] 进制转换
来源：http://aaq.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ogi.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jib.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mjj.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kes.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bil.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qeq.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uyu.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ovt.jqgfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://azu.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://akl.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hjs.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://dhh.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://omy.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lyu.yueranfly.top

Go:   encoding/gob
来源：http://tgy.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://vkb.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://waf.quarkkingdee.top

================================================================================
来源：http://ayu.hnqzz.top

L. 网络请求
来源：http://seb.havefunace.top

================================================================================
来源：http://srn.jianghu66.top

[L01] 发送 GET 请求
来源：http://bjw.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ftt.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mat.bbcook.cn

JS:   await fetch(url)
来源：http://tlh.tianlin.xyz

TS:   await fetch(url)
来源：http://kyu.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://epu.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://sin.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://owi.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jyf.zhixingplan.top

[L02] 发送 POST JSON
来源：http://xex.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ocv.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lxq.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wpa.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kaq.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://krk.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bfk.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://glj.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zrn.vqdsnc.cn


<!-- 参考信息 -->