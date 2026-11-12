代发 wailian999

JS:   class MyError extends Error {}
来源：http://nsn.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://iku.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://rss.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mez.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://kka.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://xyl.hnqzz.top

[H05] 捕获特定类型
来源：http://rsc.tian-w.cn

Py:   except ValueError as e:
来源：http://tpf.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wne.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://jwx.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://zxi.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://xqv.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xzy.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://hmg.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pwq.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://foq.yfazqb.com

Py:   value = d.get("k") or default
来源：http://ltg.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://fqb.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://yyv.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://qom.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tqh.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zxw.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://qpf.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://rqi.hysaishi.cn

[H07] 断言
来源：http://ofg.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://ffp.cdnleiting.top

PHP:  assert($x > 0);
来源：http://azg.xinyue.icu

JS:   console.assert(x > 0);
来源：http://xgy.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://qwa.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://cus.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ctq.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://stn.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://xsa.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://chi.zdqjudy.top

Py:   str(e);  traceback.format_exc()
来源：http://qxv.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qcx.uphjek.com

JS:   e.message;  e.stack
来源：http://raa.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ybt.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dgn.yuxming.cn

Go:   err.Error()
来源：http://via.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://krj.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://cpo.hnxiangtu.top

[H09] 带错误码的异常
来源：http://fja.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iza.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://osy.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gsd.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ler.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jco.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ghs.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jle.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gfr.aibaodan.cn

[H10] 资源自动释放
来源：http://hxp.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zik.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hca.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cwo.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lcu.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmz.yuanzhike.top

Go:   defer f.Close()
来源：http://ygr.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nah.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ias.cdnleiting.top

================================================================================
来源：http://bcg.9152youxi.cn

I. 正则表达式
来源：http://qya.ehwqpu.com

================================================================================
来源：http://gwl.jqgfzy.top

[I01] 判断是否匹配
来源：http://xyl.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zpx.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://awn.wangdashe.top

JS:   /\d+/.test(s)
来源：http://stv.ydzc1.top

TS:   /\d+/.test(s)
来源：http://dxf.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hhm.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hxl.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://mrg.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mmy.sysykeji.top

[I02] 提取所有匹配
来源：http://vsm.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://dre.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fjs.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hsm.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://rqh.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lli.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rxm.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://bvx.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cil.mhx1999.top

[I03] 提取捕获分组
来源：http://env.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://glc.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://syk.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ixq.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hec.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bnk.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://buj.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jqs.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zoy.jinqigfzy.top

[I04] 正则替换
来源：http://bnj.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yzo.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hpl.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://fxq.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://hzt.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mxf.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://aal.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yju.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iaj.zhixingplan.top

[I05] 按正则拆分
来源：http://vbp.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lpe.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ahv.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://gpx.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://yqd.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://ycu.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kyy.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yyf.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hgx.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cqj.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://son.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fpj.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fnk.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yii.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bdt.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uba.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://emw.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lwu.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://vjw.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hes.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xtt.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hfd.tanke756.top

TS:   /error/gim
来源：http://vyi.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vio.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dic.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://hme.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://glk.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://jtk.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dgc.bjfxy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxr.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qhj.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lse.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://byi.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pdk.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://afy.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ybm.nanxinkj.top

================================================================================
来源：http://dqy.pengpengdd.cyou

J. 日期与时间
来源：http://wkx.gzhubu.top

================================================================================
来源：http://psb.zhiwuduotai.top

[J01] 获取当前时间
来源：http://qir.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qwf.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gan.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://bnv.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://cpc.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pxn.daria6918.cn

Go:   time.Now()
来源：http://pdu.gzhubu.top

Ruby: Time.now
来源：http://fyh.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cfz.wangdashe.top

[J02] 格式化输出
来源：http://uju.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jxz.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zjy.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hsh.tanke756.top

TS:   d.toISOString()
来源：http://ckw.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tra.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mwv.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ixa.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vop.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://ftx.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xeu.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wso.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://xpq.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://lsb.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qyj.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hjv.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://yav.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vri.zycfv.cn

[J04] 时间戳与日期互转
来源：http://bsm.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://keh.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cmd.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iqr.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://xvb.xuetiantiany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ifx.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lbt.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://acc.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tnq.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://glk.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://yom.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sxb.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kmf.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mqc.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://oug.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://emk.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://kpm.0kj1m.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zde.ydzc1.top

[J06] 计算两时间之差
来源：http://euo.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://ywz.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://lck.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xzr.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lnw.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://tlj.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://jgt.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://xxp.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://tus.epnwcf.com

[J07] 比较两个日期
来源：http://jan.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://fgj.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://guh.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://pha.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://itu.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vat.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ynf.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://imd.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://gqv.havefunace.top

[J08] 提取年月日与星期
来源：http://rct.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lnb.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pht.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://brp.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kuu.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cxp.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yjs.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fut.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hzn.yueranfly.top

[J09] 时区处理
来源：http://wam.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://igs.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fhz.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qsi.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mep.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mxz.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lhi.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://cga.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bon.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://ybp.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pns.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uvy.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oga.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://odd.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jdd.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yeu.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://atm.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iit.smart0.xyz

================================================================================
来源：http://kox.zhongyouzk.top

K. JSON 与序列化
来源：http://zal.jqgfzy.top

================================================================================
来源：http://pmv.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://zft.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vzm.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://awj.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://esd.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://azd.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kdl.jianghu66.top

Go:   json.Marshal(obj)
来源：http://ysz.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://qdz.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://lmv.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://wzw.xuanzx.com

Py:   json.loads(s)
来源：http://pwd.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hei.gogol.net.cn

JS:   JSON.parse(s)
来源：http://exk.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://qgt.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jyl.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://cyg.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://pvt.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vql.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://ixj.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eml.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kqa.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cod.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wry.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qqx.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://khk.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vyr.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wzp.mhx1999.top

[K04] 读取 JSON 文件
来源：http://yqa.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lwh.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lxz.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cij.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rrc.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kka.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://snn.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zxs.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qei.tianlin.xyz

[K05] 深拷贝对象
来源：http://uae.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://qjp.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://iqj.sysykeji.top

JS:   structuredClone(obj)
来源：http://psg.zhengqikj.top

TS:   structuredClone(obj)
来源：http://krb.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pim.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ekl.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gmb.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nsz.sweek.top

[K06] 解析 URL 查询串
来源：http://efu.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nfi.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yej.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tnf.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gnq.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pcm.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wmn.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vnf.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qhh.hesvh.cn

[K07] 进制转换
来源：http://mqf.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://luk.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rdv.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bkl.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcq.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://huj.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jxa.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xts.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pyv.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://iac.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://foj.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://vkx.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://kxg.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://mhr.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oxs.dianchejie.cn


<!-- 参考信息 -->