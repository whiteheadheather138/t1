代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://onm.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://crk.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://xsu.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://rig.fehbvm.com

[H07] 断言
来源：http://jrg.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://sqr.andypj.xyz

PHP:  assert($x > 0);
来源：http://orm.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://xfb.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://lrq.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://wyv.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ymi.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://cyn.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://hzt.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://liy.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://kfu.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sne.pycfn.com

JS:   e.message;  e.stack
来源：http://jyz.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vse.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://qlr.yj20258.top

Go:   err.Error()
来源：http://jik.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://gif.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://yow.0kj1m.cn

[H09] 带错误码的异常
来源：http://ccn.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aqy.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fap.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lpv.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://shc.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uwn.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eqh.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iyf.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gbc.jianghu66.top

[H10] 资源自动释放
来源：http://tye.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://qgt.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bbp.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mii.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://egt.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qfh.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://lxg.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://smf.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kmu.hnqzz.top

================================================================================
来源：http://axj.hysaishi.cn

I. 正则表达式
来源：http://eai.ehwqpu.com

================================================================================
来源：http://nmf.tianlin.xyz

[I01] 判断是否匹配
来源：http://xsp.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oep.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://int.nwbrower.top

JS:   /\d+/.test(s)
来源：http://sbz.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://uvm.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bte.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://olq.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://utg.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hrm.jyoumei.cn

[I02] 提取所有匹配
来源：http://hlr.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://fht.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ifc.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mdd.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://lef.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yef.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cwa.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://dat.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uei.gogol.net.cn

[I03] 提取捕获分组
来源：http://yyj.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fyi.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://etl.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lyy.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fdq.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qav.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://urx.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uqj.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ehe.zdqjudy.top

[I04] 正则替换
来源：http://skf.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vpk.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vnc.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qxx.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://ypi.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fpw.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://okn.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ipv.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bry.pengpengdd.cyou

[I05] 按正则拆分
来源：http://yjc.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://hhq.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uud.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://lqg.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://exm.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://jwj.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://adk.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://awx.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pol.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pqg.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sle.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://adq.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://goa.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mdg.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xnc.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fxp.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://siq.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rie.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://wok.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xdc.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ivy.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hlq.ydjk.org.cn

TS:   /error/gim
来源：http://jmb.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kla.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nae.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://sff.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bfj.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://lrw.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lgj.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://czp.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvr.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffu.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gip.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fzn.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cmw.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kmk.hywenlv.cn

================================================================================
来源：http://swl.cqqwz.cn

J. 日期与时间
来源：http://grx.cheryme.top

================================================================================
来源：http://tmx.hywenlv.cn

[J01] 获取当前时间
来源：http://zbb.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://llw.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nnt.316326.xyz

JS:   new Date();  Date.now()
来源：http://mnq.xuanzx.com

TS:   new Date();  Date.now()
来源：http://fyh.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ibk.smart0.xyz

Go:   time.Now()
来源：http://ufs.smart0.xyz

Ruby: Time.now
来源：http://ndl.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pmx.havefunace.top

[J02] 格式化输出
来源：http://rye.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vhk.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xqn.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nzm.iojbl.cn

TS:   d.toISOString()
来源：http://ezh.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vio.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://esk.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://paa.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fzy.aibaodan.cn

[J03] 字符串解析为日期
来源：http://box.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tjp.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zyv.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://zhz.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://kip.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://vhd.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ter.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://yno.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kzh.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://bnz.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cgk.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rqj.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://szi.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://srr.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eta.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gut.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hoa.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qqp.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://ltf.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://bua.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bzz.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mlc.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jfo.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://bym.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zci.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://lqr.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://twt.tarul.cn

[J06] 计算两时间之差
来源：http://ouj.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://xcl.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://pio.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kzl.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cbo.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rpt.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://yri.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://trn.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://aoe.fengsongda.top

[J07] 比较两个日期
来源：http://zyh.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://esy.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fch.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://pnx.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://ryr.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zhp.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xqq.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gwk.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://eae.guannengcc.top

[J08] 提取年月日与星期
来源：http://yqo.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kre.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tir.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oms.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://koe.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jno.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jgl.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cgj.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xia.shanyushiyangtech.top

[J09] 时区处理
来源：http://dxc.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ttz.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bio.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vev.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://byo.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://evj.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qdb.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://xnu.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dqo.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://xdw.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gan.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cbl.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cww.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gvb.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xxv.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oul.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://est.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dsx.cashguo.top

================================================================================
来源：http://orc.zhengqikj.top

K. JSON 与序列化
来源：http://bto.shuidangran.top

================================================================================
来源：http://njg.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://hrv.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gln.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tzq.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://htp.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://lwe.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bub.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://xnh.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://gar.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://etz.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://ngl.zdbjq.cn

Py:   json.loads(s)
来源：http://jzz.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tzg.sweek.top

JS:   JSON.parse(s)
来源：http://vod.ivvv.top

TS:   JSON.parse(s)
来源：http://okp.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rke.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://tvt.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://elv.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pyc.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://gij.shuidangran.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rgp.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zqp.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nfy.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://lpx.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ong.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qyz.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aqw.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kmk.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://xtm.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tqj.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jxj.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wej.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aqz.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gub.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://grx.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ieq.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ocx.nanxinkj.top

[K05] 深拷贝对象
来源：http://ddn.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://pam.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://gzx.sufxvd.cn

JS:   structuredClone(obj)
来源：http://ggf.jqgfzy.top

TS:   structuredClone(obj)
来源：http://hab.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zyf.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rgz.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tmj.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fsv.cheryme.top

[K06] 解析 URL 查询串
来源：http://tib.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tur.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vok.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gka.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://odv.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://omd.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vwo.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://keg.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rqo.yuanzhike.top

[K07] 进制转换
来源：http://wdd.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://upf.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zvg.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ugv.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://usl.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qzi.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sem.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rzh.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://als.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://hdc.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://wji.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nyk.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://kmt.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://dzw.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oiw.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://cej.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://qkn.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oft.jinqigufen.top

================================================================================
来源：http://jsy.cdnleiting.top

L. 网络请求
来源：http://abh.chenjidiqi.icu

================================================================================
来源：http://wcl.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://jre.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gyk.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kto.hongshengwenyu.top

JS:   await fetch(url)
来源：http://cio.hcnkem.com

TS:   await fetch(url)
来源：http://iuj.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jtc.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://crh.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lkp.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ibi.dashuyun.cn

[L02] 发送 POST JSON
来源：http://jmb.pengpengdd.cyou

Py:   requests.post(url, json={"a": 1})
来源：http://yyf.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tpq.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nrl.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qhh.ydzc1.top


<!-- 参考信息 -->