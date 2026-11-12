代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://ixz.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://jol.cucudq.cn

[H05] 捕获特定类型
来源：http://qbj.havefunace.top

Py:   except ValueError as e:
来源：http://euy.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dmy.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://srv.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://lrm.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://nzg.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cyg.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://iyh.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ruj.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://qjl.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://zhe.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://yxm.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://sma.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dro.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fis.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wlr.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://lxs.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://dbi.dianchejie.cn

[H07] 断言
来源：http://eqc.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://gzr.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://uau.bjfxy.top

JS:   console.assert(x > 0);
来源：http://wqa.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://bke.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://edz.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hbg.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://diy.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://frv.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://bnb.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ynn.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ksd.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://lso.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bsz.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xcj.sweek.top

Go:   err.Error()
来源：http://duj.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://plb.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://uux.zhijiandao.cn

[H09] 带错误码的异常
来源：http://fet.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uzf.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nuj.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szu.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qqv.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yhl.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://flk.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hiv.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://vyt.xuanzx.com

[H10] 资源自动释放
来源：http://ipr.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lsm.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ecl.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://peo.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gzx.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://car.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://rel.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tbj.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wdq.ivvv.top

================================================================================
来源：http://kuv.jyoumei.cn

I. 正则表达式
来源：http://vjj.zhengqikj.top

================================================================================
来源：http://jmf.andypj.xyz

[I01] 判断是否匹配
来源：http://lqf.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ckm.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pwb.hcnkem.com

JS:   /\d+/.test(s)
来源：http://ucf.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://emx.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oqm.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hrp.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://wst.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rmv.smart0.xyz

[I02] 提取所有匹配
来源：http://rvz.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://rge.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kpd.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zkm.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://jix.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vdi.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ghk.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://qba.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://png.316326.xyz

[I03] 提取捕获分组
来源：http://tfc.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vjv.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ulf.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://res.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pmo.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jxc.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://brj.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ghw.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mha.ydzc1.top

[I04] 正则替换
来源：http://laz.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zbe.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lxq.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://roc.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://gnj.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://vlc.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pke.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fhf.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fmw.yanxiufei.cn

[I05] 按正则拆分
来源：http://hox.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pni.xziqi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ciu.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://nmt.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://udg.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://muq.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qdv.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://ead.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ljb.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://msl.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kvp.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://glj.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fhy.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vjh.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dpw.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://coi.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ywb.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ait.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://pyu.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zrs.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vwr.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gwt.xuanzx.com

TS:   /error/gim
来源：http://rrq.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://unv.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zdf.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://fnq.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cdd.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://rsv.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ffg.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vej.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ypu.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zci.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nea.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ymw.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sdu.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jfl.xinyue.icu

================================================================================
来源：http://saa.ivvv.top

J. 日期与时间
来源：http://ipj.xuetiantiany.cn

================================================================================
来源：http://wrf.ydjk.org.cn

[J01] 获取当前时间
来源：http://qfq.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://twl.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://neb.vehdjk.com

JS:   new Date();  Date.now()
来源：http://adl.fehbvm.com

TS:   new Date();  Date.now()
来源：http://hzs.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://rpj.zhengqikj.top

Go:   time.Now()
来源：http://teg.cdnleiting.top

Ruby: Time.now
来源：http://dhp.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rfe.guannengcc.top

[J02] 格式化输出
来源：http://nhr.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nta.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cct.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://spj.zhongyouzk.top

TS:   d.toISOString()
来源：http://qlf.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ogd.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dgl.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dhj.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tfs.andypj.xyz

[J03] 字符串解析为日期
来源：http://owd.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ymy.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cro.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://owe.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://laq.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://odq.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://omv.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://ofk.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cdx.tarul.cn

[J04] 时间戳与日期互转
来源：http://xjh.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rqu.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://phc.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://orc.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://icg.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fnz.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pdy.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://epz.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vxq.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://zlv.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://qfz.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://vik.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gke.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://twz.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://yyc.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://chb.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://rbf.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://lea.zycfv.cn

[J06] 计算两时间之差
来源：http://sbj.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://xxo.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://lnh.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dmx.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bhk.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://bcp.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://hej.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://dhu.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://nsy.yonumen.top

[J07] 比较两个日期
来源：http://ovg.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://xxi.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://smz.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://agk.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://zxb.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zff.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ngd.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kcp.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://dzb.uphjek.com

[J08] 提取年月日与星期
来源：http://iot.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jwx.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bqk.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fpf.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gyl.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mzb.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cbh.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pel.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jad.aizwys.cn

[J09] 时区处理
来源：http://mkn.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tzj.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iof.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sjz.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://faf.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gym.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nkz.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eid.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://byn.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://kqy.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vtf.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pzk.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ydp.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ckl.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jzw.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ddb.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kbz.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tcp.jinyuanbaomall.cn

================================================================================
来源：http://bbg.zhongyouzk.top

K. JSON 与序列化
来源：http://ixu.haohaochexian.top

================================================================================
来源：http://rmq.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://buw.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zmo.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tct.uphjek.com

JS:   JSON.stringify(obj)
来源：http://gmu.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://bsh.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://miz.smart0.xyz

Go:   json.Marshal(obj)
来源：http://bbs.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://frm.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://buz.sweek.top

[K02] JSON 字符串转对象
来源：http://egx.meibo888.top

Py:   json.loads(s)
来源：http://urv.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://shy.dianchejie.cn

JS:   JSON.parse(s)
来源：http://wle.yuxming.cn

TS:   JSON.parse(s)
来源：http://meo.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dzo.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://grr.jianghu66.top

Ruby: JSON.parse(s)
来源：http://rzy.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rpn.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://nzi.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xbd.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sec.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vdc.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zpw.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://azk.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vwl.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://bdt.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yjg.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://lzq.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nhx.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vog.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yuu.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wwk.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xoc.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mkh.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://kij.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ady.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://pno.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://ekc.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://dhc.gotoacloud.top

JS:   structuredClone(obj)
来源：http://hrf.cucudq.cn

TS:   structuredClone(obj)
来源：http://ita.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xye.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://psh.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ybu.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://bex.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://rbd.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xpr.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vyt.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://env.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpx.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cdp.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dod.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wfw.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ymq.sjlbkw.cn

[K07] 进制转换
来源：http://xeh.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rng.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://scm.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ejj.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qhf.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uom.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kgz.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nwa.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vbi.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://bbw.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://mns.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://obb.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://xvb.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://xnt.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xud.chenzaomai.com

Go:   encoding/gob
来源：http://krn.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://gpm.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hku.xziqi.cn

================================================================================
来源：http://kmc.aibaodan.cn


<!-- 参考信息 -->