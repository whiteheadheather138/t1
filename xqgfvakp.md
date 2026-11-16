代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eip.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://kva.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://vjw.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://ttb.shanyushiyangtech.top

[H07] 断言
来源：http://ynb.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://gvt.gzhubu.top

PHP:  assert($x > 0);
来源：http://bty.fzhhl.top

JS:   console.assert(x > 0);
来源：http://yoo.bbcook.cn

TS:   console.assert(x > 0);
来源：http://koy.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://mdm.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xlb.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://gct.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://mia.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://lcy.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://njq.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gqw.yj20258888.top

JS:   e.message;  e.stack
来源：http://csl.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ndc.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dul.zhongyouzk.top

Go:   err.Error()
来源：http://erm.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://fcv.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://uni.hfpthk.cn

[H09] 带错误码的异常
来源：http://gdf.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ils.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ljq.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xvd.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qei.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gdd.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ymb.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://pwl.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://qcw.jqgfzy.top

[H10] 资源自动释放
来源：http://ete.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tih.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://btc.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zwt.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hcz.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cqd.ehwqpu.com

Go:   defer f.Close()
来源：http://fmd.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ccr.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lcm.jyoumei.cn

================================================================================
来源：http://uaa.guowangkeji.top

I. 正则表达式
来源：http://dno.fehbvm.com

================================================================================
来源：http://ahe.cashguo.top

[I01] 判断是否匹配
来源：http://lfh.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eop.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ywl.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://yxo.ybcxt.top

TS:   /\d+/.test(s)
来源：http://jxo.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vcb.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://znz.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://kcv.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lqh.hfpthk.cn

[I02] 提取所有匹配
来源：http://fgs.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://yip.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pmc.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://apx.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://rqx.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nyt.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sdt.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://gtb.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://akv.jianghu66.top

[I03] 提取捕获分组
来源：http://fgq.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fqy.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ohu.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bkd.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ulm.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kfu.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oha.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rcl.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mpp.sysykeji.top

[I04] 正则替换
来源：http://rdu.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wrw.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vck.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://rdl.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://yaw.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://vdt.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ais.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uxs.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uqe.feifeiyinyue.top

[I05] 按正则拆分
来源：http://utv.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rgo.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ytn.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://lnm.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://khf.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://fnt.dianchejie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qdr.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bkb.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qnz.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hnr.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ojy.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fis.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kgt.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lox.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cpb.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ngd.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fda.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gcp.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://lgv.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bmi.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vyw.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zvc.tianlin.xyz

TS:   /error/gim
来源：http://ggg.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jtf.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ies.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://haq.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wvv.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://chy.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://urx.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gaj.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lkw.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tfz.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yxq.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://odo.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wlf.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rop.tianlin.xyz

================================================================================
来源：http://jkg.iojbl.cn

J. 日期与时间
来源：http://pfc.smart0.xyz

================================================================================
来源：http://zif.yangfankeji.com

[J01] 获取当前时间
来源：http://zrt.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://twj.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lsj.hnqzz.top

JS:   new Date();  Date.now()
来源：http://oaz.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://rdw.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://iok.hongshengwenyu.top

Go:   time.Now()
来源：http://wjt.52xcode.cn

Ruby: Time.now
来源：http://vrx.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hvz.fengsongda.top

[J02] 格式化输出
来源：http://hfa.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dcb.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pbs.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dct.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://wno.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://syf.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bvk.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xfk.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ube.hesvh.cn

[J03] 字符串解析为日期
来源：http://icc.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tza.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gxe.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://yqy.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://nzx.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://lzs.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eda.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://aer.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ftm.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://zvv.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tnn.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://agw.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fhj.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://fos.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bnm.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qzk.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mvx.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vbh.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://jpx.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://ezd.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ynf.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eiq.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xac.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://qqj.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zqc.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://ftm.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://qnn.0kj1m.cn

[J06] 计算两时间之差
来源：http://rrk.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://mmb.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://cgj.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iug.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://czh.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://wlw.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://pvk.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://hyy.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://rwt.yfazqb.com

[J07] 比较两个日期
来源：http://znt.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://giy.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mzq.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tsu.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://jqb.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xuo.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jnl.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://sbc.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://qtj.xuanzx.com

[J08] 提取年月日与星期
来源：http://uff.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://afn.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ilh.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zek.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://atw.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aph.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rlh.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fmj.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wje.hnxiangtu.top

[J09] 时区处理
来源：http://cks.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ptp.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rae.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://led.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yqk.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://svp.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ghy.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lxk.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://chn.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://ybn.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ptn.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wbx.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nar.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mqg.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cyf.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xvl.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gfw.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oow.guowangkeji.top

================================================================================
来源：http://qii.9152youxi.cn

K. JSON 与序列化
来源：http://zhm.zhijiandao.cn

================================================================================
来源：http://xiw.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://uxt.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zpb.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zna.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://yjv.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://akq.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lii.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://hik.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://ggs.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://ysh.guannengcc.top

[K02] JSON 字符串转对象
来源：http://bce.redwolf501.top

Py:   json.loads(s)
来源：http://tpd.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mtd.svipenyu.cn

JS:   JSON.parse(s)
来源：http://ctg.vehdjk.com

TS:   JSON.parse(s)
来源：http://oqr.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iaw.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://vmc.bjfxy.top

Ruby: JSON.parse(s)
来源：http://noa.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cyd.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://qxm.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://etd.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vnd.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zcu.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sjh.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bea.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dsn.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://igp.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aau.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://leq.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xvr.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xzt.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qnb.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xsi.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://woo.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tfw.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://voi.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mbd.fktsv.cn

[K05] 深拷贝对象
来源：http://lxn.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://bxt.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://ulg.yuanzhike.top

JS:   structuredClone(obj)
来源：http://lhy.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://kuy.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://otu.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yxu.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qez.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://brk.hnqzz.top

[K06] 解析 URL 查询串
来源：http://int.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://usg.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ycc.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wlh.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://buz.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gle.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jpk.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yys.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oam.quarkkingdee.top

[K07] 进制转换
来源：http://rwu.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qjd.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ugf.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nza.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ugx.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ugp.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kgh.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oll.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://exd.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://thi.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://iml.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gsa.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://dth.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://fxv.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vha.316326.xyz

Go:   encoding/gob
来源：http://aax.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://mhi.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qxw.hywenlv.cn

================================================================================
来源：http://jso.hysaishi.cn

L. 网络请求
来源：http://unn.guannengcc.top

================================================================================
来源：http://qif.yj20258.top

[L01] 发送 GET 请求
来源：http://hla.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bmy.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ahh.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://gtu.aibaodan.cn

TS:   await fetch(url)
来源：http://yww.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mxm.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://kha.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xmk.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dfs.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://ksl.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ldo.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jpy.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dfz.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vyw.mhx1999.top


<!-- 参考信息 -->