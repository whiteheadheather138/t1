代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://icb.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://jxv.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://foo.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://cof.xuanzx.com

Py:   value = d.get("k") or default
来源：http://ijc.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://ser.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hvb.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://cbz.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vjz.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xnt.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://oeh.xuetiantiany.cn

C#:   obj?.A?.B ?? default
来源：http://wxl.zycfv.cn

[H07] 断言
来源：http://zjk.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://rlj.yj20258888.top

PHP:  assert($x > 0);
来源：http://hhh.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://ggh.epnwcf.com

TS:   console.assert(x > 0);
来源：http://hfr.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://bfh.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wfd.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://ddu.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://gbg.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://qxm.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://fyv.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xld.9152youxi.cn

JS:   e.message;  e.stack
来源：http://bnh.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yjp.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fnp.zhongyouzk.top

Go:   err.Error()
来源：http://jqt.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://exf.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://nwz.52xcode.cn

[H09] 带错误码的异常
来源：http://gxo.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mhx.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rvr.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ipp.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gun.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lma.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://not.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://elr.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zct.kuanghao11.cn

[H10] 资源自动释放
来源：http://qhn.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://msj.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://skh.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zrn.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dgg.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://heu.uphjek.com

Go:   defer f.Close()
来源：http://vdh.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uck.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qbb.shanyushiyangtech.top

================================================================================
来源：http://lli.zdqjudy.top

I. 正则表达式
来源：http://tsx.shanyushiyangkeji.top

================================================================================
来源：http://woi.andypj.xyz

[I01] 判断是否匹配
来源：http://kwh.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dah.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://whd.vehdjk.com

JS:   /\d+/.test(s)
来源：http://hgp.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://ryg.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://atx.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uuz.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://crb.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xyn.aizwys.cn

[I02] 提取所有匹配
来源：http://fxo.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://uri.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ice.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hsi.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://sib.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://afs.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rse.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://hhj.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uog.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://pxw.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xxg.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jpm.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pex.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gvy.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://slo.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dfw.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hwr.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ffj.zhoulong.xyz

[I04] 正则替换
来源：http://nle.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uxx.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iva.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://mzw.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hkw.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fmr.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bxx.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wed.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nbj.yueranfly.top

[I05] 按正则拆分
来源：http://loz.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xrv.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://frl.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://vmj.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://rso.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://pfx.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gws.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rjp.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xlv.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ipx.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fhh.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://irx.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oef.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nme.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jrb.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qwz.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uao.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cyy.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://gui.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://etk.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vtt.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://spr.guannengcc.top

TS:   /error/gim
来源：http://bst.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zes.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rff.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://khc.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yjt.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://vzt.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://smi.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fou.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pkt.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gxw.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nhc.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fwt.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://juf.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kod.jinqigfzy.top

================================================================================
来源：http://soe.zhaomingkeji.xyz

J. 日期与时间
来源：http://rdg.0kj1m.cn

================================================================================
来源：http://znx.wangshuangyany.cn

[J01] 获取当前时间
来源：http://tpd.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nmz.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bao.cucudq.cn

JS:   new Date();  Date.now()
来源：http://nur.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://jkj.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://syl.tian-w.cn

Go:   time.Now()
来源：http://tsv.yuxming.cn

Ruby: Time.now
来源：http://hmk.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fpc.tanke756.top

[J02] 格式化输出
来源：http://xfe.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://glu.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wch.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aiw.shangyingyoupin.top

TS:   d.toISOString()
来源：http://xcm.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ywq.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qmq.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwa.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jnj.aizwys.cn

[J03] 字符串解析为日期
来源：http://cui.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://now.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vyl.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://yvo.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://hsa.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://lxp.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yly.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://rds.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jgl.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://cre.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qee.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ner.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lln.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://mhm.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kzy.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vnm.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hen.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lww.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://nan.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://ped.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jfv.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ner.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zrv.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://rsl.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://scv.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://koz.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zlf.yanxiufei.cn

[J06] 计算两时间之差
来源：http://msw.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://nbk.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://xtc.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kic.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ebl.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xur.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://wrz.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://plq.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://aor.birdmap.top

[J07] 比较两个日期
来源：http://eck.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://nko.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dhg.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jvi.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://xrm.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eid.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pik.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ghm.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://ktl.c1oappe.top

[J08] 提取年月日与星期
来源：http://fbp.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bwu.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wis.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iil.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hjb.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rgq.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hhz.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yvz.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://woc.jyoumei.cn

[J09] 时区处理
来源：http://oyc.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iqy.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yuu.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asw.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://piw.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ama.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mjh.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lmc.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://urb.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://rye.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vlu.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pvl.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mig.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zji.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eds.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cgk.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mzi.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pwm.dianchejie.cn

================================================================================
来源：http://cnr.gaohongyu789.top

K. JSON 与序列化
来源：http://xgv.zhaomingkeji.xyz

================================================================================
来源：http://ujg.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://ako.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fsx.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tpm.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://fng.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://cqs.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bkr.yfazqb.com

Go:   json.Marshal(obj)
来源：http://bwa.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://xdv.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zke.yuxming.cn

[K02] JSON 字符串转对象
来源：http://any.shuidangran.top

Py:   json.loads(s)
来源：http://ybg.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qey.hnqzz.top

JS:   JSON.parse(s)
来源：http://snq.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://jkw.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uzr.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://hrl.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://grv.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://faq.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://jgg.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://myl.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://arw.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xrv.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://drq.tian-w.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gaf.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eyi.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://rro.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ycb.andypj.xyz

[K04] 读取 JSON 文件
来源：http://jyn.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://beq.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eio.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jpc.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bux.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zgk.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vzj.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kdu.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wqy.hesvh.cn

[K05] 深拷贝对象
来源：http://xyh.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://dnf.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://rzq.bbcook.cn

JS:   structuredClone(obj)
来源：http://orx.epnwcf.com

TS:   structuredClone(obj)
来源：http://qxt.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bwh.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nar.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pch.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://nkq.iojbl.cn

[K06] 解析 URL 查询串
来源：http://vws.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rlz.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pyx.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rzl.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wpw.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ljr.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tbw.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fcn.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://txt.yanxiufei.cn

[K07] 进制转换
来源：http://kbn.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cuv.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://efe.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zre.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbz.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cag.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://epg.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wts.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tfy.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://ead.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://tgf.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://tti.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://ssu.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://byw.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://glj.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://hcf.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://dpk.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcr.fzhhl.top

================================================================================
来源：http://oli.chenzaomai.com

L. 网络请求
来源：http://nvk.yj20258.top

================================================================================
来源：http://dph.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://kre.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nqr.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nxx.gotoacloud.top

JS:   await fetch(url)
来源：http://hgf.kuanghao11.cn

TS:   await fetch(url)
来源：http://odk.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fyn.yonumen.top


<!-- 参考信息 -->