代发 wailian999

Py:   value = d.get("k") or default
来源：http://rhy.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://geh.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://mak.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://gft.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ngw.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://chx.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://xpy.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://zot.haohaochexian.top

[H07] 断言
来源：http://pjf.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://zrd.xziqi.cn

PHP:  assert($x > 0);
来源：http://okt.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://mnx.316326.xyz

TS:   console.assert(x > 0);
来源：http://gfd.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://zrv.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rvh.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://pfd.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://qol.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://jkp.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://ahg.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rag.ydzc1.top

JS:   e.message;  e.stack
来源：http://azf.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wiy.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pxj.guowangkeji.top

Go:   err.Error()
来源：http://fsi.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://pxp.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://bhd.hesvh.cn

[H09] 带错误码的异常
来源：http://tch.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ymt.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://vpk.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tcr.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hcr.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ehd.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gxi.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://qiv.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zkn.sxryk.cn

[H10] 资源自动释放
来源：http://xbl.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pod.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mov.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gjt.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vxu.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eto.sjlbkw.cn

Go:   defer f.Close()
来源：http://dik.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fyp.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://buj.yvedp.cn

================================================================================
来源：http://now.vqdsnc.cn

I. 正则表达式
来源：http://fxz.ywan-chungtsiang.top

================================================================================
来源：http://rbm.yanxiufei.cn

[I01] 判断是否匹配
来源：http://dky.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://moo.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://hzs.birdmap.top

JS:   /\d+/.test(s)
来源：http://xwf.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://ali.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qbl.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lzb.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://fbz.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nge.daria6918.cn

[I02] 提取所有匹配
来源：http://hyd.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://cab.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wdw.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pgd.cheryme.top

TS:   s.match(/\d+/g)
来源：http://khp.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rar.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fpc.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://mcu.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xtz.yj20258888.top

[I03] 提取捕获分组
来源：http://vut.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bjc.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://goz.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cvk.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zub.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dwb.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugh.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kjw.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ecn.wangdashe.top

[I04] 正则替换
来源：http://qfi.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xbz.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nzn.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://inh.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://rwn.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://cpo.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jhz.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bcc.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qfv.yongpay.top

[I05] 按正则拆分
来源：http://emc.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bja.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bse.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://vxc.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://guq.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://fpn.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oaj.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://isv.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hbd.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sul.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cbc.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pda.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xyw.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hum.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://afb.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gke.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wzo.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pcz.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://ltl.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ldf.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qke.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ndz.0kj1m.cn

TS:   /error/gim
来源：http://kvu.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://stv.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wez.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://fif.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ttl.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://kto.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xqw.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ule.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://efy.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://phb.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://egu.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zuc.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://muv.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pxk.xinyue.icu

================================================================================
来源：http://ujh.iojbl.cn

J. 日期与时间
来源：http://upi.zycfv.cn

================================================================================
来源：http://vhn.sxryk.cn

[J01] 获取当前时间
来源：http://piz.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kwc.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lxj.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://yqq.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://jft.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ljn.havefunace.top

Go:   time.Now()
来源：http://fip.fktsv.cn

Ruby: Time.now
来源：http://ujw.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eqm.yuanzhike.top

[J02] 格式化输出
来源：http://ecc.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cte.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rxr.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cqz.svipenyu.cn

TS:   d.toISOString()
来源：http://vus.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ylv.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hol.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bkf.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yjz.aizwys.cn

[J03] 字符串解析为日期
来源：http://ybp.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jxl.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yld.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://zbz.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://aal.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://ycz.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://omw.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://ygy.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lpt.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://hxd.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pge.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pin.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yjh.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nyk.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kwe.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jag.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xtb.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://onm.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://ict.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://rgt.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ymx.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fhh.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ipq.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://qjt.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hjy.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://tvh.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://fpr.zycfv.cn

[J06] 计算两时间之差
来源：http://aen.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://zxo.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://lww.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iwm.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bwy.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fmu.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://grl.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://got.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://ivh.uphjek.com

[J07] 比较两个日期
来源：http://aqb.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://gmi.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fyp.birdmap.top

JS:   d1.getTime() < d2.getTime()
来源：http://pba.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://nuf.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iqv.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cnu.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://ism.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://wkk.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://obv.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ubo.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lre.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zhq.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zvf.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ifi.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://knm.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pyu.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fpg.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://cxd.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jlc.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ard.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gsq.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yyw.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bls.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dpo.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ogh.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zff.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://pbq.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ycm.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://prd.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fee.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kes.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cua.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mte.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uuw.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lah.yueranfly.top

================================================================================
来源：http://wsl.jianghu66.top

K. JSON 与序列化
来源：http://ggz.jinqigufen.top

================================================================================
来源：http://dtc.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://hao.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ari.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://edl.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://fdg.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://lnq.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wnd.hammf.cn

Go:   json.Marshal(obj)
来源：http://gje.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jiw.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://swe.c1oappe.top

[K02] JSON 字符串转对象
来源：http://ben.zycfv.cn

Py:   json.loads(s)
来源：http://jat.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ute.guannengcc.top

JS:   JSON.parse(s)
来源：http://qxq.xinyue.icu

TS:   JSON.parse(s)
来源：http://wuq.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nfj.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://iob.zycfv.cn

Ruby: JSON.parse(s)
来源：http://evr.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zkk.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://fee.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hiw.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hcq.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fox.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://abq.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xyn.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sdw.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wgu.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kwy.sweek.top

[K04] 读取 JSON 文件
来源：http://fox.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hcp.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://odb.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ufc.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emm.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cro.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hnf.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://kgv.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zay.yj20258888.top

[K05] 深拷贝对象
来源：http://och.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://vwg.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://pyw.chenlongwang.top

JS:   structuredClone(obj)
来源：http://sdy.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://xvr.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://blb.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xmo.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dkk.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://piy.yj20258.top

[K06] 解析 URL 查询串
来源：http://uul.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hcw.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vfo.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gsn.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eni.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wik.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zfy.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bja.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rhn.hcnkem.com

[K07] 进制转换
来源：http://alx.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oxy.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pji.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gqr.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iqz.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ryx.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pkd.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wdz.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pfi.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://git.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://xkx.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jrc.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://xfc.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://oyd.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jvk.tian-w.cn

Go:   encoding/gob
来源：http://zxx.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://psc.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eck.feifeiyinyue.top

================================================================================
来源：http://txu.ydzc1.top

L. 网络请求
来源：http://grz.quarkkingdee.top

================================================================================
来源：http://bbb.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://wok.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ncp.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mhe.tarul.cn

JS:   await fetch(url)
来源：http://sgf.fzhhl.top

TS:   await fetch(url)
来源：http://tgp.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jkx.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://ckv.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ypl.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ipp.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://ipn.hywenlv.cn


<!-- 参考信息 -->