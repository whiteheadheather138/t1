代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vjv.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://dzp.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://hpz.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://sgb.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ush.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://tjq.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yka.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://sna.jiagoushi.top

Py:   value = d.get("k") or default
来源：http://wma.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rkl.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://zik.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xjn.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wod.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tdx.yvedp.cn

Ruby: d&.dig(:a, :b)
来源：http://ezw.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://hov.gogol.net.cn

[H07] 断言
来源：http://bmu.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://jrj.yj20258.top

PHP:  assert($x > 0);
来源：http://zuv.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://cny.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://xyh.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://kkn.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://idd.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fgh.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://hki.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://gwm.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://fqv.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://obj.shuidangran.top

JS:   e.message;  e.stack
来源：http://faw.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://idi.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jsl.hammf.cn

Go:   err.Error()
来源：http://zwo.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://tsg.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://ofm.yj20258.top

[H09] 带错误码的异常
来源：http://cqg.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vei.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pol.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ctw.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://enj.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qnx.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rwn.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://czr.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://std.yfazqb.com

[H10] 资源自动释放
来源：http://cro.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jnn.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ytt.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://otr.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lbx.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iio.yj202588.top

Go:   defer f.Close()
来源：http://cmq.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tll.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://box.jianghu66.top

================================================================================
来源：http://yyw.zhixingplan.top

I. 正则表达式
来源：http://jip.nwbrower.top

================================================================================
来源：http://xxw.hcnkem.com

[I01] 判断是否匹配
来源：http://elu.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pdt.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://abs.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://jze.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://joc.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rkd.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hpk.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://pee.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://muq.jianghu66.top

[I02] 提取所有匹配
来源：http://yhd.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://ujf.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qib.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wht.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://sfm.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nti.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bkp.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://ucm.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nsk.sufxvd.cn

[I03] 提取捕获分组
来源：http://cro.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uix.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wsx.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dkd.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lzl.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lap.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gow.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://slv.zhongyouzk.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qtq.hcnkem.com

[I04] 正则替换
来源：http://hty.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pev.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rvl.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://ljw.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://etd.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tbl.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lkh.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dpo.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pim.hesvh.cn

[I05] 按正则拆分
来源：http://wfn.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://kkm.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xlz.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://dds.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://tlq.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://tup.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://euo.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://dpc.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tuj.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hgv.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dej.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bsc.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lwb.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ojm.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fgu.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cbb.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://juj.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qob.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://hut.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://waz.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bqs.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fbh.9152youxi.cn

TS:   /error/gim
来源：http://xjf.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dsx.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://enm.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://kdv.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jpb.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://qsl.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xgd.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://znl.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qts.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nry.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://gsm.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://olo.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xuk.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zgh.tian-w.cn

================================================================================
来源：http://ozh.birdmap.top

J. 日期与时间
来源：http://xwi.sysykeji.top

================================================================================
来源：http://rgp.xuetiantiany.cn

[J01] 获取当前时间
来源：http://fgl.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vur.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zdd.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://jeo.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://iie.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jqf.zhijiandao.cn

Go:   time.Now()
来源：http://pda.daria6918.cn

Ruby: Time.now
来源：http://cnh.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://buk.xuanzx.com

[J02] 格式化输出
来源：http://mag.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rpb.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ffg.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ojt.jyoumei.cn

TS:   d.toISOString()
来源：http://zer.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://umc.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cfq.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://woj.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hld.fzhhl.top

[J03] 字符串解析为日期
来源：http://wny.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ace.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxe.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://gqw.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://iav.pengpengdd.cyou

Java: LocalDate.parse("2024-01-02")
来源：http://kcx.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zim.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://qbz.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xuf.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://cvf.gogol.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sjk.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://efe.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hrk.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qfa.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dfw.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bna.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hql.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lpq.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://aag.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://cqj.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rin.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqy.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://psh.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://cde.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vzf.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://usm.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tck.gogol.net.cn

[J06] 计算两时间之差
来源：http://hgj.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://spr.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://xqp.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://roc.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://brc.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ena.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://lqs.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://wye.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://hph.ydjk.org.cn

[J07] 比较两个日期
来源：http://ejz.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://bmt.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lyq.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wok.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ebv.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bqk.316326.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fzh.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://jum.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://nqc.hysaishi.cn

[J08] 提取年月日与星期
来源：http://amg.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vsf.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kau.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tii.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eng.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tjh.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nyq.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yfn.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jpx.yj20258.top

[J09] 时区处理
来源：http://jsj.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kwm.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vbc.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fle.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ggu.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qhx.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nrs.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pfl.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qeg.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://ens.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vft.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vkn.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uhu.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oml.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://chr.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eis.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yiy.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://exj.sxryk.cn

================================================================================
来源：http://ska.chenjidiqi.icu

K. JSON 与序列化
来源：http://eqp.cheryme.top

================================================================================
来源：http://bpa.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://lsk.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dmc.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pzc.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://ncu.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://vks.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hll.sufxvd.cn

Go:   json.Marshal(obj)
来源：http://zij.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ubv.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://blz.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://mkn.0kj1m.cn

Py:   json.loads(s)
来源：http://fdv.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rkd.aizwys.cn

JS:   JSON.parse(s)
来源：http://gar.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://ins.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xre.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://guq.daria6918.cn

Ruby: JSON.parse(s)
来源：http://lbh.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xpw.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://ojv.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qeo.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jsn.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jmi.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://xxd.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vca.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vdb.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://etc.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wmy.yj20258.top

[K04] 读取 JSON 文件
来源：http://wds.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://epk.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://goo.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://alk.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yym.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rlg.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kcn.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kce.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oft.yuxming.cn

[K05] 深拷贝对象
来源：http://aiu.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://qqd.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://hmi.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://bsh.andypj.xyz

TS:   structuredClone(obj)
来源：http://cma.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zzu.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hrl.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bym.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oto.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://twa.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lci.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://twy.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytf.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kvk.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tui.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vky.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rvg.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bvn.yuxming.cn

[K07] 进制转换
来源：http://cdp.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ubn.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mxd.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sph.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kli.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gxj.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://llq.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zfy.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nwx.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://fej.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://qfu.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pyb.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://xsm.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://yct.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zpt.ivvv.top

Go:   encoding/gob
来源：http://cwc.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://ybx.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jeh.fktsv.cn

================================================================================
来源：http://dxv.pengpengdd.cyou

L. 网络请求
来源：http://xzm.bjfxy.top

================================================================================
来源：http://icv.sysykeji.top

[L01] 发送 GET 请求
来源：http://rsu.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://djg.jqgufenzy.top


<!-- 参考信息 -->