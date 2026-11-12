代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tfd.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://bzv.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://kit.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://lvw.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ytd.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://clm.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dtl.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://oxd.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://qzd.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://pvq.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gsm.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://xzb.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gbk.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eph.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://vac.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://zru.jianghu66.top

[H07] 断言
来源：http://zlx.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://bxc.zdbjq.cn

PHP:  assert($x > 0);
来源：http://evu.tarul.cn

JS:   console.assert(x > 0);
来源：http://fgq.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://spe.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://zag.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nyu.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tjq.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://nup.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://hhz.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://aak.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ooc.haohaochexian.top

JS:   e.message;  e.stack
来源：http://qcc.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uck.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wok.feifeiyinyue.top

Go:   err.Error()
来源：http://pfm.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://ifx.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://dff.gotoacloud.top

[H09] 带错误码的异常
来源：http://opj.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qzp.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://oce.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kuj.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qoq.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eao.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ozl.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://nhf.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cmu.gaohongyu789.top

[H10] 资源自动释放
来源：http://vcg.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://juv.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ivd.yangfankeji.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yks.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ikr.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tqn.c1oappe.top

Go:   defer f.Close()
来源：http://oxz.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kca.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vzz.dashuyun.cn

================================================================================
来源：http://vmm.shzxlz.cn

I. 正则表达式
来源：http://jby.chenlongwang.top

================================================================================
来源：http://qhj.9152youxi.cn

[I01] 判断是否匹配
来源：http://gfo.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bte.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://nri.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://cfx.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://nmb.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://czq.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dva.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://hxa.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wwk.hywenlv.cn

[I02] 提取所有匹配
来源：http://vnz.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://mpa.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rqd.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://igq.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://kpd.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://epl.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vbb.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://icv.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cye.zhengqikj.top

[I03] 提取捕获分组
来源：http://jim.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cje.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fkj.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nco.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hum.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fuf.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fjd.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qcz.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fbr.chenlongwang.top

[I04] 正则替换
来源：http://yet.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aam.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://swq.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://zkz.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xhw.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://owe.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bix.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ueg.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yxs.aibaodan.cn

[I05] 按正则拆分
来源：http://ake.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://trq.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xcu.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://liw.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://lwo.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://vyb.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xuh.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ncv.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xva.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ziy.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uai.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ztp.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://huw.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://usc.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dqd.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cue.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xga.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cth.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://bkh.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pnn.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kea.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xlj.wangdashe.top

TS:   /error/gim
来源：http://edm.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://msq.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jwl.pycfn.com

Ruby: s.scan(/error/i)
来源：http://zdu.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zll.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://jfq.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cpm.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mtd.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oyu.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wtf.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mjv.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kpm.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pzn.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jep.smart0.xyz

================================================================================
来源：http://bda.yj202588.top

J. 日期与时间
来源：http://wok.haohaochexian.top

================================================================================
来源：http://xbc.bbcook.cn

[J01] 获取当前时间
来源：http://pqq.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oks.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fml.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://oxb.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://hdj.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hpa.zhongyouzk.top

Go:   time.Now()
来源：http://nqg.birdmap.top

Ruby: Time.now
来源：http://dsw.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://koo.yj20258.top

[J02] 格式化输出
来源：http://lvt.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kia.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bru.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tgr.birdmap.top

TS:   d.toISOString()
来源：http://bov.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fpa.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jhl.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gfs.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cfq.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://wyk.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nrx.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gvx.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://ulg.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://nuj.bjfxy.top

Java: LocalDate.parse("2024-01-02")
来源：http://uol.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dwo.jinyuanbaomall.cn

Ruby: Date.parse("2024-01-02")
来源：http://wjw.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mkb.nwbrower.top

[J04] 时间戳与日期互转
来源：http://khu.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://unk.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bbe.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zyk.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sih.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hvg.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zeg.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sip.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fse.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://ief.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://gmo.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://amy.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxp.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://djh.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://klu.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nzk.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://nxg.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://ind.tanke756.top

[J06] 计算两时间之差
来源：http://bmt.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://fjz.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://gkx.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jcc.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iah.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://spv.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://tma.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://mwy.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://ydu.jqgufenzy.top

[J07] 比较两个日期
来源：http://ndg.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://aje.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kbf.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://eui.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://ggd.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xmc.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xxr.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xpx.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://ihc.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://oki.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dkp.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vpt.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://adm.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ycb.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mse.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zol.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sbh.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fyb.zdqjudy.top

[J09] 时区处理
来源：http://ahx.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vno.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hez.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xpi.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wvb.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://plx.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lhi.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tdg.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cqf.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://prd.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://ddb.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zoa.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kss.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pms.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eqa.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mhc.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rje.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kds.ydjk.org.cn

================================================================================
来源：http://fcs.gotoacloud.top

K. JSON 与序列化
来源：http://tyn.sjlbkw.cn

================================================================================
来源：http://fyq.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://yri.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ity.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rfb.meibo888.top

JS:   JSON.stringify(obj)
来源：http://uha.meibo888.top

TS:   JSON.stringify(obj)
来源：http://obm.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dnn.52xcode.cn

Go:   json.Marshal(obj)
来源：http://lvy.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://urb.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://njl.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://zcl.nwbrower.top

Py:   json.loads(s)
来源：http://ajo.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kmu.zdqjudy.top

JS:   JSON.parse(s)
来源：http://zxb.yj20258.top

TS:   JSON.parse(s)
来源：http://rnb.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rvb.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://jxt.yvedp.cn

Ruby: JSON.parse(s)
来源：http://mve.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zmt.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://zlz.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bmc.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://omp.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://enp.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://knv.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://apv.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eiy.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://gqq.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bdj.cashguo.top

[K04] 读取 JSON 文件
来源：http://bpc.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nqu.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ozx.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rrz.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ukf.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bvz.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rgz.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qif.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jvo.kuanghao11.cn

[K05] 深拷贝对象
来源：http://gny.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://xnx.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://ihi.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://ika.daxiang520.top

TS:   structuredClone(obj)
来源：http://ayp.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://xeq.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pvv.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tkk.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vpr.yj20258888.top

[K06] 解析 URL 查询串
来源：http://ifh.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hmp.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://njd.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mdo.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ywx.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://etn.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://txh.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://upu.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kce.zhijiandao.cn

[K07] 进制转换
来源：http://oct.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hpp.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bmo.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oox.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hup.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vfy.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zrj.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jlt.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cxr.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://roq.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://cgt.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://phv.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://dim.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ghy.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nxu.epnwcf.com

Go:   encoding/gob
来源：http://kmn.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://jkp.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bzr.hywenlv.cn

================================================================================
来源：http://bjy.316326.xyz

L. 网络请求
来源：http://sec.uphjek.com

================================================================================
来源：http://inr.yueranfly.top

[L01] 发送 GET 请求
来源：http://brm.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xty.pengpengdd.cyou


<!-- 参考信息 -->