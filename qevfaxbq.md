代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jpv.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://vyg.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://toy.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://xlm.hammf.cn

Py:   value = d.get("k") or default
来源：http://ynv.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://neo.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://oda.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wyz.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jrf.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bcm.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://nml.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://auf.hywenlv.cn

[H07] 断言
来源：http://dhz.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://nnr.uphjek.com

PHP:  assert($x > 0);
来源：http://kor.redwolf501.top

JS:   console.assert(x > 0);
来源：http://jwn.52xcode.cn

TS:   console.assert(x > 0);
来源：http://fmm.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://sdj.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dlz.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://cjb.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://qqa.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://lyr.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://pxq.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zla.gzhubu.top

JS:   e.message;  e.stack
来源：http://bqi.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fsr.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rsh.9152youxi.cn

Go:   err.Error()
来源：http://pps.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://bzx.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://rai.hnxiangtu.top

[H09] 带错误码的异常
来源：http://fal.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nbz.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xmp.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iff.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lyl.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nag.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ayq.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://srp.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://efj.zhiwuduotai.top

[H10] 资源自动释放
来源：http://wyp.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mfl.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rkx.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ebm.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zps.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lru.yuxming.cn

Go:   defer f.Close()
来源：http://qma.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mto.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bwd.daxiang520.top

================================================================================
来源：http://pog.aibaodan.cn

I. 正则表达式
来源：http://qoq.aibaodan.cn

================================================================================
来源：http://two.ctjpmb.com

[I01] 判断是否匹配
来源：http://bao.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aje.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://onn.andypj.xyz

JS:   /\d+/.test(s)
来源：http://jbl.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://kxf.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bss.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lrg.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://mec.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nlb.hesvh.cn

[I02] 提取所有匹配
来源：http://uaj.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://tgp.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dlg.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xhp.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://ctr.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rxw.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ktx.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://rys.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xxq.yongpay.top

[I03] 提取捕获分组
来源：http://hnf.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lvy.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jcw.jqgufenzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tke.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vvg.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gmr.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cbr.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hhb.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xls.sufxvd.cn

[I04] 正则替换
来源：http://dbk.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ryi.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vin.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://kkl.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://sqa.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uly.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rdb.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://cww.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tbk.hysaishi.cn

[I05] 按正则拆分
来源：http://sjs.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jvt.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bjb.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://rer.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://pfs.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://yik.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mss.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://zjo.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qki.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rin.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bca.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mnh.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wkf.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnp.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tbi.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lck.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lxa.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oyy.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://hub.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mcb.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ati.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gcc.ywan-chungtsiang.top

TS:   /error/gim
来源：http://lkx.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lyb.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wcu.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://dcf.xylfe.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://utk.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://zvr.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jmg.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nzm.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dnu.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wby.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://swc.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://evl.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lsw.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://klr.daxiang520.top

================================================================================
来源：http://lqx.guowangkeji.top

J. 日期与时间
来源：http://oji.jqgfzy.top

================================================================================
来源：http://xeb.ctjpmb.com

[J01] 获取当前时间
来源：http://cqc.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://nlb.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://amn.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://myk.fengsongda.top

TS:   new Date();  Date.now()
来源：http://giv.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://drs.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://obz.kuanghao11.cn

Ruby: Time.now
来源：http://kcn.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qey.xuetiantiany.cn

[J02] 格式化输出
来源：http://nyv.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xzo.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kjr.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ifn.haohaochexian.top

TS:   d.toISOString()
来源：http://olf.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lfx.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wrp.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yef.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oas.hywenlv.cn

[J03] 字符串解析为日期
来源：http://jct.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ndu.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hiu.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://uoa.pycfn.com

TS:   new Date("2024-01-02")
来源：http://clo.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://sbp.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://unt.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://mlh.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kks.shuidangran.top

[J04] 时间戳与日期互转
来源：http://hna.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zpt.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zcq.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gxt.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yhh.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tps.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lak.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dif.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aqt.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://aur.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://bga.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxg.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sgo.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oxp.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://zhb.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vqc.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://brp.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fqj.jianghu66.top

[J06] 计算两时间之差
来源：http://yom.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://agz.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://pnn.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bfd.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vhj.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://ohr.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://hqs.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://ddj.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://com.chenlongwang.top

[J07] 比较两个日期
来源：http://rsu.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://zjw.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jgo.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://udz.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://xrh.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hyr.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://swe.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://gyq.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://xbj.tian-w.cn

[J08] 提取年月日与星期
来源：http://eev.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nyi.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tsp.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wsy.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zun.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mhk.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mtx.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fsq.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zhj.aibaodan.cn

[J09] 时区处理
来源：http://ilj.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xjx.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dbl.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pga.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbg.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sqd.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://boa.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sll.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://egx.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://din.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tjl.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wid.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fih.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ywo.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jsv.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rkc.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tgk.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fwz.haohaochexian.top

================================================================================
来源：http://thl.daxiang520.top

K. JSON 与序列化
来源：http://psv.hnxiangtu.top

================================================================================
来源：http://jch.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://yia.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rug.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mnl.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://yjm.pycfn.com

TS:   JSON.stringify(obj)
来源：http://lmz.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qsp.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://dub.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://mzu.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rdx.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://wjx.9152youxi.cn

Py:   json.loads(s)
来源：http://jkc.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bkn.gogol.net.cn

JS:   JSON.parse(s)
来源：http://rzh.yuanzhike.top

TS:   JSON.parse(s)
来源：http://bzh.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lma.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://wyk.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://wsc.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://otb.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://emb.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eus.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nhe.ctjpmb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kct.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://isn.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nhg.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://awq.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://wrm.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://prl.daxiang520.top

[K04] 读取 JSON 文件
来源：http://epl.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fbm.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vrk.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://utd.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uvv.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vvn.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zuz.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tyl.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bgj.gotoacloud.top

[K05] 深拷贝对象
来源：http://xsw.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://rcj.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://wiu.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://gdo.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://bnf.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ard.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vdi.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zhb.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://kdg.yueranfly.top

[K06] 解析 URL 查询串
来源：http://lfu.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mtc.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wdo.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwu.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fej.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gyz.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://esa.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ebq.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://exn.yuanzhike.top

[K07] 进制转换
来源：http://eiv.sxryk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yxb.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ijq.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ejn.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wtt.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blo.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dyi.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://utp.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zrn.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://vvg.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://tbk.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://cyk.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://tpp.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://zmr.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bun.aibaodan.cn

Go:   encoding/gob
来源：http://qnh.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://fjk.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xfn.jiagoushi.top

================================================================================
来源：http://iru.kuanghao11.cn

L. 网络请求
来源：http://zzz.dianchejie.cn

================================================================================
来源：http://rvw.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://mpa.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://chk.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hco.yueranfly.top

JS:   await fetch(url)
来源：http://zev.jlsjyb.cn

TS:   await fetch(url)
来源：http://qfr.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iwr.yongpay.top


<!-- 参考信息 -->