代发 wailian999

JS:   class MyError extends Error {}
来源：http://wch.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://rtu.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://hmz.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aok.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://igb.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://gbu.sufxvd.cn

[H05] 捕获特定类型
来源：http://vth.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://bjx.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://szt.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://irw.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://uqf.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://baa.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fob.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://gpy.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iot.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://hac.yj20258888.top

Py:   value = d.get("k") or default
来源：http://ofi.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://dbw.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://kdf.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iis.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://syw.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hpl.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://wfg.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://nqa.yangfankeji.com

[H07] 断言
来源：http://rpb.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://ksh.aizwys.cn

PHP:  assert($x > 0);
来源：http://ach.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://kax.smart0.xyz

TS:   console.assert(x > 0);
来源：http://leg.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://qre.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nio.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://ack.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://lya.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://sao.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://efh.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rxz.sysykeji.top

JS:   e.message;  e.stack
来源：http://dod.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ghg.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qaz.snrcjt.cn

Go:   err.Error()
来源：http://lrd.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://cps.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://dai.haohaochexian.top

[H09] 带错误码的异常
来源：http://trc.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://azi.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wws.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sds.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rvw.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zij.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dop.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wfb.ywan-chungtsiang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ymr.ybcxt.top

[H10] 资源自动释放
来源：http://exy.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://clt.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nvt.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sug.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lkv.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://prt.yueranfly.top

Go:   defer f.Close()
来源：http://zwy.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lzt.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fbw.smart0.xyz

================================================================================
来源：http://wkk.jyoumei.cn

I. 正则表达式
来源：http://usx.shanyushiyangtech.top

================================================================================
来源：http://suc.dashuyun.cn

[I01] 判断是否匹配
来源：http://dfo.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cwo.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://udq.fzhhl.top

JS:   /\d+/.test(s)
来源：http://efz.fehbvm.com

TS:   /\d+/.test(s)
来源：http://mso.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yfb.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ghz.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://pmh.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gix.daria6918.cn

[I02] 提取所有匹配
来源：http://iyz.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://ebg.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jhb.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oyu.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://iwm.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hpf.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zty.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://quo.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://udn.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://jde.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://omw.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gdv.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://shl.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hsp.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vfw.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://chg.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://txm.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mpn.feifeiyinyue.top

[I04] 正则替换
来源：http://oce.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://glu.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bkd.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://ygc.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://bsw.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://kie.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cnx.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rpw.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://axu.zhengqikj.top

[I05] 按正则拆分
来源：http://mvw.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fbe.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qqr.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://nps.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://uwg.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://snc.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wzo.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ahk.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fun.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vdx.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xub.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pjl.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://syj.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://neb.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wdh.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lvq.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rgj.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ktp.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://tdo.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fph.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iwr.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nxb.xylfe.cn

TS:   /error/gim
来源：http://qxi.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bmj.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yib.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://jqp.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uey.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://jye.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kes.sufxvd.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fdy.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://esp.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nau.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vss.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kyo.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sbv.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dyv.jqgufenzy.top

================================================================================
来源：http://llk.jyoumei.cn

J. 日期与时间
来源：http://cld.ydjk.org.cn

================================================================================
来源：http://xlg.yongpay.top

[J01] 获取当前时间
来源：http://apv.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://irb.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rng.xuanzx.com

JS:   new Date();  Date.now()
来源：http://tnq.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://jke.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xxh.hnxiangtu.top

Go:   time.Now()
来源：http://sgy.shuidangran.top

Ruby: Time.now
来源：http://cyb.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xaw.jinqigfzy.top

[J02] 格式化输出
来源：http://mcm.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wfy.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fcm.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iqd.yanxiufei.cn

TS:   d.toISOString()
来源：http://fbp.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yax.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oim.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfb.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iho.aizwys.cn

[J03] 字符串解析为日期
来源：http://iaw.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://atn.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yje.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://ogr.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://wib.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zcy.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vbj.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://hkz.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://owt.andypj.xyz

[J04] 时间戳与日期互转
来源：http://gad.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://epq.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wqd.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bpf.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zxa.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kqj.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yia.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jkk.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fdf.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://oik.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://qpx.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qqn.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zjr.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nhu.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://sox.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://znr.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://srq.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://sto.jiagoushi.top

[J06] 计算两时间之差
来源：http://ikg.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://pmj.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://mcu.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://flq.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tnw.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://jlh.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://gzr.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://fok.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://sge.bbcook.cn

[J07] 比较两个日期
来源：http://edg.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://wzy.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dqj.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://uib.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://vlr.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lip.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ksh.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aup.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://cra.ydzc1.top

[J08] 提取年月日与星期
来源：http://lra.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ogc.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ixx.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://quc.zhoulong.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mzt.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://icb.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ekh.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pgq.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qdm.tianlin.xyz

[J09] 时区处理
来源：http://khf.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://daq.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tuz.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rup.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://afb.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://idi.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhv.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ikz.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://faj.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://nmx.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ipn.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://odp.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cin.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wsf.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mrh.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zin.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nfn.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mqa.cucudq.cn

================================================================================
来源：http://dou.daria6918.cn

K. JSON 与序列化
来源：http://slx.yfazqb.com

================================================================================
来源：http://xyl.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://ilb.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hzp.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://slo.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://ejv.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://ybm.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bel.pycfn.com

Go:   json.Marshal(obj)
来源：http://fiw.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://wfu.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fwd.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://kkg.sufxvd.cn

Py:   json.loads(s)
来源：http://rfr.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bur.jianghu66.top

JS:   JSON.parse(s)
来源：http://vbs.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://fcs.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vdj.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://fhw.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://pxv.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jds.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://cut.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ltm.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bgk.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://boi.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://bcg.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vjl.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://goy.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rsp.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vkv.jianghu66.top

[K04] 读取 JSON 文件
来源：http://hdh.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fyt.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysj.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hrb.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drw.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rzl.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hpm.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zyz.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vjn.hfpthk.cn

[K05] 深拷贝对象
来源：http://fce.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://elb.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://sga.fengsongda.top

JS:   structuredClone(obj)
来源：http://bui.daxiang520.top

TS:   structuredClone(obj)
来源：http://eak.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kqa.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gji.yj20258.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yid.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://uyr.meibo888.top

[K06] 解析 URL 查询串
来源：http://fjx.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wmb.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://epe.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bnk.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rwv.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ytq.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yxs.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tuf.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dac.jinyuanbaomall.cn

[K07] 进制转换
来源：http://qdj.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://csm.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qfw.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pcv.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vts.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tql.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ozd.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nti.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ssc.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://swp.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://gmw.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cvr.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://bcv.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://zfi.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lvg.sjlbkw.cn


<!-- 参考信息 -->