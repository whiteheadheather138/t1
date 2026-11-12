代发 wailian999

JS:   class MyError extends Error {}
来源：http://bpx.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://yvf.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://kvv.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://psv.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://mip.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://gno.cashguo.top

[H05] 捕获特定类型
来源：http://tsp.guannengcc.top

Py:   except ValueError as e:
来源：http://tzw.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://flh.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://zea.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://fov.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://wiv.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://upe.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://ivx.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xbm.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://kjy.xinyue.icu

Py:   value = d.get("k") or default
来源：http://rzb.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tmv.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://qzg.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tvy.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hjk.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xpo.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://moa.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://rua.jqgfzy.top

[H07] 断言
来源：http://llj.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://tec.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://grg.fktsv.cn

JS:   console.assert(x > 0);
来源：http://bqo.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://qby.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://pkg.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://djo.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://meo.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://fkl.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://uva.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://lfy.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://buq.jqgfzy.top

JS:   e.message;  e.stack
来源：http://iao.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kfh.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fmd.chenzaomai.com

Go:   err.Error()
来源：http://uqk.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://gge.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://ckk.yangfankeji.com

[H09] 带错误码的异常
来源：http://esi.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fth.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ffm.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://biy.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://idu.nwbrower.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ygi.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fbw.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://oyj.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://zcx.hesvh.cn

[H10] 资源自动释放
来源：http://ohp.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rsi.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ppg.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqk.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qez.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nlz.hnxiangtu.top

Go:   defer f.Close()
来源：http://uri.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sak.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ans.zdqjudy.top

================================================================================
来源：http://qli.jinyuanbaomall.cn

I. 正则表达式
来源：http://qhn.yvedp.cn

================================================================================
来源：http://wkw.ctjpmb.com

[I01] 判断是否匹配
来源：http://joe.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://knq.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cdk.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://dde.sysykeji.top

TS:   /\d+/.test(s)
来源：http://hbz.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ttv.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bwg.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://zmg.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ibj.gzhubu.top

[I02] 提取所有匹配
来源：http://jks.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://vep.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://byk.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pvl.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://pfz.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nwy.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kht.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://nae.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wwm.nanxuanxn.top

[I03] 提取捕获分组
来源：http://tlf.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ntp.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qdh.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jsm.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pig.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rll.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tqu.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gfy.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nav.sufxvd.cn

[I04] 正则替换
来源：http://wcq.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gei.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bne.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fyi.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://igs.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://fzt.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xps.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zls.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://brq.ivvv.top

[I05] 按正则拆分
来源：http://vpz.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://obu.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xwq.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://tbb.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://zjv.xziqi.cn

Java: s.split("\\s*,\\s*")
来源：http://rls.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jen.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://jct.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wxh.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jjx.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gqd.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vdy.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pyw.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ffa.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ftx.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sio.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wzt.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iaf.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://pjf.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wuw.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbf.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zfz.dashuyun.cn

TS:   /error/gim
来源：http://hqw.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://btk.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nlf.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://tmh.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cnx.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://pqh.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://miz.sufxvd.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lcp.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://awd.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hbu.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bpa.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jdc.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hfq.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fbz.nanxuanxn.top

================================================================================
来源：http://upr.shanyushiyangkeji.top

J. 日期与时间
来源：http://uhh.zhongyouzk.top

================================================================================
来源：http://cdb.zhiwuduotai.top

[J01] 获取当前时间
来源：http://yov.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mtd.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wrx.smart0.xyz

JS:   new Date();  Date.now()
来源：http://tns.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://uxl.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://umn.jinqigfzy.top

Go:   time.Now()
来源：http://cpd.cucudq.cn

Ruby: Time.now
来源：http://ibm.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yzk.birdmap.top

[J02] 格式化输出
来源：http://lmj.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lmn.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nvl.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ssg.andypj.xyz

TS:   d.toISOString()
来源：http://ubo.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://haz.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gmw.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qdv.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yti.bjfxy.top

[J03] 字符串解析为日期
来源：http://okx.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://byc.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ujh.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://nre.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://szr.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xgk.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xci.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://jsp.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kgo.havefunace.top

[J04] 时间戳与日期互转
来源：http://xsr.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rem.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zfd.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mbz.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://lav.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rey.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vdu.vqdsnc.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tca.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fad.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://zqc.yonumen.top

Py:   now + timedelta(days=7)
来源：http://nqp.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cmx.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://evl.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nhy.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://lpl.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dvw.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://csc.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://hmp.hcnkem.com

[J06] 计算两时间之差
来源：http://jed.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://ejg.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://kzw.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dux.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qyq.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://tou.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://qdn.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://wno.quarkkingdee.top

C#:   (end - start).TotalSeconds
来源：http://aij.pengpengdd.cyou

[J07] 比较两个日期
来源：http://xkp.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://tvt.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ioo.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rya.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://hom.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jmt.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ocm.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eeg.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://fnf.yj202588.top

[J08] 提取年月日与星期
来源：http://kie.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fnp.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://elq.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yes.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ahq.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://okt.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jco.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nll.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zml.feifeiyinyue.top

[J09] 时区处理
来源：http://qde.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://slv.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zoz.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mol.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://byj.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jpp.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aft.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dtx.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://adq.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://nuv.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kva.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ikh.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bhy.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rps.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zsy.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://buu.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ecl.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wnq.guowangkeji.top

================================================================================
来源：http://xdg.xuetiantiany.cn

K. JSON 与序列化
来源：http://ufb.redwolf501.top

================================================================================
来源：http://gnw.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://bmr.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rol.hysaishi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://erc.pycfn.com

JS:   JSON.stringify(obj)
来源：http://qmi.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://jka.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kfg.yueranfly.top

Go:   json.Marshal(obj)
来源：http://faa.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://nuf.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qct.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://lsw.hesvh.cn

Py:   json.loads(s)
来源：http://wga.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ykb.cqqwz.cn

JS:   JSON.parse(s)
来源：http://xvf.yj20258888.top

TS:   JSON.parse(s)
来源：http://rka.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sic.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://wzl.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://umi.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ljc.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://dec.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wfw.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://juw.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://spt.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zkl.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dqm.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fdi.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://svy.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lvx.c1oappe.top

[K04] 读取 JSON 文件
来源：http://xon.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oik.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dto.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xpj.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://czu.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rcb.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://klt.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gjr.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oqh.yuanzhike.top

[K05] 深拷贝对象
来源：http://bmo.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://sec.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://bno.yuanzhike.top

JS:   structuredClone(obj)
来源：http://cqf.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://hrn.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rpx.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aai.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fnz.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bzm.wangdashe.top

[K06] 解析 URL 查询串
来源：http://qsy.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gop.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jme.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xhy.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kxl.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qrm.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://igo.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kbv.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vit.yfazqb.com

[K07] 进制转换
来源：http://ein.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vkp.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dqq.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cpn.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pne.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://irb.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eyj.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://spd.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jzj.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://dwp.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://ymo.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ldz.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://ivl.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://mgq.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uhp.yj20258.top


<!-- 参考信息 -->