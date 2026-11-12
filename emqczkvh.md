代发 wailian999

JS:   class MyError extends Error {}
来源：http://whk.fzhhl.top

TS:   class MyError extends Error {}
来源：http://lce.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://pel.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mul.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://wdh.andypj.xyz

C#:   class MyException : Exception {}
来源：http://xvl.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://clf.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://fae.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xsq.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://wez.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://mhy.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://vwv.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zhv.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://xmo.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qlb.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://pjm.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://kpn.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://dny.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://znl.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://xms.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pqx.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ijp.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://evm.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://uzp.yfazqb.com

[H07] 断言
来源：http://hnn.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://ksw.aibaodan.cn

PHP:  assert($x > 0);
来源：http://xad.ydzc1.top

JS:   console.assert(x > 0);
来源：http://iws.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://lwi.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://nwo.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nef.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://whc.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://ezr.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://hxd.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://lhe.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oxf.yfazqb.com

JS:   e.message;  e.stack
来源：http://lnx.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tbh.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://mle.fktsv.cn

Go:   err.Error()
来源：http://mcz.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://epx.hywenlv.cn

C#:   e.Message;  e.StackTrace
来源：http://kat.daxiang520.top

[H09] 带错误码的异常
来源：http://gfl.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oyz.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fqh.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zww.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mgy.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rdc.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zwv.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pjh.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rvy.hnqzz.top

[H10] 资源自动释放
来源：http://izg.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://irr.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fio.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rpn.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://itd.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vaa.andypj.xyz

Go:   defer f.Close()
来源：http://zuh.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mvn.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xrl.zdqjudy.top

================================================================================
来源：http://exw.sxryk.cn

I. 正则表达式
来源：http://vcg.zhongyouzk.top

================================================================================
来源：http://psv.ctjpmb.com

[I01] 判断是否匹配
来源：http://syu.c1oappe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sle.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://gcd.hcnkem.com

JS:   /\d+/.test(s)
来源：http://rgn.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://uwo.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://trd.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rpe.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://knv.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tdo.sufxvd.cn

[I02] 提取所有匹配
来源：http://nvd.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://dfm.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yhr.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wju.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://ykb.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nfr.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nlp.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://nir.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rax.birdmap.top

[I03] 提取捕获分组
来源：http://rbe.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lba.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xpc.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dyv.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nsd.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xfj.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ndx.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kjb.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kuk.nanxuanxn.top

[I04] 正则替换
来源：http://lgp.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ibi.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oms.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eca.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jih.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mck.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://qtr.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rnb.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cqa.cashguo.top

[I05] 按正则拆分
来源：http://sxc.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ahz.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oko.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://kjg.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://syd.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://viv.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://moi.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dqt.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ayx.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wgb.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zet.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://psg.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pmo.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wah.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vcl.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dla.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hay.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uxf.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://xzh.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vzr.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cul.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lcd.cdnleiting.top

TS:   /error/gim
来源：http://mmc.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kbf.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gpi.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://flj.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cnd.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://syw.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uxw.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wis.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kgc.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gqn.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hme.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tcs.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zyk.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jwf.aizwys.cn

================================================================================
来源：http://xyc.jqgufenzy.top

J. 日期与时间
来源：http://wwe.jyoumei.cn

================================================================================
来源：http://jgq.hongshengwenyu.top

[J01] 获取当前时间
来源：http://kzr.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dnj.hcnkem.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bff.52xcode.cn

JS:   new Date();  Date.now()
来源：http://frx.c1oappe.top

TS:   new Date();  Date.now()
来源：http://jkw.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wpu.hfpthk.cn

Go:   time.Now()
来源：http://brn.gzhubu.top

Ruby: Time.now
来源：http://jgn.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jwl.nwbrower.top

[J02] 格式化输出
来源：http://yjw.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axj.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wdz.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tcp.xuetiantiany.cn

TS:   d.toISOString()
来源：http://zbp.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mca.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://svl.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcs.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://glv.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://njr.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iwy.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://afs.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://ehh.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://vmj.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://bna.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jsm.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://pam.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nwi.epnwcf.com

[J04] 时间戳与日期互转
来源：http://btq.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://now.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uob.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yjh.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xxs.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jkf.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hic.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qqy.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qfu.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://ehz.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://xrf.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://nex.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dil.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rbo.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://dfu.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ovd.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://dbq.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://kun.cucudq.cn

[J06] 计算两时间之差
来源：http://qle.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://gds.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://jpv.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pkm.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qks.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wtd.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://vup.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://dsp.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://lel.tianlin.xyz

[J07] 比较两个日期
来源：http://gbz.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://iyw.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dfx.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://bml.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eja.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://euf.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tiz.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://eyd.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://uow.wangdashe.top

[J08] 提取年月日与星期
来源：http://skk.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://exz.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bvy.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gec.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xen.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jvv.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cwm.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://spj.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nxw.chenlongwang.top

[J09] 时区处理
来源：http://kmp.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ple.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tqh.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://msp.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xzv.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kwa.tian-w.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xjz.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wfz.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ixy.sweek.top

[J10] 取今天 / 本月第一天
来源：http://hig.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nbz.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bje.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hyr.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jao.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uwx.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gcz.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ads.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cbd.xuetiantiany.cn

================================================================================
来源：http://cwo.chenlongwang.top

K. JSON 与序列化
来源：http://byq.yj20258.top

================================================================================
来源：http://oge.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://yqd.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://djw.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gyk.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://hry.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://dfl.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rop.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://neo.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://cgu.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://bit.hcnkem.com

[K02] JSON 字符串转对象
来源：http://qch.tian-w.cn

Py:   json.loads(s)
来源：http://hrm.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bkp.hnqzz.top

JS:   JSON.parse(s)
来源：http://gzx.tanke756.top

TS:   JSON.parse(s)
来源：http://xkw.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aaf.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://erk.redwolf501.top

Ruby: JSON.parse(s)
来源：http://jvi.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ovj.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://uty.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ehn.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hzp.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fnf.hesvh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xon.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ogr.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ilx.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cyw.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mlt.sxryk.cn

[K04] 读取 JSON 文件
来源：http://kfh.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gms.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dfm.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dxp.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ylf.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ptz.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uwl.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cat.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ndm.yuanzhike.top

[K05] 深拷贝对象
来源：http://nms.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://jxe.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://hsk.cucudq.cn

JS:   structuredClone(obj)
来源：http://kcb.hysaishi.cn

TS:   structuredClone(obj)
来源：http://nzt.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xny.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qoy.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uzq.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qpk.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://yip.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pyz.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gpg.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://elr.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uns.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xqd.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wyd.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jbq.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://feo.shuidangran.top

[K07] 进制转换
来源：http://pel.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iup.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uun.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bot.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gws.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cde.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wnt.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zko.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://apf.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://obq.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://ubv.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xao.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://sjc.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://ujs.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ezj.jlsjyb.cn


<!-- 参考信息 -->