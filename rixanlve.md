代发 wailian999

TS:   throw new Error("错误信息");
来源：http://szh.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nnz.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iba.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yhf.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://rbj.daxiang520.top

[H04] 自定义异常类型
来源：http://ewq.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://hkb.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://eyu.nwbrower.top

JS:   class MyError extends Error {}
来源：http://vva.316326.xyz

TS:   class MyError extends Error {}
来源：http://pzl.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://opd.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hhe.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://dui.sxryk.cn

C#:   class MyException : Exception {}
来源：http://yrb.yj202588.top

[H05] 捕获特定类型
来源：http://zce.uphjek.com

Py:   except ValueError as e:
来源：http://xei.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mog.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://lhm.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://tgc.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://rxb.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hxg.yuxming.cn

Ruby: rescue ArgumentError => e
来源：http://qxz.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sel.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://mba.daria6918.cn

Py:   value = d.get("k") or default
来源：http://eaa.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://exe.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iud.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ulo.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rae.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yka.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://xjl.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://mdb.feifeiyinyue.top

[H07] 断言
来源：http://mus.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://ixy.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://pyx.andypj.xyz

JS:   console.assert(x > 0);
来源：http://qac.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://tur.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://itp.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xju.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://iki.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://swc.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://zfj.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://kxi.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://txj.cashguo.top

JS:   e.message;  e.stack
来源：http://lzu.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://clw.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://anu.nanxuanxn.top

Go:   err.Error()
来源：http://rgq.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://npg.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://flp.cqqwz.cn

[H09] 带错误码的异常
来源：http://lii.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pkf.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yrt.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cfe.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yzh.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lyw.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ffy.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://alv.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://xwf.gaohongyu789.top

[H10] 资源自动释放
来源：http://inj.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://tpm.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dfy.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sst.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sbc.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wlz.cheryme.top

Go:   defer f.Close()
来源：http://ied.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gzz.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dgk.tian-w.cn

================================================================================
来源：http://rrq.cdnleiting.top

I. 正则表达式
来源：http://eqm.vehdjk.com

================================================================================
来源：http://afg.pycfn.com

[I01] 判断是否匹配
来源：http://nkh.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ynj.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rtw.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://pwl.cucudq.cn

TS:   /\d+/.test(s)
来源：http://rwy.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ste.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zzd.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://eod.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://arj.jqgufenzy.top

[I02] 提取所有匹配
来源：http://cbw.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://zww.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qcm.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qsg.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://pgm.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pfu.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qee.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://fpg.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rfg.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://lly.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pts.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wtf.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cxf.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hum.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nko.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ymp.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://laf.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lql.chenzaomai.com

[I04] 正则替换
来源：http://nxb.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zmz.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://csh.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://tzb.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://xzk.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://hwi.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nsu.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://agk.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yyz.c1oappe.top

[I05] 按正则拆分
来源：http://vag.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://tvc.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xdd.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://ydf.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ecm.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://atx.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lza.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yho.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jzs.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wse.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wln.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jao.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gyy.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tvz.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zup.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ucn.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eaz.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fow.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://plu.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ndz.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://txg.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gnt.shuidangran.top

TS:   /error/gim
来源：http://ovh.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dqv.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rwq.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://yjh.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://srw.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://jgh.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xzv.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uft.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://czc.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ajq.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bnb.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://evk.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cth.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ton.yangfankeji.com

================================================================================
来源：http://pyu.daria6918.cn

J. 日期与时间
来源：http://fir.cucudq.cn

================================================================================
来源：http://plf.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://ltg.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ghx.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ngp.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://vva.smart0.xyz

TS:   new Date();  Date.now()
来源：http://qrf.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kop.yj20258888.top

Go:   time.Now()
来源：http://pzk.sxryk.cn

Ruby: Time.now
来源：http://isw.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sur.316326.xyz

[J02] 格式化输出
来源：http://zek.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zsb.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vgx.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cun.yueranfly.top

TS:   d.toISOString()
来源：http://aao.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iqt.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vqt.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qaq.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ate.jinqigufen.top

[J03] 字符串解析为日期
来源：http://wfa.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ege.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zmk.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://crm.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://hun.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nbf.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ufv.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://had.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iig.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://ldx.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ipz.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nqk.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bkp.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mhw.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tup.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rwm.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wud.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qgp.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://vwi.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://vqz.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lat.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://usv.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ean.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://klw.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kbv.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://vrv.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://zxp.epnwcf.com

[J06] 计算两时间之差
来源：http://zkv.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://xkp.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://gyq.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rmv.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tua.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://rev.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://sya.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://wmt.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://kus.jlsjyb.cn

[J07] 比较两个日期
来源：http://wdl.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://qgl.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://chf.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://yzu.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dmu.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uyi.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wpw.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://iyb.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://bbp.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://umn.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qsq.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vjl.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tha.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://etp.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nrr.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uet.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yyf.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vqg.uphjek.com

[J09] 时区处理
来源：http://ldv.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://znq.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dhh.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pre.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yus.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cvo.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rgt.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iqx.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gfm.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://uau.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qvd.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://loo.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://emx.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cwf.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://llu.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vjz.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fhu.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jcy.nwbrower.top

================================================================================
来源：http://tdf.bbcook.cn

K. JSON 与序列化
来源：http://sbi.shangyingyoupin.top

================================================================================
来源：http://tae.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://qrk.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://imb.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yfl.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://uyf.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://ida.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kbr.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://tfc.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bbh.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lze.hcnkem.com

[K02] JSON 字符串转对象
来源：http://aoj.316326.xyz

Py:   json.loads(s)
来源：http://hnl.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wsu.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://ivl.316326.xyz

TS:   JSON.parse(s)
来源：http://vmc.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zhc.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://kpu.daria6918.cn

Ruby: JSON.parse(s)
来源：http://hld.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://doe.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://yjt.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uxl.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vly.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cgu.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tsr.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wdk.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mev.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://edy.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lpp.cheryme.top

[K04] 读取 JSON 文件
来源：http://xzm.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vvi.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uqb.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ost.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hci.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vds.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gwf.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eme.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xvi.yanxiufei.cn

[K05] 深拷贝对象
来源：http://lob.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://cic.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://opp.daxiang520.top

JS:   structuredClone(obj)
来源：http://zhj.snrcjt.cn

TS:   structuredClone(obj)
来源：http://lhp.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dei.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iaf.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://idr.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yad.fengsongda.top

[K06] 解析 URL 查询串
来源：http://nvw.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gme.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cbd.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nxg.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hpy.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zgw.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://csc.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://olz.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mwb.zhoulong.xyz

[K07] 进制转换
来源：http://xva.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qpy.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hfn.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://byz.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bwc.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zaw.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pwm.daxiang520.top


<!-- 参考信息 -->