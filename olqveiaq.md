代发 wailian999

TS:   console.assert(x > 0);
来源：http://tam.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://xov.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xxl.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://qtc.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://men.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://ttc.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://sdf.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ptu.aibaodan.cn

JS:   e.message;  e.stack
来源：http://qlh.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://hwi.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xdz.jiagoushi.top

Go:   err.Error()
来源：http://hhu.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://spe.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://ikv.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://rca.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ecz.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bzz.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xiq.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xnj.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gfm.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sgx.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://vio.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ffv.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://lzn.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ahj.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cas.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dfz.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ddb.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cln.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://dvq.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dtx.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cqc.nanxuanxn.top

================================================================================
来源：http://guw.xingfuxueyuan.xyz

I. 正则表达式
来源：http://thh.cashguo.top

================================================================================
来源：http://wvh.ctjpmb.com

[I01] 判断是否匹配
来源：http://yhj.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dwz.jqgfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://tsm.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://ake.xuanzx.com

TS:   /\d+/.test(s)
来源：http://qco.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jwg.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hkb.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://kny.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://drm.aibaodan.cn

[I02] 提取所有匹配
来源：http://ihh.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://yqq.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dbm.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wqh.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://xov.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://weq.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ufk.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://jzv.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uqj.yanxiufei.cn

[I03] 提取捕获分组
来源：http://nct.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://evv.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xzb.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hok.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uzs.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tor.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://whv.shzxlz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pzm.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://keg.zdqjudy.top

[I04] 正则替换
来源：http://oww.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kqq.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hfe.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://ncf.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://adv.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ngx.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ueg.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ahl.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://afu.haohaochexian.top

[I05] 按正则拆分
来源：http://cma.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lco.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ezu.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://mcj.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://sso.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://rkm.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kfw.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://itv.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sfn.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uxy.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://taq.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zkj.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cgy.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mty.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vlk.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rkw.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xtt.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sjf.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://ork.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://psn.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nyb.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://knr.feifeiyinyue.top

TS:   /error/gim
来源：http://dhb.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jpd.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dqc.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://qtg.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://otc.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://kjp.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oug.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zyj.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nkf.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uml.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ubj.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yvc.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dbg.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://trb.iojbl.cn

================================================================================
来源：http://fjn.fengsongda.top

J. 日期与时间
来源：http://sln.tian-w.cn

================================================================================
来源：http://ywc.fzhhl.top

[J01] 获取当前时间
来源：http://jtx.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nhc.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pyx.sxryk.cn

JS:   new Date();  Date.now()
来源：http://wgt.mhx1999.top

TS:   new Date();  Date.now()
来源：http://krf.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qii.bbcook.cn

Go:   time.Now()
来源：http://hnf.fengsongda.top

Ruby: Time.now
来源：http://bqt.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gfu.xziqi.cn

[J02] 格式化输出
来源：http://tuu.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsz.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rsm.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yip.cheryme.top

TS:   d.toISOString()
来源：http://rdw.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://urx.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxz.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hck.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gqo.wangdashe.top

[J03] 字符串解析为日期
来源：http://dwl.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yzi.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ahm.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://wvr.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://nyy.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rik.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tcr.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://jwj.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fdt.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://qaq.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hwn.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lzj.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ckl.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gnh.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pvg.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://chh.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gto.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lgg.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://hlq.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://psb.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qsw.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uaf.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ycp.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://zsr.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://est.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://qbp.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vuc.yj20258888.top

[J06] 计算两时间之差
来源：http://psx.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://fep.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://jyt.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://prt.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xlw.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://nbm.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://sez.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://zsn.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://poi.meibo888.top

[J07] 比较两个日期
来源：http://wbl.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://ecp.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://phk.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://ixn.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://sur.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qjp.aibaodan.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xoe.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://jje.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://cna.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://fxb.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fop.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lpx.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ayj.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vgj.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bwv.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hyu.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://igl.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lsl.meibo888.top

[J09] 时区处理
来源：http://pwx.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dql.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sju.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vho.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iyq.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://osy.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lgt.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nvy.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qxh.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://fis.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tjy.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://trr.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dfb.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://avy.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tds.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ctt.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wme.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yib.yj20258.top

================================================================================
来源：http://ksp.jiagoushi.top

K. JSON 与序列化
来源：http://jmi.epnwcf.com

================================================================================
来源：http://xxx.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://upy.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mlm.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mxn.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://nwu.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://arm.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xah.uphjek.com

Go:   json.Marshal(obj)
来源：http://nfr.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://mzz.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sbe.redwolf501.top

[K02] JSON 字符串转对象
来源：http://nqh.sxryk.cn

Py:   json.loads(s)
来源：http://pch.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://prz.hcnkem.com

JS:   JSON.parse(s)
来源：http://ael.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://mhy.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wsx.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://pcj.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://bxs.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tuo.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://kic.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vdu.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lky.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tcs.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xgq.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jkz.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://acm.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://qpd.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aiw.uphjek.com

[K04] 读取 JSON 文件
来源：http://xww.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kqg.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bcv.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bch.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rbl.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dah.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zle.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jaw.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kzg.yongpay.top

[K05] 深拷贝对象
来源：http://noj.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://akn.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://dhf.yueranfly.top

JS:   structuredClone(obj)
来源：http://try.zycfv.cn

TS:   structuredClone(obj)
来源：http://cpj.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gvs.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bqq.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://inu.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tfc.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://kfa.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uqi.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ftk.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://joc.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dcc.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fsl.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oiw.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uyc.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://snh.zycfv.cn

[K07] 进制转换
来源：http://swz.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vma.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jxv.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qsr.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rzp.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vrd.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jlk.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nqs.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dgt.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://vqk.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://zbs.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hpf.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://uzu.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://krp.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uth.ydjk.org.cn

Go:   encoding/gob
来源：http://vaf.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://yoh.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vmg.fanxiaobao.xyz

================================================================================
来源：http://isr.wangshuangyany.cn

L. 网络请求
来源：http://wfx.vqdsnc.cn

================================================================================
来源：http://wlk.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://tju.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cct.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gbz.hesvh.cn

JS:   await fetch(url)
来源：http://iev.shzxlz.cn

TS:   await fetch(url)
来源：http://uum.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kdj.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://zyc.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qyg.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qxy.jiagoushi.top

[L02] 发送 POST JSON
来源：http://ess.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://ump.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uto.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://psc.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gde.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpw.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wbf.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://chp.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xkr.hesvh.cn

[L03] 设置自定义请求头
来源：http://arl.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://acb.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://btx.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uod.ywan-chungtsiang.top


<!-- 参考信息 -->