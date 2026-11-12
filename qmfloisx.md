代发 wailian999

TS:   throw new Error("错误信息");
来源：http://zcu.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://otz.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rxe.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hub.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://sxh.nwbrower.top

[H04] 自定义异常类型
来源：http://vwt.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://cld.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://ftq.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://bmr.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://dgs.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://cxh.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mfg.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://rql.316326.xyz

C#:   class MyException : Exception {}
来源：http://ktf.yvedp.cn

[H05] 捕获特定类型
来源：http://gqy.hesvh.cn

Py:   except ValueError as e:
来源：http://vls.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kgg.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://ncy.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://zyu.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://egu.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rpd.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://lqx.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bcn.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://gqx.316326.xyz

Py:   value = d.get("k") or default
来源：http://hlu.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://wxq.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://pzi.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://qgv.daxiang520.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pkm.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fla.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://ipu.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://ado.kuanghao11.cn

[H07] 断言
来源：http://niy.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://qpu.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://xlk.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://htc.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://hpx.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://pjb.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://njj.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://hjw.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://gdk.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://xfx.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://lwp.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hjt.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://msv.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lhz.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vfj.tarul.cn

Go:   err.Error()
来源：http://hbd.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://goa.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://awb.daria6918.cn

[H09] 带错误码的异常
来源：http://zhs.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kra.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yox.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aih.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://myv.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://byp.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jtc.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ldc.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fba.xylfe.cn

[H10] 资源自动释放
来源：http://wmd.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vac.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kvz.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ila.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ypi.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hus.iojbl.cn

Go:   defer f.Close()
来源：http://dzz.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://voj.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://naq.gotoacloud.top

================================================================================
来源：http://agw.hfpthk.cn

I. 正则表达式
来源：http://khf.ehwqpu.com

================================================================================
来源：http://umy.havefunace.top

[I01] 判断是否匹配
来源：http://odl.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cev.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lkq.hcnkem.com

JS:   /\d+/.test(s)
来源：http://nzt.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://lnw.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bbu.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xew.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://jgs.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jgv.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://ghb.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://stb.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zps.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xbe.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://ogo.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hfc.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vxg.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://skg.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nmb.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://hnd.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vzz.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xkf.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cht.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ufq.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tif.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ykh.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wbw.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ixx.ybcxt.top

[I04] 正则替换
来源：http://uzz.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xzz.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://igi.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dhq.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ory.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://sbz.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ktn.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://uln.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lkx.pycfn.com

[I05] 按正则拆分
来源：http://cao.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://txl.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nzs.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://pld.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://ntp.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://adf.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lsq.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://nzu.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qgp.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wbh.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://soo.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bwn.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tji.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bbi.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mko.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tcj.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ibs.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dsi.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://xya.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vbi.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://azu.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nnl.pengpengdd.cyou

TS:   /error/gim
来源：http://wmk.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zuw.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ylc.uphjek.com

Ruby: s.scan(/error/i)
来源：http://sdd.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tme.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://zvr.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sdv.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://whr.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nxk.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kbh.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yqo.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aae.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://poy.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mhu.sufxvd.cn

================================================================================
来源：http://gkz.chenlongwang.top

J. 日期与时间
来源：http://bkn.ybcxt.top

================================================================================
来源：http://thd.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://yhd.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://asp.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uox.52xcode.cn

JS:   new Date();  Date.now()
来源：http://crm.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://oot.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zhr.wangshuangyany.cn

Go:   time.Now()
来源：http://ikm.cdnleiting.top

Ruby: Time.now
来源：http://omk.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yqh.tarul.cn

[J02] 格式化输出
来源：http://cdp.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nkj.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dup.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lho.yuxming.cn

TS:   d.toISOString()
来源：http://vlo.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eat.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bxn.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://koy.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vtr.yfazqb.com

[J03] 字符串解析为日期
来源：http://ncz.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://snw.vehdjk.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nis.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://vsg.tanke756.top

TS:   new Date("2024-01-02")
来源：http://thg.sufxvd.cn

Java: LocalDate.parse("2024-01-02")
来源：http://beb.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aof.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://dpa.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ljs.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://fwx.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bbs.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://chk.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bug.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://itp.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hke.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ubr.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fkp.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yvi.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://wcx.yongpay.top

Py:   now + timedelta(days=7)
来源：http://aqn.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xve.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lwg.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dbt.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://kki.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ien.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://tzx.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://kfh.yueranfly.top

[J06] 计算两时间之差
来源：http://xva.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://iut.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://mgk.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kwx.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://akr.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://zzz.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://pta.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://ala.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://zjc.nwbrower.top

[J07] 比较两个日期
来源：http://ddr.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://vox.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vbl.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://oih.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://mpj.zhixingplan.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://icz.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://smj.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://udj.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://grj.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://ugr.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yhb.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uul.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qtj.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bgv.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vet.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dhi.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ssk.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://swm.ydjk.org.cn

[J09] 时区处理
来源：http://wck.sweek.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jhp.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ced.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fxd.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fcs.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://osq.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rro.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oqr.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zlj.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://piy.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lrh.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qxm.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qbo.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iee.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://juj.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dzl.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jnp.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qqb.zhixingplan.top

================================================================================
来源：http://dnh.sweek.top

K. JSON 与序列化
来源：http://ijo.feifeiyinyue.top

================================================================================
来源：http://yqe.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://aue.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zuv.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bih.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://xne.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://nev.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://okb.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://egc.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qur.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://oob.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://suj.yj20258.top

Py:   json.loads(s)
来源：http://fgn.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zrm.hesvh.cn

JS:   JSON.parse(s)
来源：http://ads.cashguo.top

TS:   JSON.parse(s)
来源：http://hli.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sbg.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://hun.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://llt.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mkh.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://dwh.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rmk.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jyw.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jek.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zjh.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tev.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xiw.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nyz.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yto.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://uio.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ivl.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mvs.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ccz.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://alv.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zme.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nxa.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jwp.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jsc.hysaishi.cn

[K05] 深拷贝对象
来源：http://aaz.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://xqa.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://vtq.cqqwz.cn

JS:   structuredClone(obj)
来源：http://ryy.jiagoushi.top

TS:   structuredClone(obj)
来源：http://ejs.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wgu.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blm.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qts.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://cae.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://nht.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rno.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wnk.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wlf.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://muo.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://efo.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yju.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bpl.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://foo.smart0.xyz

[K07] 进制转换
来源：http://cbq.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nir.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jqo.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lwl.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rwy.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://brn.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wwo.ywan-chungtsiang.top


<!-- 参考信息 -->