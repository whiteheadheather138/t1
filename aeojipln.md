代发 wailian999

TS:   console.assert(x > 0);
来源：http://jtb.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://kkv.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qfs.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lvm.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://nnh.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://fdd.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://tnf.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lle.aizwys.cn

JS:   e.message;  e.stack
来源：http://tvq.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uwx.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ayi.kuanghao11.cn

Go:   err.Error()
来源：http://cui.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://kmp.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://atv.xuanzx.com

[H09] 带错误码的异常
来源：http://tud.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pvz.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sqr.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mlp.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kvp.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://utg.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gsi.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://amf.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://gmd.sysykeji.top

[H10] 资源自动释放
来源：http://vxd.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://yhu.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hbb.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zxf.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ezj.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ara.yj20258.top

Go:   defer f.Close()
来源：http://lsq.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://opk.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nxa.fanxiaobao.xyz

================================================================================
来源：http://itt.vehdjk.com

I. 正则表达式
来源：http://ozz.zhengqikj.top

================================================================================
来源：http://sdx.gaohongyu789.top

[I01] 判断是否匹配
来源：http://alc.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jtd.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uve.nwbrower.top

JS:   /\d+/.test(s)
来源：http://kfq.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://zcn.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dnh.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://clx.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://qjs.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yyq.vqdsnc.cn

[I02] 提取所有匹配
来源：http://rzr.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://aen.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jcz.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jbk.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://xtb.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fdo.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hno.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://ith.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vvu.nanxinkj.top

[I03] 提取捕获分组
来源：http://wsx.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fls.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gvo.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hmp.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fdx.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dfq.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rgk.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://skn.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://drd.52xcode.cn

[I04] 正则替换
来源：http://yzy.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://mgd.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zfs.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tgh.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://lqg.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ohx.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://mxq.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ylr.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lfh.bjfxy.top

[I05] 按正则拆分
来源：http://iav.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zpm.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ivu.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://duu.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://kwd.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://yes.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wvs.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://rwz.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kzr.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qpd.zhiwuduotai.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pre.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jva.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fgj.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hur.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vhe.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zaw.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tye.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kzq.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://epa.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ohc.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xdy.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aso.pycfn.com

TS:   /error/gim
来源：http://kkd.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qtb.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gkm.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://dtk.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iay.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://bux.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ubv.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://unp.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tyx.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfv.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://iki.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tnc.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zul.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rjt.vehdjk.com

================================================================================
来源：http://jat.chenlongwang.top

J. 日期与时间
来源：http://xqv.fktsv.cn

================================================================================
来源：http://rfa.tarul.cn

[J01] 获取当前时间
来源：http://iob.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mnn.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aie.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://jxs.xuanzx.com

TS:   new Date();  Date.now()
来源：http://fas.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ncc.jinyuanbaomall.cn

Go:   time.Now()
来源：http://mws.ctjpmb.com

Ruby: Time.now
来源：http://uqd.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vhm.ehwqpu.com

[J02] 格式化输出
来源：http://rar.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://upq.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hjc.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mnw.iojbl.cn

TS:   d.toISOString()
来源：http://ruj.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mys.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wjg.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lag.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bwx.xylfe.cn

[J03] 字符串解析为日期
来源：http://eii.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cdw.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://clu.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://eum.cashguo.top

TS:   new Date("2024-01-02")
来源：http://yyw.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://vee.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hxt.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://dmg.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yth.ivvv.top

[J04] 时间戳与日期互转
来源：http://ccf.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hul.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tpu.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://juk.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://zjq.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xgr.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://waw.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dzd.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://njh.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://oqs.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://elz.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hyt.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tth.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sme.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://kqn.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jsy.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://vsy.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://doy.jyoumei.cn

[J06] 计算两时间之差
来源：http://pcx.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://xmc.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://vsq.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jik.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cbg.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ccf.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://rpf.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://tpw.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://krp.sysykeji.top

[J07] 比较两个日期
来源：http://pja.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://lam.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pij.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://pps.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://nmt.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aib.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ymn.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://fxe.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://sht.jiagoushi.top

[J08] 提取年月日与星期
来源：http://psr.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gxv.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://obx.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://skg.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ntb.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cam.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jer.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lud.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hkb.mhx1999.top

[J09] 时区处理
来源：http://rxx.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ukg.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xkf.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oso.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qzm.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://smg.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhj.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wlq.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hci.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://nhp.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://abe.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uvh.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wha.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iqu.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ibx.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zkb.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rda.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ggp.jinqigfzy.top

================================================================================
来源：http://bpn.yfazqb.com

K. JSON 与序列化
来源：http://ezu.ybcxt.top

================================================================================
来源：http://zug.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://nqi.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qsj.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://avx.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://ijh.sweek.top

TS:   JSON.stringify(obj)
来源：http://kli.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://req.epnwcf.com

Go:   json.Marshal(obj)
来源：http://wsn.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://viy.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lko.mhx1999.top

[K02] JSON 字符串转对象
来源：http://cid.xinyue.icu

Py:   json.loads(s)
来源：http://dts.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hpx.c1oappe.top

JS:   JSON.parse(s)
来源：http://jda.jyoumei.cn

TS:   JSON.parse(s)
来源：http://itq.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aef.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://aog.cucudq.cn

Ruby: JSON.parse(s)
来源：http://bqz.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xfh.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://xyy.yonumen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ttv.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uwl.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://eej.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jur.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kqr.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vor.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://nra.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bzb.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://zme.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ika.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ucu.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jki.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yjv.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hdu.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iiv.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mvb.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mlj.yongpay.top

[K05] 深拷贝对象
来源：http://hgl.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://gou.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://xda.yangfankeji.com

JS:   structuredClone(obj)
来源：http://prt.zhengqikj.top

TS:   structuredClone(obj)
来源：http://qij.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://las.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mjq.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ukv.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xtr.yonumen.top

[K06] 解析 URL 查询串
来源：http://mtd.hnxiangtu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nts.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pbp.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jiv.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fre.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://veu.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nyt.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://brc.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iuh.birdmap.top

[K07] 进制转换
来源：http://fzf.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hpz.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pni.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kpq.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rwf.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sff.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lxm.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xrr.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ctz.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://mza.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://zbd.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gso.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://irx.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://lpx.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gxn.sysykeji.top

Go:   encoding/gob
来源：http://ueb.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://ppu.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://msu.jinghuilouyu.cn

================================================================================
来源：http://mxq.dashuyun.cn

L. 网络请求
来源：http://eez.jianghu66.top

================================================================================
来源：http://jsn.nwbrower.top

[L01] 发送 GET 请求
来源：http://qwp.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lmo.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jjs.daria6918.cn

JS:   await fetch(url)
来源：http://wdp.hnqzz.top

TS:   await fetch(url)
来源：http://zzm.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gkm.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://mfs.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://blq.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sfl.wangdashe.top

[L02] 发送 POST JSON
来源：http://yti.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kjp.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yph.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lst.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsj.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dcg.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yti.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ncu.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uir.yongpay.top

[L03] 设置自定义请求头
来源：http://grh.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lqe.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://epn.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gna.hnxiangtu.top


<!-- 参考信息 -->