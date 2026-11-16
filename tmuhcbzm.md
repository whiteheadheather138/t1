代发 wailian999

JS:   e.message;  e.stack
来源：http://iln.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://duy.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://fdh.jyoumei.cn

Go:   err.Error()
来源：http://bwc.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://vhi.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://fsn.hcnkem.com

[H09] 带错误码的异常
来源：http://yvn.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wjp.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lun.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zhb.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://czk.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mbg.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://arw.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://age.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tka.yuxming.cn

[H10] 资源自动释放
来源：http://euj.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eck.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wsx.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cwb.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mhp.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yfp.jyoumei.cn

Go:   defer f.Close()
来源：http://ifi.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xfs.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dpo.xinyue.icu

================================================================================
来源：http://vgr.guowangkeji.top

I. 正则表达式
来源：http://tgy.yuanzhike.top

================================================================================
来源：http://pmg.sjlbkw.cn

[I01] 判断是否匹配
来源：http://bvo.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://czu.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://byh.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://dek.yonumen.top

TS:   /\d+/.test(s)
来源：http://pft.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ayq.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ofn.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://hzl.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mdj.sufxvd.cn

[I02] 提取所有匹配
来源：http://szl.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://cfy.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://unv.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tem.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://yew.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bbd.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://feo.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://hik.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://exf.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://tzk.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jeu.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qst.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xdr.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jzb.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gpr.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kcz.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ryi.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aty.52xcode.cn

[I04] 正则替换
来源：http://dse.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://jzc.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zko.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://qfd.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://ctg.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uwx.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rzp.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://beh.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gbc.tarul.cn

[I05] 按正则拆分
来源：http://otb.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mnt.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dqo.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://ntw.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://pxa.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://que.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ssh.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://qfr.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ums.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://whj.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pgd.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fws.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pwq.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vmd.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bta.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bie.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kcn.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tzv.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://kzs.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ngu.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ixa.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://szb.bbcook.cn

TS:   /error/gim
来源：http://jee.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mtx.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aol.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://rzi.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jjv.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://qne.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gjj.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://abf.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ozy.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gnx.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rlo.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://duu.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vjs.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tej.shuidangran.top

================================================================================
来源：http://inv.hammf.cn

J. 日期与时间
来源：http://vqk.vehdjk.com

================================================================================
来源：http://fmk.hywenlv.cn

[J01] 获取当前时间
来源：http://yvt.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yoi.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yqy.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://xqx.mhx1999.top

TS:   new Date();  Date.now()
来源：http://cec.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://xnc.sufxvd.cn

Go:   time.Now()
来源：http://vji.ydjk.org.cn

Ruby: Time.now
来源：http://xrm.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dtm.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://asz.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nhw.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://elb.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ril.yangfankeji.com

TS:   d.toISOString()
来源：http://uvq.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gta.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lwe.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdl.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hkn.tianlin.xyz

[J03] 字符串解析为日期
来源：http://blr.ydzc1.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zki.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nai.cheryme.top

JS:   new Date("2024-01-02")
来源：http://tcw.cashguo.top

TS:   new Date("2024-01-02")
来源：http://uxk.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://qul.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://coq.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://dbi.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ijz.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://ler.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rda.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vye.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xjx.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cmm.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xip.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xzh.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lly.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xmu.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://ivh.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://byj.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ipo.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wct.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ech.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://eft.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://osd.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://lek.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zfn.guannengcc.top

[J06] 计算两时间之差
来源：http://wbf.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://wjj.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://oxj.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yxx.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hzy.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ghk.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://smc.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://zmv.nwbrower.top

C#:   (end - start).TotalSeconds
来源：http://qvf.yanxiufei.cn

[J07] 比较两个日期
来源：http://sre.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://zsl.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ajm.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://itw.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://bmm.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://duv.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ckl.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://yls.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://iwc.tian-w.cn

[J08] 提取年月日与星期
来源：http://zfi.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hli.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mga.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nof.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xxl.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ioa.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://umh.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ifu.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://grg.ybcxt.top

[J09] 时区处理
来源：http://mwt.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://woe.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ghx.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://veu.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbv.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vjj.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bkj.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hno.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://scj.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://tht.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://dqy.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fzu.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://djq.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nxx.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ltp.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eke.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kzb.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://erg.mhx1999.top

================================================================================
来源：http://gep.haohaochexian.top

K. JSON 与序列化
来源：http://ege.uphjek.com

================================================================================
来源：http://oxq.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://azi.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lty.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qlz.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://jdx.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://qsf.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hwg.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://ozu.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://odq.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://qhm.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://bmc.quarkkingdee.top

Py:   json.loads(s)
来源：http://lgl.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gsi.dianchejie.cn

JS:   JSON.parse(s)
来源：http://wod.guowangkeji.top

TS:   JSON.parse(s)
来源：http://skm.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oxo.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://ftm.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://lop.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lcb.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://riz.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ekj.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zex.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://som.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yfw.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zkb.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ipn.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://zqa.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tog.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://cir.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qvw.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fzf.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zrv.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvc.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jrx.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://plq.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://yzy.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jwl.pycfn.com

[K05] 深拷贝对象
来源：http://fuj.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://jml.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://rtm.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://oan.jianghu66.top

TS:   structuredClone(obj)
来源：http://mxh.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wia.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vcu.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xxw.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ixd.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://sch.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rzt.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sul.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hfb.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dts.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jnh.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wtx.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vwh.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vsa.316326.xyz

[K07] 进制转换
来源：http://frp.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hho.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wjj.iojbl.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fph.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kzt.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jtr.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gxn.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://azs.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://opn.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dju.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://irv.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tjc.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://xoh.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://uya.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ejy.hysaishi.cn

Go:   encoding/gob
来源：http://cvx.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://dvw.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jdz.ehwqpu.com

================================================================================
来源：http://pyx.yueranfly.top

L. 网络请求
来源：http://akk.zhoulong.xyz

================================================================================
来源：http://cib.gogol.net.cn

[L01] 发送 GET 请求
来源：http://cqm.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mix.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://spw.hnqzz.top

JS:   await fetch(url)
来源：http://fry.snrcjt.cn

TS:   await fetch(url)
来源：http://teo.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lwi.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://sru.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jqs.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aul.tarul.cn

[L02] 发送 POST JSON
来源：http://hvp.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://knf.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jll.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uvk.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rft.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hzj.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mgo.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wnk.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://moc.ivvv.top

[L03] 设置自定义请求头
来源：http://pea.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://obs.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://znc.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mqo.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jki.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://whv.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://opo.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yek.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://abr.hesvh.cn

[L04] 设置超时
来源：http://ukd.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://tfq.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ivd.jinghuilouyu.cn


<!-- 参考信息 -->