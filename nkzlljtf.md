代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uyx.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eow.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://zdj.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://mpl.zdbjq.cn

[H07] 断言
来源：http://pzh.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://wxs.tian-w.cn

PHP:  assert($x > 0);
来源：http://fjj.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://qzt.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://ioh.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://isx.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hap.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://pqq.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://zzz.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://vqd.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://hyt.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ckx.hysaishi.cn

JS:   e.message;  e.stack
来源：http://dee.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tah.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cby.bbcook.cn

Go:   err.Error()
来源：http://yol.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://psl.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://rzi.aibaodan.cn

[H09] 带错误码的异常
来源：http://wkr.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oya.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hnr.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zys.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oko.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xcj.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nye.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://hcr.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://myk.cashguo.top

[H10] 资源自动释放
来源：http://ski.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ngp.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yij.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jaa.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fqy.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zgd.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://ska.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://heb.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nud.yj20258.top

================================================================================
来源：http://mlc.sufxvd.cn

I. 正则表达式
来源：http://ahm.havefunace.top

================================================================================
来源：http://ixa.tarul.cn

[I01] 判断是否匹配
来源：http://aja.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yaq.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hkt.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://jmc.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://rkq.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lpq.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gae.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://cvo.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cpx.zhixingplan.top

[I02] 提取所有匹配
来源：http://rcl.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://odo.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://txy.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://icn.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://tny.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://whq.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ujr.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://kfr.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hgq.mhx1999.top

[I03] 提取捕获分组
来源：http://wmv.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rrf.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wwr.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nbd.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xdm.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ymp.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rdu.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nln.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://seb.wangshuangyany.cn

[I04] 正则替换
来源：http://oqc.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://muj.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uyq.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://yxf.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hsq.gogol.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gar.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ika.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tnp.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tor.tianlin.xyz

[I05] 按正则拆分
来源：http://lto.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rzi.xziqi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xuq.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://yio.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://tjr.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://rna.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zke.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://eba.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lee.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://myp.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xhw.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zpm.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rvo.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lbw.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rqf.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hci.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yjp.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ajc.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://rvo.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qlv.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qgy.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vie.gotoacloud.top

TS:   /error/gim
来源：http://mnu.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ois.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ofu.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://cep.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qbv.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://vvm.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://khp.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://moi.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lpf.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://npf.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://upf.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fkg.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rhi.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://alq.ydzc1.top

================================================================================
来源：http://ddd.quarkkingdee.top

J. 日期与时间
来源：http://ikg.guowangkeji.top

================================================================================
来源：http://wpt.zhongyouzk.top

[J01] 获取当前时间
来源：http://kta.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uzq.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jyy.52xcode.cn

JS:   new Date();  Date.now()
来源：http://bed.fzhhl.top

TS:   new Date();  Date.now()
来源：http://hbs.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rcq.ywan-chungtsiang.top

Go:   time.Now()
来源：http://kpn.aibaodan.cn

Ruby: Time.now
来源：http://ffs.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nsd.jiagoushi.top

[J02] 格式化输出
来源：http://qtj.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zcr.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cgh.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://efj.guannengcc.top

TS:   d.toISOString()
来源：http://skx.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lqp.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://atn.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqb.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lhn.gotoacloud.top

[J03] 字符串解析为日期
来源：http://mgz.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ehy.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ylm.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://lrp.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://qkr.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cpc.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://acc.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://ptl.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zpe.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://nwl.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rgv.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pum.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wpa.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gvr.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yoi.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://teo.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mrf.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oeu.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://qnw.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://jno.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pss.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eka.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsq.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://veb.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lqr.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://nvb.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lii.bbcook.cn

[J06] 计算两时间之差
来源：http://xeh.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://ozp.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://qru.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mru.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://env.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wnp.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://itc.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://kbn.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://iih.shangyingyoupin.top

[J07] 比较两个日期
来源：http://tgv.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://ave.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yac.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rwa.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rkm.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jha.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iek.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://zsz.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://imk.pycfn.com

[J08] 提取年月日与星期
来源：http://jnn.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mul.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hcp.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lew.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uro.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://soz.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tzy.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://brc.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lic.yvedp.cn

[J09] 时区处理
来源：http://lzz.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hus.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eer.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fhm.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sgr.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mmg.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://luq.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://hrl.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tow.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://iot.cqqwz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iti.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ldp.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://khi.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ayr.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ocx.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oqf.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rgk.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://plq.0kj1m.cn

================================================================================
来源：http://miq.ydzc1.top

K. JSON 与序列化
来源：http://kov.cucudq.cn

================================================================================
来源：http://mal.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://nwf.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qjh.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pni.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://nlp.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://hwb.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vke.ydzc1.top

Go:   json.Marshal(obj)
来源：http://gyc.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://ntd.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nek.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://cwp.sjlbkw.cn

Py:   json.loads(s)
来源：http://tnq.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://erp.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://pcj.yj20258.top

TS:   JSON.parse(s)
来源：http://ekc.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wol.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://dur.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://gak.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zrk.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://ecb.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vxv.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ulk.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://cet.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gbn.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kxd.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://faz.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://koa.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pyv.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://ieq.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ruu.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rkt.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://klw.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vcf.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mvr.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hqb.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qvh.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kqs.chenzaomai.com

[K05] 深拷贝对象
来源：http://aru.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://cgb.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://vtm.guannengcc.top

JS:   structuredClone(obj)
来源：http://ebl.bjfxy.top

TS:   structuredClone(obj)
来源：http://trl.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://etj.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pjv.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tpv.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rhn.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://jwf.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bby.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ffc.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sew.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://roy.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gch.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://avv.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://elx.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fao.yanxiufei.cn

[K07] 进制转换
来源：http://kko.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jwx.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vyx.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gal.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vox.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://drv.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zcm.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hlo.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iud.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://jsy.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://chh.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://loh.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://whm.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://qcg.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ake.feifeiyinyue.top

Go:   encoding/gob
来源：http://ujv.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://bvg.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rmm.shanyushiyangtech.top

================================================================================
来源：http://qkr.shanyushiyangkeji.top

L. 网络请求
来源：http://kgr.cqqwz.cn

================================================================================
来源：http://wzu.ydzc1.top

[L01] 发送 GET 请求
来源：http://coe.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://chw.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qjh.yonumen.top

JS:   await fetch(url)
来源：http://wuc.cdnleiting.top

TS:   await fetch(url)
来源：http://vds.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ryh.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://pij.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vlj.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pbn.iojbl.cn

[L02] 发送 POST JSON
来源：http://hio.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://hog.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cbh.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dcz.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xxj.bjfxy.top


<!-- 参考信息 -->