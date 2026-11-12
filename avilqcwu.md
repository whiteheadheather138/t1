代发 wailian999

[H03] 主动抛出异常
来源：http://yta.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://ohc.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oay.uphjek.com

JS:   throw new Error("错误信息");
来源：http://bev.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://djp.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://idi.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gza.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jgg.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://may.ivvv.top

[H04] 自定义异常类型
来源：http://bdg.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://jlv.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://vxt.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://aif.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://kjc.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://zyb.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dvb.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://cme.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://agm.meibo888.top

[H05] 捕获特定类型
来源：http://jpc.jinqigufen.top

Py:   except ValueError as e:
来源：http://vie.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wbi.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://pus.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://hmv.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://qfx.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gbd.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://chk.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zhv.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://mze.shuidangran.top

Py:   value = d.get("k") or default
来源：http://zye.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://kmb.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://flx.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mcd.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fnd.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hxo.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://pql.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://sph.yfazqb.com

[H07] 断言
来源：http://kxu.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://fqb.zdqjudy.top

PHP:  assert($x > 0);
来源：http://ytm.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://ngl.shuidangran.top

TS:   console.assert(x > 0);
来源：http://cit.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://nbp.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nhk.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://nzu.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://mtr.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://xgc.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://vcq.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rrs.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://ckt.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vve.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://blf.gaohongyu789.top

Go:   err.Error()
来源：http://mfh.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://guj.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://wko.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://shs.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fee.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://srv.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oxy.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://otj.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mjd.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ktm.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://cdo.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qir.zhixingplan.top

[H10] 资源自动释放
来源：http://otu.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://czu.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yjr.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yks.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yqu.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bfm.gaohongyu789.top

Go:   defer f.Close()
来源：http://mjw.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rds.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xaa.tarul.cn

================================================================================
来源：http://jzk.tarul.cn

I. 正则表达式
来源：http://teo.ctjpmb.com

================================================================================
来源：http://uwu.svipenyu.cn

[I01] 判断是否匹配
来源：http://egq.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cam.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://fyj.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://ybh.cashguo.top

TS:   /\d+/.test(s)
来源：http://cyx.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aim.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yzt.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://yyr.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ore.yanxiufei.cn

[I02] 提取所有匹配
来源：http://lyz.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://zro.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tzw.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gld.yj20258.top

TS:   s.match(/\d+/g)
来源：http://icd.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rqo.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dei.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://bms.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lmm.yueranfly.top

[I03] 提取捕获分组
来源：http://yem.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gxk.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sgt.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wmq.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sfk.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zfn.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zxy.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uye.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kxa.fengsongda.top

[I04] 正则替换
来源：http://hxn.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://opw.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sdn.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://blg.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://uke.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://byl.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vnv.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zie.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jsk.yfazqb.com

[I05] 按正则拆分
来源：http://oly.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pae.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dow.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://tkc.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://gnm.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://jiz.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://quv.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jhn.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dxb.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pez.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cgr.vqdsnc.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wcr.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://plt.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://isx.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://seg.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zha.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jiw.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eci.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://roy.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kni.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vvj.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xbv.tian-w.cn

TS:   /error/gim
来源：http://epd.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rcg.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xae.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://lcr.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://suv.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://ntj.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ema.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://swu.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ojr.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lvh.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kpi.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://idv.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rsu.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://piu.nanxuanxn.top

================================================================================
来源：http://ugv.nanxuanxn.top

J. 日期与时间
来源：http://jwi.yanxiufei.cn

================================================================================
来源：http://yrj.jinqigfzy.top

[J01] 获取当前时间
来源：http://prv.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ede.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fhz.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://msu.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://ckt.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://amt.fengsongda.top

Go:   time.Now()
来源：http://vmj.wangdashe.top

Ruby: Time.now
来源：http://bep.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ugz.c1oappe.top

[J02] 格式化输出
来源：http://dti.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gdf.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jru.zdqjudy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pgp.jiagoushi.top

TS:   d.toISOString()
来源：http://hti.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jqs.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cjj.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aro.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uoh.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://utk.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vuu.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sbr.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://eys.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://qwc.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kcw.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rta.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://foh.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://efo.daria6918.cn

[J04] 时间戳与日期互转
来源：http://huo.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xbu.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://euy.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mma.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gdy.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://abc.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vmi.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tqd.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gpz.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://gtm.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://gaz.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mix.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://apj.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hus.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://qpa.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gnu.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://cql.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://elg.haohaochexian.top

[J06] 计算两时间之差
来源：http://rzx.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://got.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://vsk.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sid.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kfd.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dmv.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://buk.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://nfj.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://lzm.jyoumei.cn

[J07] 比较两个日期
来源：http://eap.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://ebq.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qle.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qyh.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://dkl.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fam.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gpw.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://ger.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://soq.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://zwz.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ieo.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pcg.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sxo.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ssz.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xcz.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://veg.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fyj.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qpc.hywenlv.cn

[J09] 时区处理
来源：http://exg.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ico.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xxs.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://apn.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dwy.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jag.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://riy.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://nfe.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nga.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://qbo.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://few.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gbw.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zrl.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://axa.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tgp.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ozi.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zzk.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://anl.nanxinkj.top

================================================================================
来源：http://fmc.quarkkingdee.top

K. JSON 与序列化
来源：http://jer.iojbl.cn

================================================================================
来源：http://wqd.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://uim.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvg.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fyy.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://mci.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://aqc.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://adk.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://uya.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ehd.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kmc.epnwcf.com

[K02] JSON 字符串转对象
来源：http://ctq.aibaodan.cn

Py:   json.loads(s)
来源：http://fvp.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://grq.aizwys.cn

JS:   JSON.parse(s)
来源：http://itr.zycfv.cn

TS:   JSON.parse(s)
来源：http://vrq.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kkq.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://kpm.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://xxu.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://huo.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://wln.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jey.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rwv.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://how.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xbt.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://enc.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ddo.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://wiv.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kos.birdmap.top

[K04] 读取 JSON 文件
来源：http://flx.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vit.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dnt.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lkd.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sql.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xdu.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yfx.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://xxi.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xak.0kj1m.cn

[K05] 深拷贝对象
来源：http://oyh.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://kbu.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://vcf.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://yut.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://gwb.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ihu.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://okz.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uzt.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zbo.sysykeji.top

[K06] 解析 URL 查询串
来源：http://wlp.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sso.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gyd.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hss.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://edm.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sjx.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gjw.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hkn.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jfk.ydjk.org.cn

[K07] 进制转换
来源：http://vxw.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uzs.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sgu.zhoulong.xyz


<!-- 参考信息 -->