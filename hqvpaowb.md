代发 wailian999

Py:   value = d.get("k") or default
来源：http://dtm.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rdz.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://wxt.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://gcp.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fjc.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://byz.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://fji.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://ere.yanxiufei.cn

[H07] 断言
来源：http://pdk.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://yzh.yongpay.top

PHP:  assert($x > 0);
来源：http://rpv.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://tay.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://alf.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://cgi.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ahy.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://vui.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://bkl.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://vpw.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://jrh.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vnd.ehwqpu.com

JS:   e.message;  e.stack
来源：http://swr.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cik.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://gmi.xinyue.icu

Go:   err.Error()
来源：http://ecq.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://mix.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://qne.gogol.net.cn

[H09] 带错误码的异常
来源：http://vnv.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lle.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xij.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uhv.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nkn.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sna.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nti.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lku.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mqr.hammf.cn

[H10] 资源自动释放
来源：http://ztq.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqh.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gok.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sgc.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sqt.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fjs.fzhhl.top

Go:   defer f.Close()
来源：http://kvz.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uqe.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gfm.shanyushiyangkeji.top

================================================================================
来源：http://gcr.jinghuilouyu.cn

I. 正则表达式
来源：http://elm.ehwqpu.com

================================================================================
来源：http://rke.sysykeji.top

[I01] 判断是否匹配
来源：http://urk.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wpt.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fwh.vehdjk.com

JS:   /\d+/.test(s)
来源：http://kms.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://fnw.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tmz.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fgy.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://hfe.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cnu.jinqigfzy.top

[I02] 提取所有匹配
来源：http://kzp.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://cwf.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://txk.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vgx.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://pir.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wej.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rjg.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://yzx.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://izo.aibaodan.cn

[I03] 提取捕获分组
来源：http://ras.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jjz.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hct.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xrh.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lko.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tua.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rjf.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ztn.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xeo.yueranfly.top

[I04] 正则替换
来源：http://ayg.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://hgd.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azo.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://zqm.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://lxs.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://dgj.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://gyy.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pzo.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yaa.smart0.xyz

[I05] 按正则拆分
来源：http://qsj.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://stu.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uui.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://bsp.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://gbm.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://boa.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vmz.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://trn.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qrk.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jwf.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cth.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ioz.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zsu.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mfw.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zrw.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ulq.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gqf.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zzx.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://vre.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zfn.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ylc.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xqw.xziqi.cn

TS:   /error/gim
来源：http://vbj.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wxq.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qpt.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://erz.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hqr.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://emf.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nim.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://daf.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blx.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vzr.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://apl.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jjz.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lyj.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://chx.hesvh.cn

================================================================================
来源：http://vey.hcnkem.com

J. 日期与时间
来源：http://owq.havefunace.top

================================================================================
来源：http://dbg.yj20258.top

[J01] 获取当前时间
来源：http://twg.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vzv.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://upd.yj202588.top

JS:   new Date();  Date.now()
来源：http://cpq.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://plh.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vkd.sjlbkw.cn

Go:   time.Now()
来源：http://qqf.kuanghao11.cn

Ruby: Time.now
来源：http://yvt.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wnv.tanke756.top

[J02] 格式化输出
来源：http://hol.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sgj.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ckt.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dhx.jqgfzy.top

TS:   d.toISOString()
来源：http://wpv.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nqz.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sxz.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wro.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hci.aizwys.cn

[J03] 字符串解析为日期
来源：http://ptl.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dxp.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gam.birdmap.top

JS:   new Date("2024-01-02")
来源：http://szh.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://fdl.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://czh.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vcv.9152youxi.cn

Ruby: Date.parse("2024-01-02")
来源：http://tje.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fbx.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://ktv.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://css.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://udh.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mna.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vbv.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ntf.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xee.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gga.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vby.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://mkf.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://vmv.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dna.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jtp.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qlo.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://gon.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vwf.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://own.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iin.ctjpmb.com

[J06] 计算两时间之差
来源：http://jxp.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://vvg.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://net.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rbh.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gcw.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://wex.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://wxb.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://snc.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://zfl.jianghu66.top

[J07] 比较两个日期
来源：http://oqw.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://qls.meibo888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ooa.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://pkx.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://hra.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://svm.0kj1m.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://idi.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oyu.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://imu.fzhhl.top

[J08] 提取年月日与星期
来源：http://qek.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ifk.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xgr.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jlz.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zdk.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ria.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dwb.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nqr.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vrg.yfazqb.com

[J09] 时区处理
来源：http://dcf.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uxo.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zam.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dyh.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://utz.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lev.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eax.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cnu.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ika.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://msp.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uxv.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vsr.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wwk.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jvb.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qow.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nqm.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ujp.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wug.haohaochexian.top

================================================================================
来源：http://moy.cashguo.top

K. JSON 与序列化
来源：http://ipe.uphjek.com

================================================================================
来源：http://hso.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://cnm.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://twx.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://utc.yonumen.top

JS:   JSON.stringify(obj)
来源：http://vbt.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://lix.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bml.nwbrower.top

Go:   json.Marshal(obj)
来源：http://lwa.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://udu.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zxi.smart0.xyz

[K02] JSON 字符串转对象
来源：http://tog.c1oappe.top

Py:   json.loads(s)
来源：http://jou.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://alq.daxiang520.top

JS:   JSON.parse(s)
来源：http://kvr.vehdjk.com

TS:   JSON.parse(s)
来源：http://ltf.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bpm.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://vlr.hcnkem.com

Ruby: JSON.parse(s)
来源：http://htl.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://enr.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://wbc.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kxd.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xcs.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://btb.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zgu.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nis.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dup.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nqj.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mak.cashguo.top

[K04] 读取 JSON 文件
来源：http://kme.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://quc.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xku.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ner.sjlbkw.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sru.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vjj.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lbg.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://viu.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lsd.jiagoushi.top

[K05] 深拷贝对象
来源：http://vec.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://tbf.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://hav.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://rss.zdqjudy.top

TS:   structuredClone(obj)
来源：http://jjx.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bxc.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ttk.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rfr.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://szx.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://jcq.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hee.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://urr.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qws.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qpq.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xgr.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tet.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zha.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xsa.nwbrower.top

[K07] 进制转换
来源：http://jmb.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ozi.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cez.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oev.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hiq.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wyn.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://agg.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://trp.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ywk.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://tur.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://isq.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iuq.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://oql.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://mlk.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://klo.haohaochexian.top

Go:   encoding/gob
来源：http://ati.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://feu.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ytj.chenlongwang.top

================================================================================
来源：http://wrq.zhaomingkeji.xyz

L. 网络请求
来源：http://iiy.fengsongda.top

================================================================================
来源：http://pbq.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://wtx.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gnm.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jiv.fzhhl.top

JS:   await fetch(url)
来源：http://smy.yuanzhike.top

TS:   await fetch(url)
来源：http://kch.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oix.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://tyw.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ksn.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dbt.9152youxi.cn

[L02] 发送 POST JSON
来源：http://qoj.birdmap.top


<!-- 参考信息 -->