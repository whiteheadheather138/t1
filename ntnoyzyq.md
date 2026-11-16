代发 wailian999

JS:   class MyError extends Error {}
来源：http://rrj.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://nbm.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://cpq.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vtn.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://loe.xylfe.cn

C#:   class MyException : Exception {}
来源：http://sfk.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://ifo.uphjek.com

Py:   except ValueError as e:
来源：http://zmq.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rre.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://afz.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://mty.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://tfq.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mut.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://htz.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://znc.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://zyp.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://ymg.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://jvm.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://lng.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://nol.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rng.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://umf.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://aiw.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://ysc.yj20258.top

[H07] 断言
来源：http://ems.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://uyt.shzxlz.cn

PHP:  assert($x > 0);
来源：http://ugp.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://cmi.yongpay.top

TS:   console.assert(x > 0);
来源：http://klm.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://dem.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://adj.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jtn.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://orw.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://bxa.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://zap.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wyk.nanxinkj.top

JS:   e.message;  e.stack
来源：http://ieg.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ukt.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qbb.yfazqb.com

Go:   err.Error()
来源：http://jrb.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://icp.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://dee.tianlin.xyz

[H09] 带错误码的异常
来源：http://diw.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oak.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ikz.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hsi.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xgq.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ked.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dzo.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://foz.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://mta.jqgufenzy.top

[H10] 资源自动释放
来源：http://wgk.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://agp.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://skn.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jga.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://spq.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zzx.kuanghao11.cn

Go:   defer f.Close()
来源：http://kun.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://amw.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jnp.zdqjudy.top

================================================================================
来源：http://efd.cucudq.cn

I. 正则表达式
来源：http://upc.hywenlv.cn

================================================================================
来源：http://jtk.pycfn.com

[I01] 判断是否匹配
来源：http://ybm.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://las.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mle.birdmap.top

JS:   /\d+/.test(s)
来源：http://ezc.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://jgq.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://anc.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nkx.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://qvz.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yxd.yj20258888.top

[I02] 提取所有匹配
来源：http://xwy.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://prk.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ixc.aibaodan.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ksn.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://bjy.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hou.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vfl.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://veg.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://six.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://upf.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uyz.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://flt.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ltm.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://snx.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pkm.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ree.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xqs.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rqn.zycfv.cn

[I04] 正则替换
来源：http://kne.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fzr.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dwf.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://rzd.havefunace.top

TS:   s.replace(/\d+/g, "#")
来源：http://sod.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://jae.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tem.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zxx.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rlx.svipenyu.cn

[I05] 按正则拆分
来源：http://rsx.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://czy.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ecj.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://cti.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://gqu.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://lom.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://usp.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://adv.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zwv.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cwg.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jnp.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xoe.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ttz.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qcs.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aqi.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cfa.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dyy.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hwn.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://ofb.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qlm.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pjk.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://red.daria6918.cn

TS:   /error/gim
来源：http://msx.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rpi.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://snd.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://eoe.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jyg.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://ifp.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bnu.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gsw.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dom.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qbo.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://aji.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://okz.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nnj.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jex.wangdashe.top

================================================================================
来源：http://tgn.shuidangran.top

J. 日期与时间
来源：http://cxa.sysykeji.top

================================================================================
来源：http://rte.pycfn.com

[J01] 获取当前时间
来源：http://pdy.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://voe.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gqb.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://pxv.iojbl.cn

TS:   new Date();  Date.now()
来源：http://smw.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fan.jiagoushi.top

Go:   time.Now()
来源：http://xsa.nanxinkj.top

Ruby: Time.now
来源：http://tsd.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://via.xuanzx.com

[J02] 格式化输出
来源：http://yhd.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ous.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bnz.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rqu.yvedp.cn

TS:   d.toISOString()
来源：http://rwt.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://exg.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fnb.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fet.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mel.316326.xyz

[J03] 字符串解析为日期
来源：http://alj.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fhu.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nof.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://euq.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://evu.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://xkk.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bwn.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://auw.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dlr.smart0.xyz

[J04] 时间戳与日期互转
来源：http://ogu.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qjn.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jio.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bsz.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lge.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mzl.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pvs.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bvi.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fwt.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://cmr.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://xdi.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sad.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cwj.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nfj.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://qwu.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eje.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://nqb.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://dba.haohaochexian.top

[J06] 计算两时间之差
来源：http://fpl.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://buh.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://ivy.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rix.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://orv.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://elg.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://jnu.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://xtg.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://zke.gotoacloud.top

[J07] 比较两个日期
来源：http://dry.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://fue.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nyu.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rcb.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://knh.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ruf.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://icx.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://bcp.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://cqp.sufxvd.cn

[J08] 提取年月日与星期
来源：http://unx.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eul.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pwy.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rww.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qma.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ojd.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://avx.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jeu.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uqc.pengpengdd.cyou

[J09] 时区处理
来源：http://uxq.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://efs.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://njh.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cma.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xyt.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wlr.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vwn.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qql.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fal.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://uzb.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fem.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lzs.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oye.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xnd.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fna.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vjh.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wla.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oky.hnqzz.top

================================================================================
来源：http://jdk.chenlongwang.top

K. JSON 与序列化
来源：http://trs.shuidangran.top

================================================================================
来源：http://pcf.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://fdj.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sxv.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yzt.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://vcb.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://jwx.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://min.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://fhg.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://hla.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vuz.hesvh.cn

[K02] JSON 字符串转对象
来源：http://hvz.hammf.cn

Py:   json.loads(s)
来源：http://ipy.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://plx.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://stf.hysaishi.cn

TS:   JSON.parse(s)
来源：http://xqu.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ici.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://wgk.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://int.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lbf.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://rrc.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gts.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ikd.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kfw.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zcw.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ehu.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sfk.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://llg.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dgp.meibo888.top

[K04] 读取 JSON 文件
来源：http://yzq.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://elz.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rvc.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ggc.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uyg.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vmv.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lqi.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://sou.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jvj.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://rtg.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://gii.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://cuc.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://dnp.tanke756.top

TS:   structuredClone(obj)
来源：http://egk.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://moi.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kzo.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ake.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xdh.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://zuj.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://evp.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cdl.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytt.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vzg.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://knk.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ico.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rwr.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dyl.jinqigufen.top

[K07] 进制转换
来源：http://xju.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ila.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tqq.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gpo.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ttk.kuanghao11.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nti.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cqa.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cst.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mcj.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://ysp.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://lxi.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://sgw.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://ige.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://pah.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ufs.sufxvd.cn


<!-- 参考信息 -->