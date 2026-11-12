代发 wailian999

[H03] 主动抛出异常
来源：http://yuj.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://cks.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oks.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://gye.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://zfe.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dez.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pvn.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zdj.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://nui.yj202588.top

[H04] 自定义异常类型
来源：http://fcn.uphjek.com

Py:   class MyError(Exception): pass
来源：http://lhh.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://qji.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://jay.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://xrw.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://dfm.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zmm.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://vie.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://srq.hnqzz.top

[H05] 捕获特定类型
来源：http://cjk.yuanzhike.top

Py:   except ValueError as e:
来源：http://zeh.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iax.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://plh.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://gss.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://boq.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ngn.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://gbd.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rks.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://rrm.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://jek.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://qdp.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://nxg.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://pml.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://brs.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cwc.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://gzx.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://gqs.ydjk.org.cn

[H07] 断言
来源：http://lwc.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://zyk.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://enq.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://uve.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://ucg.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://jho.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lhd.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nlv.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://rxj.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://hpd.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://yzz.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tfm.tarul.cn

JS:   e.message;  e.stack
来源：http://pjz.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dqc.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ado.hammf.cn

Go:   err.Error()
来源：http://zho.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://isc.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://bim.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://gqx.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://agz.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://idf.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lzz.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vui.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rqy.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vil.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://xph.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ncc.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://pms.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eea.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vxn.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://clo.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://phv.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wrh.cheryme.top

Go:   defer f.Close()
来源：http://fvp.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rhl.redwolf501.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://irj.sweek.top

================================================================================
来源：http://bts.redwolf501.top

I. 正则表达式
来源：http://kpq.zycfv.cn

================================================================================
来源：http://zsi.gzhubu.top

[I01] 判断是否匹配
来源：http://ypt.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mwg.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ddb.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://vym.ydzc1.top

TS:   /\d+/.test(s)
来源：http://tpm.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://won.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kac.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://vab.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ijr.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://zsf.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://avb.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hjg.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dog.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://czy.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ryu.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lkp.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://vjg.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oza.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://lcd.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hve.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aef.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fjh.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xor.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lzx.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://imc.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jdi.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uuu.chenlongwang.top

[I04] 正则替换
来源：http://mwm.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://unr.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pwx.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://trs.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://qcp.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://uqo.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rht.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://maz.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vdd.xylfe.cn

[I05] 按正则拆分
来源：http://fcj.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://hxf.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vuu.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://qsl.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://aau.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://dei.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://skb.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uxa.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jgo.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kjf.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://itx.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lxr.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ecu.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jjw.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cea.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mcu.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dmx.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mgi.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://rve.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ztn.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uvn.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ztl.chenzaomai.com

TS:   /error/gim
来源：http://hmr.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gnx.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pbv.fehbvm.com

Ruby: s.scan(/error/i)
来源：http://ktu.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qei.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://nvp.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mvq.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gac.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://udl.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ixa.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://tde.c1oappe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bbt.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://svk.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fla.wangshuangyany.cn

================================================================================
来源：http://uko.ctjpmb.com

J. 日期与时间
来源：http://kiu.aibaodan.cn

================================================================================
来源：http://dvo.quarkkingdee.top

[J01] 获取当前时间
来源：http://xqa.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mqj.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ewb.cashguo.top

JS:   new Date();  Date.now()
来源：http://hhl.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://ept.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vij.nanxinkj.top

Go:   time.Now()
来源：http://yvu.havefunace.top

Ruby: Time.now
来源：http://kjm.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hsz.jinqigufen.top

[J02] 格式化输出
来源：http://otf.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vjt.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nts.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vzu.jqgfzy.top

TS:   d.toISOString()
来源：http://uhc.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cir.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xvc.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sak.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mjo.andypj.xyz

[J03] 字符串解析为日期
来源：http://vif.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cuu.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mnr.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://wog.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://fuo.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://oyt.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sjm.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://mem.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iek.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://sjm.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sgm.shuidangran.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lfm.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eef.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://eyd.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zmh.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://liw.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mhz.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ysv.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://bct.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://xlt.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ezp.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blo.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hsq.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://svl.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://siz.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://iig.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://xba.cashguo.top

[J06] 计算两时间之差
来源：http://vjz.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://cof.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://hnj.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mkq.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cau.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://akk.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://hsj.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://lty.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://mqz.vehdjk.com

[J07] 比较两个日期
来源：http://zrv.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://syb.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wkz.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://cki.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://gtc.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ycw.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yki.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://sig.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://vrx.cucudq.cn

[J08] 提取年月日与星期
来源：http://jtp.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jek.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iuf.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://upv.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://biy.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dsd.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yft.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mrm.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rhs.pycfn.com

[J09] 时区处理
来源：http://rxo.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ctb.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://veh.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://edi.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://maw.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mnt.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xbk.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ywn.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kpl.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://ujy.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ugj.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lem.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kbf.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lux.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lhr.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rht.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mbi.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vnc.jqgfzy.top

================================================================================
来源：http://xug.shuidangran.top

K. JSON 与序列化
来源：http://uzl.cdnleiting.top

================================================================================
来源：http://xgy.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://pin.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gta.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hfk.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://tvj.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://xlc.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nyc.sxryk.cn

Go:   json.Marshal(obj)
来源：http://qxn.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jgn.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://avm.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://fam.zhiwuduotai.top

Py:   json.loads(s)
来源：http://oen.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://smr.epnwcf.com

JS:   JSON.parse(s)
来源：http://tqg.fktsv.cn

TS:   JSON.parse(s)
来源：http://fac.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hra.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://zgk.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://uwh.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oli.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://pqp.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bgj.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sfl.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kpx.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wsh.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cou.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ovk.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://ujv.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://axg.jinyuanbaomall.cn

[K04] 读取 JSON 文件
来源：http://yke.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iqj.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qaa.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://evz.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wac.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xfz.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pis.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzx.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zfd.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://xxh.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://qdb.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://vul.316326.xyz

JS:   structuredClone(obj)
来源：http://kil.chenzaomai.com

TS:   structuredClone(obj)
来源：http://ljg.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://lvr.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nis.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jyd.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ahk.hnqzz.top

[K06] 解析 URL 查询串
来源：http://ppf.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oob.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bbl.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qvo.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ifw.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnz.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kfo.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uvx.cheryme.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://btf.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://vtj.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hjv.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://obe.xziqi.cn


<!-- 参考信息 -->