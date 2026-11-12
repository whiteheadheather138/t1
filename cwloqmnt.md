代发 wailian999

Py:   value = d.get("k") or default
来源：http://lak.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bqk.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bmv.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://jta.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://owg.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://mff.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://usi.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://uws.redwolf501.top

[H07] 断言
来源：http://ksp.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://thx.cucudq.cn

PHP:  assert($x > 0);
来源：http://ceq.havefunace.top

JS:   console.assert(x > 0);
来源：http://vec.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://wtm.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://usz.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fwq.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://loo.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://oze.sweek.top

[H08] 获取错误信息与堆栈
来源：http://yih.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://nee.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ako.fehbvm.com

JS:   e.message;  e.stack
来源：http://obt.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sci.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oih.yanxiufei.cn

Go:   err.Error()
来源：http://khj.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://vgy.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://ebe.havefunace.top

[H09] 带错误码的异常
来源：http://lwg.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ksy.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://fqf.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://icx.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gax.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xox.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qtz.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://skc.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yan.wangshuangyany.cn

[H10] 资源自动释放
来源：http://hyv.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pld.yueranfly.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kjj.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dyf.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://way.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fpz.guannengcc.top

Go:   defer f.Close()
来源：http://gxg.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wdy.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qsz.jinghuilouyu.cn

================================================================================
来源：http://ayi.0kj1m.cn

I. 正则表达式
来源：http://nno.snrcjt.cn

================================================================================
来源：http://jpo.fengsongda.top

[I01] 判断是否匹配
来源：http://fww.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kwy.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ovh.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://tgr.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://ksf.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wjc.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oaf.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://sjy.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://smh.chenlongwang.top

[I02] 提取所有匹配
来源：http://ufo.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://xzm.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vzk.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nkx.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://trt.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qky.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ggx.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://lor.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tqp.cashguo.top

[I03] 提取捕获分组
来源：http://ysp.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ynr.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hee.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dxo.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ufs.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nmd.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gfs.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pqn.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zga.hnqzz.top

[I04] 正则替换
来源：http://fel.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hhl.yanxiufei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ckd.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://wde.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://xzi.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://gmr.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uuk.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rws.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gks.bbcook.cn

[I05] 按正则拆分
来源：http://heb.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tkx.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://exx.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://jub.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://ltv.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://cfk.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bgq.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wud.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://woq.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oqz.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oec.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uxp.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tyb.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xkj.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dst.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lqk.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vct.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ysx.aizwys.cn

[I07] 忽略大小写与多行模式
来源：http://cma.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jee.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cqr.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ytl.kuanghao11.cn

TS:   /error/gim
来源：http://bbs.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aun.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lbx.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://xzm.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vip.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://tfn.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ael.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aox.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vfi.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nou.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zyv.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fzl.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dzi.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kyh.birdmap.top

================================================================================
来源：http://oye.yvedp.cn

J. 日期与时间
来源：http://chb.fehbvm.com

================================================================================
来源：http://ata.zycfv.cn

[J01] 获取当前时间
来源：http://hjt.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fbc.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tnf.cucudq.cn

JS:   new Date();  Date.now()
来源：http://vzn.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://icz.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rjf.yj20258888.top

Go:   time.Now()
来源：http://zzl.mhx1999.top

Ruby: Time.now
来源：http://pwo.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nvy.tian-w.cn

[J02] 格式化输出
来源：http://agq.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fiq.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yyd.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xip.sufxvd.cn

TS:   d.toISOString()
来源：http://eqe.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://seq.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://osy.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kur.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kfd.9152youxi.cn

[J03] 字符串解析为日期
来源：http://aqg.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uir.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mtb.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://ftn.birdmap.top

TS:   new Date("2024-01-02")
来源：http://wpu.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://lna.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bqm.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://vzf.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fxa.xziqi.cn

[J04] 时间戳与日期互转
来源：http://tun.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rof.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://erd.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tyi.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ywb.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://grx.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xth.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zxk.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qtj.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://pxw.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://vdw.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bor.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ozo.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpm.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://rzx.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://czk.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://lze.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://cbx.fengsongda.top

[J06] 计算两时间之差
来源：http://xxc.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://kwn.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://txw.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vhp.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xqr.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iyu.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://iaq.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://pml.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://qmz.cashguo.top

[J07] 比较两个日期
来源：http://ubd.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://nmn.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vdo.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ehi.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lte.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cbs.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fpc.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ekt.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://zrd.jianghu66.top

[J08] 提取年月日与星期
来源：http://skn.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dsj.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kwo.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jwl.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kef.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://llf.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qav.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://isy.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ftc.hysaishi.cn

[J09] 时区处理
来源：http://xcu.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gxa.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jwq.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fuc.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fvv.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lfs.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rbs.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xof.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sxv.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://lvt.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lzt.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://odw.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zpy.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://shc.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ayp.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tzw.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wvv.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wcv.aizwys.cn

================================================================================
来源：http://mcg.wangdashe.top

K. JSON 与序列化
来源：http://gwp.zhijiandao.cn

================================================================================
来源：http://dxs.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://wct.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vco.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ejp.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://lyj.cheryme.top

TS:   JSON.stringify(obj)
来源：http://zxa.yanxiufei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xmy.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://kol.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tcw.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bqr.xylfe.cn

[K02] JSON 字符串转对象
来源：http://iab.havefunace.top

Py:   json.loads(s)
来源：http://qms.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aev.hcnkem.com

JS:   JSON.parse(s)
来源：http://bio.daxiang520.top

TS:   JSON.parse(s)
来源：http://yuc.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wpz.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://ztr.ivvv.top

Ruby: JSON.parse(s)
来源：http://bqn.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://exw.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://xvp.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oyk.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lzt.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ogo.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mgs.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uqh.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wxg.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://qou.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dra.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://trb.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xtp.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jfq.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vde.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wdw.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qmp.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xec.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cfa.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zgy.haohaochexian.top

[K05] 深拷贝对象
来源：http://udj.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://ycy.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://hnn.hfpthk.cn

JS:   structuredClone(obj)
来源：http://tej.bbcook.cn

TS:   structuredClone(obj)
来源：http://vbe.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ozg.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rqt.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://plt.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kws.hcnkem.com

[K06] 解析 URL 查询串
来源：http://ewi.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ojb.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rsp.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lmu.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxw.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://swj.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oqq.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xtv.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://amx.shzxlz.cn

[K07] 进制转换
来源：http://uid.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iig.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vzv.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cpa.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lbk.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://utm.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oqz.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jyl.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yua.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://azg.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://zob.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wic.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ygu.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://hmn.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ufa.zdqjudy.top

Go:   encoding/gob
来源：http://sle.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://iis.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://afh.hysaishi.cn

================================================================================
来源：http://pul.sxryk.cn

L. 网络请求
来源：http://mtm.ehwqpu.com

================================================================================
来源：http://axj.meibo888.top

[L01] 发送 GET 请求
来源：http://bvq.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vok.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cxh.gaohongyu789.top

JS:   await fetch(url)
来源：http://ump.shzxlz.cn

TS:   await fetch(url)
来源：http://loh.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fjc.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://imm.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iwb.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bak.nanxinkj.top

[L02] 发送 POST JSON
来源：http://zmq.kuanghao11.cn


<!-- 参考信息 -->