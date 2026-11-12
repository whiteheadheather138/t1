代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://bcc.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vic.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iyi.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hkn.jianghu66.top

[H03] 主动抛出异常
来源：http://gxh.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://zoe.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://upp.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://zls.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://szy.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfl.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sve.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ecm.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://uux.hcnkem.com

[H04] 自定义异常类型
来源：http://vlr.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://xnd.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hlq.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://fbd.hnqzz.top

TS:   class MyError extends Error {}
来源：http://ifo.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://tjm.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cgc.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://zur.aizwys.cn

C#:   class MyException : Exception {}
来源：http://muf.bjfxy.top

[H05] 捕获特定类型
来源：http://zkp.c1oappe.top

Py:   except ValueError as e:
来源：http://fiy.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jfu.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://fie.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://lvd.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://tlk.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gnt.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://skp.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://imn.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://xpm.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://exa.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://xkk.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://kqq.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aor.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://osm.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://exf.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://lpi.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://jml.xingfuxueyuan.xyz

[H07] 断言
来源：http://csk.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://jga.yuxming.cn

PHP:  assert($x > 0);
来源：http://zdk.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://qxv.gzhubu.top

TS:   console.assert(x > 0);
来源：http://sgb.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://amc.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://psn.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tqq.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://msv.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://vkf.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://hpt.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mxw.cdnleiting.top

JS:   e.message;  e.stack
来源：http://drv.guannengcc.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uhl.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://rwz.yj20258888.top

Go:   err.Error()
来源：http://kua.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://nxr.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://din.c1oappe.top

[H09] 带错误码的异常
来源：http://ohz.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nrs.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bet.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oxd.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ljv.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zmz.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gbc.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ooj.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://owi.wangdashe.top

[H10] 资源自动释放
来源：http://zeh.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mmh.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iqy.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nhk.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kzo.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wgz.fktsv.cn

Go:   defer f.Close()
来源：http://dpj.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wfu.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iwd.fehbvm.com

================================================================================
来源：http://uhw.zhixingplan.top

I. 正则表达式
来源：http://aqf.shanyushiyangkeji.top

================================================================================
来源：http://pee.cashguo.top

[I01] 判断是否匹配
来源：http://mps.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nhx.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://mug.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://ilw.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://xlq.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bvp.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zah.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://lfn.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rfu.sufxvd.cn

[I02] 提取所有匹配
来源：http://yvw.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://llc.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xlm.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ots.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://iqy.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pui.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qjo.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://xxh.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gfr.fehbvm.com

[I03] 提取捕获分组
来源：http://mtt.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kfl.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://osz.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://heh.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tij.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://avo.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://djy.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ilc.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://veg.c1oappe.top

[I04] 正则替换
来源：http://tko.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://asy.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ilv.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bfj.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://mtz.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://aas.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bcf.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wiy.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yrw.316326.xyz

[I05] 按正则拆分
来源：http://woc.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ftm.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jag.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://cpe.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://exj.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://cxi.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rpl.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ygg.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ofa.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pmo.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cnf.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yhh.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjj.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hws.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sro.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yji.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://evd.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xsq.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://uzn.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oth.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oky.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cnl.yuanzhike.top

TS:   /error/gim
来源：http://ypz.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tgq.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ejw.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://raa.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lby.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://kuq.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://avx.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mcb.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tnp.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vvr.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://swx.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zlm.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fjv.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bdp.ydzc1.top

================================================================================
来源：http://ogg.yuanzhike.top

J. 日期与时间
来源：http://sbj.shangyingyoupin.top

================================================================================
来源：http://dja.andypj.xyz

[J01] 获取当前时间
来源：http://wwq.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ihi.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://guc.sweek.top

JS:   new Date();  Date.now()
来源：http://bxc.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://uvb.chenjidiqi.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://kgj.jqgufenzy.top

Go:   time.Now()
来源：http://ndp.cheryme.top

Ruby: Time.now
来源：http://ogz.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tso.fktsv.cn

[J02] 格式化输出
来源：http://uxz.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://odo.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mey.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lev.fehbvm.com

TS:   d.toISOString()
来源：http://vkc.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uab.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jrb.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mwu.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wfd.haohaochexian.top

[J03] 字符串解析为日期
来源：http://eyh.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gud.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hfa.yongpay.top

JS:   new Date("2024-01-02")
来源：http://czb.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://omp.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://jue.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mfw.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://nic.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vde.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://cke.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hws.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://obx.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bss.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://wzc.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jot.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yfe.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qnk.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vmm.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://dcv.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://svl.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://okv.svipenyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oop.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hns.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://stq.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://htt.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://aki.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://itp.jyoumei.cn

[J06] 计算两时间之差
来源：http://mhn.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://ljw.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://gho.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tva.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ofw.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://saf.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://usw.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://aub.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://vmz.hcnkem.com

[J07] 比较两个日期
来源：http://fot.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://zmj.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tgj.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qfr.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://cld.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://scy.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sjs.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bfc.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://yvd.zycfv.cn

[J08] 提取年月日与星期
来源：http://alm.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kzt.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yvg.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zwl.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pfl.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oxw.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://snz.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dfa.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oww.hysaishi.cn

[J09] 时区处理
来源：http://jhr.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pcd.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iao.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eio.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yic.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://prm.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sob.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ins.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iwx.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://azi.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ikw.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cmi.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aqy.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cts.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mik.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tnb.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vyd.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zse.jyoumei.cn

================================================================================
来源：http://vmz.wangshuangyany.cn

K. JSON 与序列化
来源：http://ono.ydjk.org.cn

================================================================================
来源：http://fmz.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://rup.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mlk.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ekq.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://lhw.tanke756.top

TS:   JSON.stringify(obj)
来源：http://mbm.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xxv.aizwys.cn

Go:   json.Marshal(obj)
来源：http://snl.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://amj.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hvw.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://twd.yfazqb.com

Py:   json.loads(s)
来源：http://jat.sufxvd.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ygz.sufxvd.cn

JS:   JSON.parse(s)
来源：http://aku.hesvh.cn

TS:   JSON.parse(s)
来源：http://vau.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://njl.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://tvb.nwbrower.top

Ruby: JSON.parse(s)
来源：http://rmc.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cdk.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://who.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uwh.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jsf.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://iem.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ypi.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://afz.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://irk.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://rzs.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bnw.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://hah.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xgi.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rbx.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xpx.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pwj.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cjc.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kog.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zpl.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hex.zdbjq.cn

[K05] 深拷贝对象
来源：http://sgn.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://soo.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://zbr.hesvh.cn

JS:   structuredClone(obj)
来源：http://wul.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://wfj.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xaq.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cok.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ylb.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ngd.tarul.cn

[K06] 解析 URL 查询串
来源：http://qzi.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yhz.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://etb.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uns.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://crl.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hjd.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://nrh.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iys.daria6918.cn


<!-- 参考信息 -->