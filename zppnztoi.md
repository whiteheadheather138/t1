代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cyz.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uwa.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://nhf.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://rak.yfazqb.com

[H07] 断言
来源：http://wxn.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://alr.guannengcc.top

PHP:  assert($x > 0);
来源：http://wzy.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://blt.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://cxb.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://lfg.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pll.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ykz.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://ftt.zhoulong.xyz

[H08] 获取错误信息与堆栈
来源：http://oey.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://lwk.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ebm.vehdjk.com

JS:   e.message;  e.stack
来源：http://mgf.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nyt.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bfw.chenlongwang.top

Go:   err.Error()
来源：http://olu.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://lse.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://fuq.zhongyouzk.top

[H09] 带错误码的异常
来源：http://mhu.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mln.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yzs.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oww.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tap.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pct.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oum.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://mxu.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gam.zhixingplan.top

[H10] 资源自动释放
来源：http://zbj.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yls.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vme.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uhg.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bes.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://beq.chenzaomai.com

Go:   defer f.Close()
来源：http://oha.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ymt.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cip.xuetiantiany.cn

================================================================================
来源：http://wmz.fengsongda.top

I. 正则表达式
来源：http://rae.sysykeji.top

================================================================================
来源：http://cwo.jqgfzy.top

[I01] 判断是否匹配
来源：http://ook.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uiu.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rvh.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://zon.sweek.top

TS:   /\d+/.test(s)
来源：http://pyl.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kxe.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hlb.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://hfi.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rhw.sxryk.cn

[I02] 提取所有匹配
来源：http://ctu.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://pvt.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eum.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nyr.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://ypq.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lkq.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wkk.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://zyl.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fza.nanxinkj.top

[I03] 提取捕获分组
来源：http://haw.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ovz.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://slt.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jvp.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ihr.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dfn.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://muq.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vpx.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lgf.9152youxi.cn

[I04] 正则替换
来源：http://mij.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://zmz.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vjg.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://wix.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://ufw.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://ulz.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mcx.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lhu.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://swc.hongshengwenyu.top

[I05] 按正则拆分
来源：http://jqa.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hxs.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nsd.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://pgi.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://fqb.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://ejh.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lwx.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lpe.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mtd.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vki.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xpx.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zwf.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xwl.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qmq.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zgr.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mib.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hyv.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://elo.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://kqr.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lsh.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gif.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sss.jiagoushi.top

TS:   /error/gim
来源：http://fpo.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dzn.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gvm.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://lnb.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://urk.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://ikn.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wlv.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nvc.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://psq.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://urs.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rwq.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://soh.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jra.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://csd.svipenyu.cn

================================================================================
来源：http://vav.yj20258888.top

J. 日期与时间
来源：http://rqz.yj202588.top

================================================================================
来源：http://csx.zhongyouzk.top

[J01] 获取当前时间
来源：http://kqk.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ecf.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tfe.tanke756.top

JS:   new Date();  Date.now()
来源：http://dph.tanke756.top

TS:   new Date();  Date.now()
来源：http://vqv.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mkp.ybcxt.top

Go:   time.Now()
来源：http://ioz.zhijiandao.cn

Ruby: Time.now
来源：http://cux.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xbq.guowangkeji.top

[J02] 格式化输出
来源：http://php.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fcv.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zuc.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lda.yangfankeji.com

TS:   d.toISOString()
来源：http://oin.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jvo.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uqz.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ltf.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hgg.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://jnn.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ohg.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://shq.ivvv.top

JS:   new Date("2024-01-02")
来源：http://hou.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://ldx.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://var.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pow.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://thj.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vsu.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://xox.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oem.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zmf.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rcx.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tiq.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qnv.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://brn.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vyo.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fbk.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://kss.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://czy.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hwq.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbq.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbq.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://vaa.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iby.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://thm.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://wxy.xuanzx.com

[J06] 计算两时间之差
来源：http://yfg.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://gmt.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://bgn.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xhm.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dyd.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://jgf.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://ljf.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://fdj.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://moa.ivvv.top

[J07] 比较两个日期
来源：http://oau.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://ksv.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://saj.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://bjs.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cjp.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yqj.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://psa.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lga.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://zyx.aibaodan.cn

[J08] 提取年月日与星期
来源：http://ijx.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgv.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wdt.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pfx.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vgh.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vth.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vaa.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ibj.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iwp.redwolf501.top

[J09] 时区处理
来源：http://duu.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pcu.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://apq.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emt.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wjg.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tyh.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://paf.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fnh.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aax.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://zid.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://uvu.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ass.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dfj.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dva.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vfy.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vsz.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yzb.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jqn.aibaodan.cn

================================================================================
来源：http://uay.zycfv.cn

K. JSON 与序列化
来源：http://bry.smart0.xyz

================================================================================
来源：http://zyz.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://agw.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://exw.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rlj.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://vix.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://zyf.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ulp.sysykeji.top

Go:   json.Marshal(obj)
来源：http://nyd.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://qln.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jlc.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://ogn.andypj.xyz

Py:   json.loads(s)
来源：http://mit.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eon.nwbrower.top

JS:   JSON.parse(s)
来源：http://dfh.ydzc1.top

TS:   JSON.parse(s)
来源：http://rbf.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://amj.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://win.smart0.xyz

Ruby: JSON.parse(s)
来源：http://jdd.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pfv.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://sum.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gju.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rih.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://svo.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tme.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://exw.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgs.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://cjp.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uni.epnwcf.com

[K04] 读取 JSON 文件
来源：http://cww.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oax.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://psd.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yhf.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tdu.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fql.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mgt.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qrk.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kpn.52xcode.cn

[K05] 深拷贝对象
来源：http://cth.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://ixg.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://myl.hcnkem.com

JS:   structuredClone(obj)
来源：http://xin.cucudq.cn

TS:   structuredClone(obj)
来源：http://oez.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jjx.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eck.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kxf.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eyr.iojbl.cn

[K06] 解析 URL 查询串
来源：http://zrj.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zmv.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://und.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://frg.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivx.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ikw.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://buc.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uvz.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://msg.bjfxy.top

[K07] 进制转换
来源：http://ncr.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://caj.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iqy.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kor.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ldo.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uaj.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lrx.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ajh.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rav.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://uah.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://arr.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cac.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://jmh.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://sfl.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cfx.yj202588.top

Go:   encoding/gob
来源：http://wbf.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://ycz.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yfv.xinyue.icu

================================================================================
来源：http://svo.ctjpmb.com

L. 网络请求
来源：http://iee.svipenyu.cn

================================================================================
来源：http://knx.hnqzz.top

[L01] 发送 GET 请求
来源：http://nmw.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://euc.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fao.zdqjudy.top

JS:   await fetch(url)
来源：http://mkl.hcnkem.com

TS:   await fetch(url)
来源：http://eyj.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://spq.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://exw.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://max.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gyc.yvedp.cn

[L02] 发送 POST JSON
来源：http://grz.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://xxm.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bsu.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nin.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jqw.shzxlz.cn


<!-- 参考信息 -->