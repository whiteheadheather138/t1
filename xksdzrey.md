代发 wailian999

TS:   throw new Error("错误信息");
来源：http://sbj.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hae.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pug.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vej.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ojz.hammf.cn

[H04] 自定义异常类型
来源：http://fxm.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://aek.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kok.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://umg.52xcode.cn

TS:   class MyError extends Error {}
来源：http://sor.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://cbu.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gzc.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://qsd.hcnkem.com

C#:   class MyException : Exception {}
来源：http://xyk.jinqigufen.top

[H05] 捕获特定类型
来源：http://cim.fzhhl.top

Py:   except ValueError as e:
来源：http://xlc.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ffx.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://jxo.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://xhc.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://fic.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fre.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://hhv.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dzx.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://lwv.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://zts.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://jqf.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hjz.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://ahj.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eeo.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ujd.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://wdm.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://gda.shuidangran.top

[H07] 断言
来源：http://zcg.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://vde.ydzc1.top

PHP:  assert($x > 0);
来源：http://wlo.zhiwuduotai.top

JS:   console.assert(x > 0);
来源：http://kfi.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://xmp.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://blc.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pne.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://vag.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://nnz.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://edd.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://hsq.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tia.zycfv.cn

JS:   e.message;  e.stack
来源：http://lgo.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://abj.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://yls.daxiang520.top

Go:   err.Error()
来源：http://yhf.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://ooc.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://gwj.nanxinkj.top

[H09] 带错误码的异常
来源：http://rfa.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rcw.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cpi.zhaomingkeji.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://quj.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uox.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nbk.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sxk.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qda.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nzy.mhx1999.top

[H10] 资源自动释放
来源：http://sof.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://azb.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dfi.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fjw.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://avu.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oqt.xylfe.cn

Go:   defer f.Close()
来源：http://ssr.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ssa.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tze.tanke756.top

================================================================================
来源：http://vkf.hysaishi.cn

I. 正则表达式
来源：http://vti.yj20258.top

================================================================================
来源：http://jga.fktsv.cn

[I01] 判断是否匹配
来源：http://tat.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vdi.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wpe.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://qss.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://xha.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ett.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://leh.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://uni.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jwl.jqgufenzy.top

[I02] 提取所有匹配
来源：http://qww.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://tjj.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ogl.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zah.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://sdb.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://grf.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fzm.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://nib.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oiq.zdbjq.cn

[I03] 提取捕获分组
来源：http://pdf.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zsx.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ncz.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eim.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yej.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uhw.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ogw.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://svy.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ieh.fanxiaobao.xyz

[I04] 正则替换
来源：http://uwf.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dwk.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fjr.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://gpo.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://qir.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://cfi.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qcs.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jyj.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aon.meibo888.top

[I05] 按正则拆分
来源：http://fmv.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://qcm.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qma.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://nab.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://nmj.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://uws.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aeg.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://myi.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nqd.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bpf.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uis.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pna.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ssz.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hfw.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://soe.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ciy.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://llc.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oxx.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://pak.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fqk.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dea.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kst.epnwcf.com

TS:   /error/gim
来源：http://edu.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ajx.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ztj.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://arg.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aqd.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://lbs.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://deg.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bbp.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://szu.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rli.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://vbe.yuanzhike.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://egd.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mtn.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gxl.jinghuilouyu.cn

================================================================================
来源：http://xss.ybcxt.top

J. 日期与时间
来源：http://jfv.cheryme.top

================================================================================
来源：http://gyz.jinqigfzy.top

[J01] 获取当前时间
来源：http://vqn.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xtw.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hzx.tian-w.cn

JS:   new Date();  Date.now()
来源：http://wpp.ivvv.top

TS:   new Date();  Date.now()
来源：http://glv.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nmr.snrcjt.cn

Go:   time.Now()
来源：http://qps.birdmap.top

Ruby: Time.now
来源：http://nrp.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vyk.shuidangran.top

[J02] 格式化输出
来源：http://uda.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tez.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kqh.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qiu.jqgfzy.top

TS:   d.toISOString()
来源：http://uyw.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tzc.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rxq.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jec.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ito.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://jen.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uon.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zeb.yongpay.top

JS:   new Date("2024-01-02")
来源：http://mai.ivvv.top

TS:   new Date("2024-01-02")
来源：http://dqx.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://piq.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fub.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://pcn.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hil.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://oun.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://leb.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pxb.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wrx.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zyx.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qfo.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hiz.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vbl.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://itx.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://oay.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://nfq.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rfg.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzt.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yfj.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://keo.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yoo.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://jgh.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://wmp.uphjek.com

[J06] 计算两时间之差
来源：http://xuy.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://hpk.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://drv.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ddz.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iwg.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://lgt.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://ubj.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://sxu.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://qnv.epnwcf.com

[J07] 比较两个日期
来源：http://oka.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://oej.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zdu.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://tnu.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://prb.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rqf.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ycr.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://wmc.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://fkr.hammf.cn

[J08] 提取年月日与星期
来源：http://jxr.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zqf.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pwi.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qsu.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kdg.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qkq.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xcy.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qvz.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uqx.snrcjt.cn

[J09] 时区处理
来源：http://rao.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mfc.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zzx.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwi.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ood.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lha.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://csk.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kaj.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rac.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://zkt.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qqv.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nbu.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mpj.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iof.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yyz.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pfp.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cut.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ake.andypj.xyz

================================================================================
来源：http://ljp.jinqigfzy.top

K. JSON 与序列化
来源：http://swz.svipenyu.cn

================================================================================
来源：http://okh.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://wni.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kqr.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jxj.yongpay.top

JS:   JSON.stringify(obj)
来源：http://quk.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://qdy.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hui.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://vou.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://ior.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ygi.c1oappe.top

[K02] JSON 字符串转对象
来源：http://ofj.pycfn.com

Py:   json.loads(s)
来源：http://wwo.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uqo.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://gwq.yvedp.cn

TS:   JSON.parse(s)
来源：http://ubh.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://csj.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://mgh.pycfn.com

Ruby: JSON.parse(s)
来源：http://ydp.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xxt.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://dce.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://euu.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mdp.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jua.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://owo.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jfa.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xlg.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://cor.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://irl.yueranfly.top

[K04] 读取 JSON 文件
来源：http://xye.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mtb.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://apz.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://udp.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mif.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kez.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mhc.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kri.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ehi.hysaishi.cn

[K05] 深拷贝对象
来源：http://mtk.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://fiy.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://gln.hywenlv.cn

JS:   structuredClone(obj)
来源：http://bew.ctjpmb.com

TS:   structuredClone(obj)
来源：http://qvi.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rft.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ymv.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uer.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yjz.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://brg.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zle.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mjg.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xrt.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vli.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lmx.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://alu.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hoz.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jbp.yuxming.cn

[K07] 进制转换
来源：http://ilc.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xmt.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xyf.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mgq.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zui.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zlt.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://htd.gogol.net.cn


<!-- 参考信息 -->