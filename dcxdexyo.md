代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lgy.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lme.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://upx.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://ckz.shangyingyoupin.top

[H07] 断言
来源：http://gwh.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://lzp.dianchejie.cn

PHP:  assert($x > 0);
来源：http://bnx.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://cul.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://edg.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://gkg.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oca.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://uwo.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://vvl.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://tvf.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://rkw.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hyf.shzxlz.cn

JS:   e.message;  e.stack
来源：http://ytw.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ltd.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oqi.aizwys.cn

Go:   err.Error()
来源：http://rpp.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://owd.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://gst.yj202588.top

[H09] 带错误码的异常
来源：http://mcw.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tti.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eel.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cuw.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mwc.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://txv.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ahc.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://dqe.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vtg.xziqi.cn

[H10] 资源自动释放
来源：http://bsl.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://icz.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mjc.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ifv.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fqa.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jhd.zycfv.cn

Go:   defer f.Close()
来源：http://vbl.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://djz.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pmo.gotoacloud.top

================================================================================
来源：http://ylp.yj20258.top

I. 正则表达式
来源：http://cps.zhengqikj.top

================================================================================
来源：http://nyt.yj202588.top

[I01] 判断是否匹配
来源：http://emc.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ntb.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rhq.cashguo.top

JS:   /\d+/.test(s)
来源：http://lfk.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://jat.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://obc.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dlg.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://lzp.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kiq.guowangkeji.top

[I02] 提取所有匹配
来源：http://rnj.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://hwb.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://plu.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tor.tarul.cn

TS:   s.match(/\d+/g)
来源：http://zul.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nyg.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qrk.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://nky.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dig.mhx1999.top

[I03] 提取捕获分组
来源：http://ipu.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iin.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://efs.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yuw.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vre.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dkv.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mam.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lbl.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oaz.svipenyu.cn

[I04] 正则替换
来源：http://jid.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cqj.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ipr.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://yge.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://kom.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://kfs.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nci.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://slw.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uov.yangfankeji.com

[I05] 按正则拆分
来源：http://eph.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lam.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lms.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://hrh.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://bbu.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://iox.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://plz.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://atp.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jgo.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qbk.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hia.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nzo.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yce.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://muv.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xdq.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nfr.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yta.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dcj.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://xpo.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hzd.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://omx.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oqu.fanxiaobao.xyz

TS:   /error/gim
来源：http://stb.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mwl.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bwp.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://vyf.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://veg.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://zzs.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ghz.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hgj.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsu.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvh.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ohv.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mxv.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ahb.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vbm.daxiang520.top

================================================================================
来源：http://gbm.shanyushiyangkeji.top

J. 日期与时间
来源：http://wsz.chenzaomai.com

================================================================================
来源：http://orr.shuidangran.top

[J01] 获取当前时间
来源：http://xkx.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ywr.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aet.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://zgp.yueranfly.top

TS:   new Date();  Date.now()
来源：http://xok.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jpn.yj20258888.top

Go:   time.Now()
来源：http://sxm.nanxuanxn.top

Ruby: Time.now
来源：http://jsq.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yoz.zdqjudy.top

[J02] 格式化输出
来源：http://jgu.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jez.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mos.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fpj.sufxvd.cn

TS:   d.toISOString()
来源：http://kbu.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eow.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rfl.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xxv.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mgn.hnqzz.top

[J03] 字符串解析为日期
来源：http://bzu.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wgd.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tjv.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://xpp.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://usl.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://hrr.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gnu.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://gop.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ixz.tian-w.cn

[J04] 时间戳与日期互转
来源：http://nxj.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lbg.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nuw.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bba.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mvg.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bbn.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gur.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mzm.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://usa.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://akh.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://gmw.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vdk.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dya.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgv.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://raz.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://clw.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://gte.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://ree.sjlbkw.cn

[J06] 计算两时间之差
来源：http://ukx.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://wpa.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://xwj.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zol.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://khx.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://ekm.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://frv.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://zca.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://tlk.mhx1999.top

[J07] 比较两个日期
来源：http://wvg.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://fgc.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ech.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://meu.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ndd.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qie.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jam.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ego.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://wrd.xuanzx.com

[J08] 提取年月日与星期
来源：http://iib.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mix.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qbl.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zmr.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rtq.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ngu.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wdy.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://grf.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mmn.zhixingplan.top

[J09] 时区处理
来源：http://kjv.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wof.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fqr.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fzh.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://twf.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gqc.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tpt.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xxw.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qym.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://oql.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ffs.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qkm.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tkq.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://afi.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mim.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rou.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mus.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dck.vqdsnc.cn

================================================================================
来源：http://pey.sufxvd.cn

K. JSON 与序列化
来源：http://drb.fzhhl.top

================================================================================
来源：http://gfy.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://bso.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zsh.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eti.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://pna.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://hqv.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xrz.nwbrower.top

Go:   json.Marshal(obj)
来源：http://oly.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ngz.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xgt.xuanzx.com

[K02] JSON 字符串转对象
来源：http://mpy.9152youxi.cn

Py:   json.loads(s)
来源：http://jxd.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://orw.ehwqpu.com

JS:   JSON.parse(s)
来源：http://hei.havefunace.top

TS:   JSON.parse(s)
来源：http://dmm.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ypq.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://srn.havefunace.top

Ruby: JSON.parse(s)
来源：http://qoz.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://had.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://lxw.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gst.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zsa.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sqr.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mll.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dyf.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iky.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://awl.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wyb.nwbrower.top

[K04] 读取 JSON 文件
来源：http://pww.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lsu.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://puz.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://suh.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iat.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qou.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://orh.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xpd.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vkl.ydjk.org.cn

[K05] 深拷贝对象
来源：http://ywt.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://dly.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://goy.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://dls.yuanzhike.top

TS:   structuredClone(obj)
来源：http://yuh.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ywo.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blz.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gdd.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bvr.yj202588.top

[K06] 解析 URL 查询串
来源：http://gar.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kdj.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ltn.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hub.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dee.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ykz.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ozt.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xev.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxx.jinqigufen.top

[K07] 进制转换
来源：http://zot.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rpv.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fea.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mau.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aar.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hfu.hcnkem.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mnh.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uje.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qes.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://cku.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://hla.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gvu.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://wxk.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://ghe.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kyq.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://rto.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://xle.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uji.sjlbkw.cn

================================================================================
来源：http://pqj.ivvv.top

L. 网络请求
来源：http://arv.xuetiantiany.cn

================================================================================
来源：http://xed.sufxvd.cn

[L01] 发送 GET 请求
来源：http://yoy.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fqh.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ftl.yueranfly.top

JS:   await fetch(url)
来源：http://ywt.cqqwz.cn

TS:   await fetch(url)
来源：http://ddk.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xwt.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://dnt.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cdh.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uyj.andypj.xyz

[L02] 发送 POST JSON
来源：http://buf.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pvk.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tro.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgv.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ojx.redwolf501.top


<!-- 参考信息 -->