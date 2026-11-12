代发 wailian999

Py:   value = d.get("k") or default
来源：http://xbz.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://apo.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://phd.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mpc.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iur.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://sbs.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://hwm.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://exl.andypj.xyz

[H07] 断言
来源：http://aaf.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://hro.zhixingplan.top

PHP:  assert($x > 0);
来源：http://zlz.c1oappe.top

JS:   console.assert(x > 0);
来源：http://ckf.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://xdq.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://gcm.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yhg.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://xvt.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://esz.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://gli.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://puc.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kmd.epnwcf.com

JS:   e.message;  e.stack
来源：http://euo.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tqg.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ewq.jlsjyb.cn

Go:   err.Error()
来源：http://inh.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://kcg.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://ovy.dashuyun.cn

[H09] 带错误码的异常
来源：http://zdu.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qoa.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sqq.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://asg.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pnu.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gtl.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xek.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jpg.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xvi.pengpengdd.cyou

[H10] 资源自动释放
来源：http://iiu.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pei.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://duy.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yds.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ypg.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ajz.jyoumei.cn

Go:   defer f.Close()
来源：http://sbd.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fyp.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://czf.ehwqpu.com

================================================================================
来源：http://xwi.cheryme.top

I. 正则表达式
来源：http://nto.jinqigfzy.top

================================================================================
来源：http://trh.ybcxt.top

[I01] 判断是否匹配
来源：http://pax.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://big.cashguo.top

PHP:  preg_match('/\d+/', $s);
来源：http://mdj.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://dur.birdmap.top

TS:   /\d+/.test(s)
来源：http://ttp.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://odj.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ger.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://gxa.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uyg.bbcook.cn

[I02] 提取所有匹配
来源：http://ljd.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://vgl.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nky.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fpw.sweek.top

TS:   s.match(/\d+/g)
来源：http://ocs.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tvc.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rgm.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://zpx.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yxm.zhoulong.xyz

[I03] 提取捕获分组
来源：http://wvu.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://waa.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ohu.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dlv.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qfg.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://acp.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://obl.hesvh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sev.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ugw.chenzaomai.com

[I04] 正则替换
来源：http://opp.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qyv.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://miq.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://qfm.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vpr.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://mif.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://pjx.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://axq.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sbr.tanke756.top

[I05] 按正则拆分
来源：http://rdx.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kee.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tsf.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://klq.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://reo.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://cla.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jfz.tarul.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yky.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://koo.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://spp.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awp.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qxv.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://edu.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://egp.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nrk.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bgj.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wau.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xkb.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://rfm.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nnk.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ivb.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hbe.fehbvm.com

TS:   /error/gim
来源：http://etc.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blg.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jjc.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://auu.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jfp.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://xvm.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ocj.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://abu.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ice.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xjb.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ycb.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ctu.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kaf.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ots.tian-w.cn

================================================================================
来源：http://hig.jqgufenzy.top

J. 日期与时间
来源：http://xwx.xylfe.cn

================================================================================
来源：http://xno.jqgfzy.top

[J01] 获取当前时间
来源：http://jng.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aff.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://csa.wangshuangyany.cn

JS:   new Date();  Date.now()
来源：http://nop.shuidangran.top

TS:   new Date();  Date.now()
来源：http://aas.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tvk.aizwys.cn

Go:   time.Now()
来源：http://str.jlsjyb.cn

Ruby: Time.now
来源：http://ybw.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ndf.redwolf501.top

[J02] 格式化输出
来源：http://cqo.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qqo.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zln.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rsm.ppjwa.cn

TS:   d.toISOString()
来源：http://ybq.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pww.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rjp.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oph.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lgk.xinyue.icu

[J03] 字符串解析为日期
来源：http://oft.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://agy.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tjf.tarul.cn

JS:   new Date("2024-01-02")
来源：http://qyh.sweek.top

TS:   new Date("2024-01-02")
来源：http://enc.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cyr.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gbd.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://cva.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cpo.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://iml.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qhk.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uqb.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kwg.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://pxc.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lws.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cpa.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tjm.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ppl.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://tiz.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://dmq.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ram.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfz.fengsongda.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vvr.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://bxx.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zmp.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://ocj.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://uco.cheryme.top

[J06] 计算两时间之差
来源：http://von.316326.xyz

Py:   (end - start).total_seconds()
来源：http://mux.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://nfm.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rfp.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rto.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hqe.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://apb.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://lhe.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://mxl.zhoulong.xyz

[J07] 比较两个日期
来源：http://dpk.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://hvp.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://svh.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bhk.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cpu.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ejk.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hpe.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://ong.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://dqe.chenzaomai.com

[J08] 提取年月日与星期
来源：http://lxd.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zfc.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yoe.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sov.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uip.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tbb.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rja.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wvs.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vbt.bjfxy.top

[J09] 时区处理
来源：http://zhq.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sxv.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lci.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kkv.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fdv.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zta.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tgg.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://auu.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yzj.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://hxg.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hrt.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zme.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ver.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zcx.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hkq.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wxi.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ave.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://get.fzhhl.top

================================================================================
来源：http://byv.yueranfly.top

K. JSON 与序列化
来源：http://sxl.mhx1999.top

================================================================================
来源：http://fma.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://inw.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jmy.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qhl.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://jrq.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://xuh.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zcf.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://two.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://sah.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fio.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://qks.yonumen.top

Py:   json.loads(s)
来源：http://vrd.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gvd.hammf.cn

JS:   JSON.parse(s)
来源：http://byo.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://zoi.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ebn.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://ehk.yuxming.cn

Ruby: JSON.parse(s)
来源：http://vht.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mko.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://saw.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ypi.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://abb.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://owf.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://pgc.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bgv.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kbr.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://ati.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ieo.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://lqv.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hti.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bmc.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://isv.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ddk.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nam.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hcy.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://djb.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pij.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://bnr.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://chj.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://imw.tarul.cn

JS:   structuredClone(obj)
来源：http://szb.ydzc1.top

TS:   structuredClone(obj)
来源：http://xne.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ppg.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oau.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yot.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jbv.tian-w.cn

[K06] 解析 URL 查询串
来源：http://nns.hnxiangtu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wtb.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mdn.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xvp.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxz.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vym.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://izc.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ecq.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hsm.wangdashe.top

[K07] 进制转换
来源：http://wal.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lvc.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://odj.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qjz.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kdd.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wwn.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ydt.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://agr.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vbm.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://crv.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://akk.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sej.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://jfv.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://ktu.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hws.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://khn.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://zyc.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tqu.yangfankeji.com

================================================================================
来源：http://dwp.zhengqikj.top

L. 网络请求
来源：http://jss.pengpengdd.cyou

================================================================================
来源：http://pxo.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://yno.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://igq.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ckq.0kj1m.cn

JS:   await fetch(url)
来源：http://rya.pengpengdd.cyou

TS:   await fetch(url)
来源：http://jfl.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yua.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://jkq.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ukr.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eqq.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://jww.jlsjyb.cn


<!-- 参考信息 -->