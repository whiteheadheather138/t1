代发 wailian999

[H07] 断言
来源：http://aao.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://xdp.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://bhg.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://owm.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://xby.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://pbg.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://utg.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://fno.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://wph.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://tck.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://dcu.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xcv.cashguo.top

JS:   e.message;  e.stack
来源：http://oat.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://sol.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vqt.haohaochexian.top

Go:   err.Error()
来源：http://wow.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://any.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://yaj.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://rib.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fgs.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vmp.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rez.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pka.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uwg.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rff.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://qvb.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tlk.nanxinkj.top

[H10] 资源自动释放
来源：http://hnc.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fnn.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://geu.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iop.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aga.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yef.ctjpmb.com

Go:   defer f.Close()
来源：http://hxy.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dvw.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nqn.kuanghao11.cn

================================================================================
来源：http://cst.mhx1999.top

I. 正则表达式
来源：http://gvm.jiagoushi.top

================================================================================
来源：http://oeq.yj20258888.top

[I01] 判断是否匹配
来源：http://mvs.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://adm.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uol.wangdashe.top

JS:   /\d+/.test(s)
来源：http://ubn.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://flc.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xby.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ogj.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://jem.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aqv.ivvv.top

[I02] 提取所有匹配
来源：http://kdy.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://tyv.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mlq.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aam.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://xjf.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://thk.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lxo.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://lfx.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uto.meibo888.top

[I03] 提取捕获分组
来源：http://kit.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yho.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://laq.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jsq.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ghp.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dun.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qir.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvf.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pzq.fengsongda.top

[I04] 正则替换
来源：http://qzc.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tuk.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpw.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://shr.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://qbs.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://yhr.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yfo.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wew.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eei.smart0.xyz

[I05] 按正则拆分
来源：http://bxs.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dhq.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qbq.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://ahh.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://bri.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://mzf.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://brb.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://ecd.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgd.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://abi.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nla.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lky.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bhg.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rij.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qub.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qjs.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pvq.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eqm.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://ysv.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jxb.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gov.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gwl.vqdsnc.cn

TS:   /error/gim
来源：http://hso.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ryr.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jds.cheryme.top

Ruby: s.scan(/error/i)
来源：http://ymj.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://otb.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://wdx.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tmf.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uta.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lqt.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybv.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://axo.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nvh.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gfi.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://siv.sysykeji.top

================================================================================
来源：http://shn.epnwcf.com

J. 日期与时间
来源：http://pgg.shangyingyoupin.top

================================================================================
来源：http://blw.cucudq.cn

[J01] 获取当前时间
来源：http://jqa.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dvv.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vdi.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://lnn.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://akw.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sxp.uphjek.com

Go:   time.Now()
来源：http://sli.fzhhl.top

Ruby: Time.now
来源：http://irq.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rfy.fengsongda.top

[J02] 格式化输出
来源：http://tzo.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ekw.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://urf.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vjy.dashuyun.cn

TS:   d.toISOString()
来源：http://wjh.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eba.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xrs.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hzz.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://chq.xinyue.icu

[J03] 字符串解析为日期
来源：http://qsl.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tyu.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xiq.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://zbi.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://mce.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://rid.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zok.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://pti.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fks.ivvv.top

[J04] 时间戳与日期互转
来源：http://dxn.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bnz.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rhc.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ukw.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uje.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hpc.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jlf.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://feb.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gtl.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://gmn.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://ouy.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dfp.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jij.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://frf.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://jrs.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://epz.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://yqp.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://xae.hfpthk.cn

[J06] 计算两时间之差
来源：http://yla.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://qma.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://mkg.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sjk.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hgb.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uiy.fzhhl.top

Go:   end.Sub(start).Hours()
来源：http://aqi.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://kxk.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://fmw.316326.xyz

[J07] 比较两个日期
来源：http://xww.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://son.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aam.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zou.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://rog.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xoa.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uol.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://ine.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://qku.zdqjudy.top

[J08] 提取年月日与星期
来源：http://gdc.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgb.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ghk.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hlj.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ogy.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wye.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ryh.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://igh.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lis.hcnkem.com

[J09] 时区处理
来源：http://cqz.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kqc.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xdl.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jti.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kab.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kxr.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fme.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qfh.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hop.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://aib.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rss.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fxl.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pee.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fdp.jiagoushi.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wsf.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fnd.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kbf.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wwd.jqgufenzy.top

================================================================================
来源：http://fjf.tianlin.xyz

K. JSON 与序列化
来源：http://mqt.chenzaomai.com

================================================================================
来源：http://gqc.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://qnx.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bow.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wdq.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://uxm.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://oov.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kgu.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://zug.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://wbz.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dkt.daria6918.cn

[K02] JSON 字符串转对象
来源：http://nlb.sysykeji.top

Py:   json.loads(s)
来源：http://zfm.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://unx.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://uzp.zdbjq.cn

TS:   JSON.parse(s)
来源：http://hkb.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://roy.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://gzn.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://hmn.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lpr.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ctc.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wlc.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bul.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vbe.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://thb.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zwe.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://emz.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://quq.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cfz.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://bmj.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hht.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://que.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bfl.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dbn.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pqx.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qvk.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sya.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xtl.hysaishi.cn

[K05] 深拷贝对象
来源：http://lps.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://fqy.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://ljs.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://dsz.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://rmb.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ptd.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://teh.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gup.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dgq.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://jyd.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xql.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lxy.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ibm.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zra.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tdd.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://spc.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://urh.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ghb.zhongyouzk.top

[K07] 进制转换
来源：http://wyq.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ubo.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ykk.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxj.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wlm.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eoy.ywan-chungtsiang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sdw.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oif.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tir.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://jwb.yueranfly.top

Py:   pickle.dumps(obj)
来源：http://ydd.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yzg.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://frg.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://vml.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ont.mhx1999.top

Go:   encoding/gob
来源：http://xze.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://qlq.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xet.jinghuilouyu.cn

================================================================================
来源：http://hvp.yj202588.top

L. 网络请求
来源：http://kbs.feifeiyinyue.top

================================================================================
来源：http://fmq.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://rmg.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nih.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qmm.0kj1m.cn

JS:   await fetch(url)
来源：http://dkw.fktsv.cn

TS:   await fetch(url)
来源：http://cdm.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kud.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://kmw.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ajq.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xrw.bbcook.cn

[L02] 发送 POST JSON
来源：http://ezd.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dfw.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blk.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tew.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jtk.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ffa.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vtw.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xnm.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wtt.zycfv.cn


<!-- 参考信息 -->