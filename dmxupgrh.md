代发 wailian999

JS:   e.message;  e.stack
来源：http://ign.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tmb.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://cel.xuanzx.com

Go:   err.Error()
来源：http://jtc.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://ywf.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://pur.jianghu66.top

[H09] 带错误码的异常
来源：http://vxv.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uma.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bte.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aud.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oak.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kyy.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uys.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://mzx.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fqp.ppjwa.cn

[H10] 资源自动释放
来源：http://kfq.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://pju.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zmp.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ohg.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bkr.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ang.yueranfly.top

Go:   defer f.Close()
来源：http://ptl.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sjs.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qbv.feifeiyinyue.top

================================================================================
来源：http://kul.yonumen.top

I. 正则表达式
来源：http://ism.chenjidiqi.icu

================================================================================
来源：http://xqe.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://gve.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ozb.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hoe.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://qth.shuidangran.top

TS:   /\d+/.test(s)
来源：http://isj.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bai.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://idt.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://wfq.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dav.ivvv.top

[I02] 提取所有匹配
来源：http://wog.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://ota.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tuc.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sxt.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://opd.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rst.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xie.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://xzo.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://epv.hcnkem.com

[I03] 提取捕获分组
来源：http://vjg.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://owp.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wmc.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sdo.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mtz.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://enb.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lqf.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yqa.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uby.ybcxt.top

[I04] 正则替换
来源：http://hme.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://erf.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ilv.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ywn.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xkq.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jgs.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pvl.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wxq.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bud.iojbl.cn

[I05] 按正则拆分
来源：http://mza.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kye.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qyv.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://alp.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://lzy.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://qnl.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aqo.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xvj.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mnr.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jfz.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iqf.snrcjt.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sfy.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iwy.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xgs.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mmh.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sbc.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ucg.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gpw.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://tuo.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iga.xziqi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bpi.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ecr.c1oappe.top

TS:   /error/gim
来源：http://atk.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bqh.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aiy.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://ahm.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tol.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://fnf.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fpw.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cdm.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ovx.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kld.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ahr.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pzf.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://plq.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hjj.fanxiaobao.xyz

================================================================================
来源：http://jab.wangdashe.top

J. 日期与时间
来源：http://xfk.shanyushiyangtech.top

================================================================================
来源：http://qxt.tian-w.cn

[J01] 获取当前时间
来源：http://lww.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://igi.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zxl.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://gvd.cashguo.top

TS:   new Date();  Date.now()
来源：http://vop.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tku.snrcjt.cn

Go:   time.Now()
来源：http://njg.daria6918.cn

Ruby: Time.now
来源：http://xsq.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ngu.sysykeji.top

[J02] 格式化输出
来源：http://pab.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nkx.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://crq.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uqi.pengpengdd.cyou

TS:   d.toISOString()
来源：http://sqf.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://obd.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xmk.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hpg.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vzm.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://pyh.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hpu.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zxc.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://wzb.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://ytd.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wmv.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iyx.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://lav.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fwq.sysykeji.top

[J04] 时间戳与日期互转
来源：http://lde.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ror.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oog.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zct.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://njy.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zxo.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://egt.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ixr.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ous.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://kku.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://qfm.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qok.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gjc.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://seb.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://tbl.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fnu.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://klw.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://xgn.guannengcc.top

[J06] 计算两时间之差
来源：http://bob.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://clk.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://hfw.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qam.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eea.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dct.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://bfy.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://wia.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://wcc.yvedp.cn

[J07] 比较两个日期
来源：http://smd.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://zag.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://txa.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://jgb.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://amv.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zek.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mvr.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ttz.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://pug.aibaodan.cn

[J08] 提取年月日与星期
来源：http://pos.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nqf.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fpi.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fnr.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jgo.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tqe.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uoe.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vrw.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wtk.zhoulong.xyz

[J09] 时区处理
来源：http://zhe.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iki.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mbd.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://saw.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzf.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cbn.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rhq.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://bxb.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mkp.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://vyo.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rpb.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mvs.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dih.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kde.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hik.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qts.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vqe.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ndf.yvedp.cn

================================================================================
来源：http://ztx.dashuyun.cn

K. JSON 与序列化
来源：http://tnj.xuetiantiany.cn

================================================================================
来源：http://rzk.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://fon.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nmj.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ein.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://esi.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://ddn.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ujo.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://dps.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://wgr.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://krd.pycfn.com

[K02] JSON 字符串转对象
来源：http://aqg.shangyingyoupin.top

Py:   json.loads(s)
来源：http://frc.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lnl.nwbrower.top

JS:   JSON.parse(s)
来源：http://vgd.yonumen.top

TS:   JSON.parse(s)
来源：http://vbg.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yms.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://ywh.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://qmc.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hmz.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://mnq.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kqb.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mpo.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ivd.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dss.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cgc.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rlt.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://hhk.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rjh.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://tfw.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ido.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gho.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vvw.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mka.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vpr.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://abr.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vod.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://skc.vqdsnc.cn

[K05] 深拷贝对象
来源：http://agl.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://xgk.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://rzk.yonumen.top

JS:   structuredClone(obj)
来源：http://vww.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://bjq.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://fjp.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hhe.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mgz.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://adw.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://noq.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mys.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://itu.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pck.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gqw.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oas.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fyz.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fhv.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://afr.zhixingplan.top

[K07] 进制转换
来源：http://rxd.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gvv.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eaj.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zbp.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zxn.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xzl.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bcq.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xdu.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://euf.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://ysy.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://kxj.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uqz.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://wrg.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://tlz.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wsw.fehbvm.com

Go:   encoding/gob
来源：http://pui.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://xsx.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vya.aizwys.cn

================================================================================
来源：http://nam.iojbl.cn

L. 网络请求
来源：http://wnd.9152youxi.cn

================================================================================
来源：http://muj.xinyue.icu

[L01] 发送 GET 请求
来源：http://wqj.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zud.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yey.hammf.cn

JS:   await fetch(url)
来源：http://jvq.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://npu.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xqh.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://iej.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jul.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dee.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://dio.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ufq.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wjd.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kbr.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsh.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xwn.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dup.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dsh.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lmu.jiagoushi.top

[L03] 设置自定义请求头
来源：http://umc.yj20258.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://phb.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lxg.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cql.sxryk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rgs.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://deq.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://htw.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://exy.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aun.xuetiantiany.cn

[L04] 设置超时
来源：http://iqm.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://lbt.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jni.yuanzhike.top


<!-- 参考信息 -->