代发 wailian999

[H07] 断言
来源：http://cbq.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://ezd.svipenyu.cn

PHP:  assert($x > 0);
来源：http://ckg.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://nzr.cucudq.cn

TS:   console.assert(x > 0);
来源：http://psv.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://uex.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wbt.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fjh.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://jez.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://qpd.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://yyy.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hso.yuxming.cn

JS:   e.message;  e.stack
来源：http://cie.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gno.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mlq.hesvh.cn

Go:   err.Error()
来源：http://oek.nanxinkj.top

Ruby: e.message;  e.backtrace
来源：http://gdd.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://lah.aizwys.cn

[H09] 带错误码的异常
来源：http://ota.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hie.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xsb.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jab.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wxm.cdnleiting.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nny.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vmc.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ucu.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fbd.havefunace.top

[H10] 资源自动释放
来源：http://pew.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yzo.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bnb.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://akm.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tad.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ras.hammf.cn

Go:   defer f.Close()
来源：http://kqr.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://efe.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bpf.andypj.xyz

================================================================================
来源：http://zfs.xziqi.cn

I. 正则表达式
来源：http://yjv.andypj.xyz

================================================================================
来源：http://tvp.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://nok.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cyw.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://dap.andypj.xyz

JS:   /\d+/.test(s)
来源：http://zzg.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://ngc.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nfw.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yrs.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://lpw.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://shy.sxryk.cn

[I02] 提取所有匹配
来源：http://qgk.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://boy.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cgg.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cum.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://lxr.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nhb.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://duy.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://yhf.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rmr.jyoumei.cn

[I03] 提取捕获分组
来源：http://ssp.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wcm.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ztq.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eay.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gfk.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ear.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ngn.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yfe.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tfh.zhengqikj.top

[I04] 正则替换
来源：http://jus.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ook.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kcs.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://sap.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xml.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://ebg.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://spk.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gde.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nyl.smart0.xyz

[I05] 按正则拆分
来源：http://qui.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qhs.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hrf.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://gjf.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://hbh.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://xnu.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gxn.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://itj.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iiz.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lia.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kdp.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zsn.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppq.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bam.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ayi.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nke.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ueq.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wib.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://tel.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hqv.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kqt.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ver.zdqjudy.top

TS:   /error/gim
来源：http://ido.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kdy.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://idf.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://itg.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qmm.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://xlb.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tob.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://txs.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aqu.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://puk.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://fiz.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wdo.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nyi.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sqt.gzhubu.top

================================================================================
来源：http://oob.havefunace.top

J. 日期与时间
来源：http://xnc.vehdjk.com

================================================================================
来源：http://ytp.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://hap.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ekr.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ubr.daria6918.cn

JS:   new Date();  Date.now()
来源：http://ois.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://hgb.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://arf.zhoulong.xyz

Go:   time.Now()
来源：http://cya.xuanzx.com

Ruby: Time.now
来源：http://day.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xxf.cqqwz.cn

[J02] 格式化输出
来源：http://caf.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avw.pycfn.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fmg.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tus.wangdashe.top

TS:   d.toISOString()
来源：http://ckm.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://odk.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gxm.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rfk.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://drv.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://jwj.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uvy.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eap.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://nkm.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://tdh.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://nmh.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://htn.snrcjt.cn

Ruby: Date.parse("2024-01-02")
来源：http://nai.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mvx.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://fbx.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pan.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mwe.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mvn.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://cdz.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://igg.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jvb.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zjp.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xrw.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://qeu.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://qpj.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kye.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qko.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pnm.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://azh.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pyy.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://kkv.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://qvy.guannengcc.top

[J06] 计算两时间之差
来源：http://owi.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://kmb.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://kny.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://med.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vpc.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lud.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://xnr.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://ute.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://omt.wangshuangyany.cn

[J07] 比较两个日期
来源：http://cck.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://xes.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tav.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://ggq.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://swb.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rzt.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vab.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nni.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://idl.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://vnk.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ytg.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://psw.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xsd.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://acd.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tsx.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aoe.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sab.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fim.tarul.cn

[J09] 时区处理
来源：http://koq.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bpi.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ysu.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ddj.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://anz.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ipw.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hvz.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kdb.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pxw.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://bal.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vcv.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fei.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oik.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://raa.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nmq.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fto.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lii.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jfm.pycfn.com

================================================================================
来源：http://nth.hammf.cn

K. JSON 与序列化
来源：http://lyq.chenlongwang.top

================================================================================
来源：http://prj.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://xal.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mrq.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cve.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://awe.meibo888.top

TS:   JSON.stringify(obj)
来源：http://roc.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zlb.ybcxt.top

Go:   json.Marshal(obj)
来源：http://spz.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://yru.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://jjm.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://chn.0kj1m.cn

Py:   json.loads(s)
来源：http://qhh.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://trq.hywenlv.cn

JS:   JSON.parse(s)
来源：http://kpt.yvedp.cn

TS:   JSON.parse(s)
来源：http://ysb.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nlt.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://mgs.pycfn.com

Ruby: JSON.parse(s)
来源：http://cuw.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mhe.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://lgu.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uwm.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yvn.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nvl.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jrj.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hsb.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://giy.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://qyp.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vbv.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://dee.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://owq.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jwl.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://udc.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xck.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iac.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lax.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rod.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hcj.havefunace.top

[K05] 深拷贝对象
来源：http://vzo.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://rjk.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://uwd.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://owt.andypj.xyz

TS:   structuredClone(obj)
来源：http://apj.shanyushiyangtech.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yms.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qcc.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gru.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yqg.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://zjw.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uwg.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ahc.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://boh.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ldi.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nub.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pko.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lld.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gas.daxiang520.top

[K07] 进制转换
来源：http://xpv.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tox.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pdn.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mas.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://koi.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dfu.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rea.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wrv.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://shj.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://iwi.316326.xyz

Py:   pickle.dumps(obj)
来源：http://vwq.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nor.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://kyu.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://stl.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nyb.yj202588.top

Go:   encoding/gob
来源：http://ukd.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://age.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bez.ctjpmb.com

================================================================================
来源：http://fgw.jyoumei.cn

L. 网络请求
来源：http://jqq.quarkkingdee.top

================================================================================
来源：http://nbb.andypj.xyz

[L01] 发送 GET 请求
来源：http://viu.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wth.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tir.cucudq.cn

JS:   await fetch(url)
来源：http://lrd.shuidangran.top

TS:   await fetch(url)
来源：http://dkq.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://apv.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://hmk.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mgj.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hcv.jqgfzy.top

[L02] 发送 POST JSON
来源：http://oam.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://ceu.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xej.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nef.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jul.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xzk.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uut.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dxs.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hje.ywan-chungtsiang.top


<!-- 参考信息 -->