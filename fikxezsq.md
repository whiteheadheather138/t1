代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://qqf.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://viz.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cej.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmh.jqgfzy.top

[H03] 主动抛出异常
来源：http://adv.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://jab.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixh.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://nsj.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://shg.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dgs.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yyc.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://nzq.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://udf.bjfxy.top

[H04] 自定义异常类型
来源：http://mlv.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://trp.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://qfj.guannengcc.top

JS:   class MyError extends Error {}
来源：http://auw.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://zud.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://mfd.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jap.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://ebt.jianghu66.top

C#:   class MyException : Exception {}
来源：http://vxb.0kj1m.cn

[H05] 捕获特定类型
来源：http://ceg.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://aai.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zav.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://epb.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://bha.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://iqp.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ytf.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://cxv.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qfc.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://gmd.wangdashe.top

Py:   value = d.get("k") or default
来源：http://vem.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://fiu.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://gro.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://dsk.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://myn.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://obl.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://vxt.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://kug.yueranfly.top

[H07] 断言
来源：http://oaf.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://cwy.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://zyw.aizwys.cn

JS:   console.assert(x > 0);
来源：http://joq.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://nmu.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://ngy.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wau.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://djh.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://nvv.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://imb.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://jgu.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vlf.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://yfh.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://zzx.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gyt.dianchejie.cn

Go:   err.Error()
来源：http://cmt.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://dnj.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://adr.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://guy.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yfd.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mrw.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vud.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bxn.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xmc.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kid.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://qsn.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sxa.sysykeji.top

[H10] 资源自动释放
来源：http://xsr.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://epw.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ljr.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://svm.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hxu.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sdn.ppjwa.cn

Go:   defer f.Close()
来源：http://qkr.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ixj.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://caw.ctjpmb.com

================================================================================
来源：http://cdr.yj20258888.top

I. 正则表达式
来源：http://jzy.ctjpmb.com

================================================================================
来源：http://oei.yvedp.cn

[I01] 判断是否匹配
来源：http://mee.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nsd.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://zue.ybcxt.top

JS:   /\d+/.test(s)
来源：http://jea.meibo888.top

TS:   /\d+/.test(s)
来源：http://fyq.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvs.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kjc.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://krm.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ymt.snrcjt.cn

[I02] 提取所有匹配
来源：http://qps.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://lxo.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jfa.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kki.sweek.top

TS:   s.match(/\d+/g)
来源：http://tmx.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nrn.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zbd.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://gsj.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wia.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://kcm.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tfc.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zen.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jxv.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qnb.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iev.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nco.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rtf.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sej.smart0.xyz

[I04] 正则替换
来源：http://lvc.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ncr.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rpp.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wfs.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://aou.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pli.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cvn.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kaf.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://awm.pengpengdd.cyou

[I05] 按正则拆分
来源：http://jjp.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://din.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://diy.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://qik.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://geh.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://ijt.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qsy.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://cml.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bmp.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wgd.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nyr.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zex.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lff.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xvx.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lqp.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tsr.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wkb.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ejr.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://xov.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rvs.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wdv.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lut.jianghu66.top

TS:   /error/gim
来源：http://eva.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bnt.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://myb.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://wez.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://edq.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://nll.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hdv.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fbo.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxc.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tez.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hou.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://udc.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dmz.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fql.bjfxy.top

================================================================================
来源：http://mbh.fzhhl.top

J. 日期与时间
来源：http://muh.fanxiaobao.xyz

================================================================================
来源：http://bqn.nwbrower.top

[J01] 获取当前时间
来源：http://wla.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://fhf.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hxh.zhaomingkeji.xyz

JS:   new Date();  Date.now()
来源：http://mog.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://eas.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rhq.xinyue.icu

Go:   time.Now()
来源：http://dnt.wangdashe.top

Ruby: Time.now
来源：http://zag.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xnt.birdmap.top

[J02] 格式化输出
来源：http://ber.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zqf.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nue.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zzf.hammf.cn

TS:   d.toISOString()
来源：http://swo.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tup.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://its.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uhe.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ztp.hesvh.cn

[J03] 字符串解析为日期
来源：http://zhe.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qmf.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bin.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://hxw.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://iei.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://uda.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zre.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xzt.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gts.jianghu66.top

[J04] 时间戳与日期互转
来源：http://yuz.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jat.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qhu.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yqg.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bob.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sxm.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gyr.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gwy.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ven.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://xnx.sweek.top

Py:   now + timedelta(days=7)
来源：http://wxy.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://efa.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://onm.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpx.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://cty.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ojh.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://sox.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://zto.aizwys.cn

[J06] 计算两时间之差
来源：http://pqm.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://usj.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://oec.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ggg.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ukg.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lmz.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://isc.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://fxe.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://edf.jlsjyb.cn

[J07] 比较两个日期
来源：http://dch.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ysg.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sep.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gra.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jlv.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vmt.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ugn.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ikq.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://nks.yongpay.top

[J08] 提取年月日与星期
来源：http://swo.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pps.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xuh.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wal.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://owt.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vhc.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://epk.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://era.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tvk.epnwcf.com

[J09] 时区处理
来源：http://tlc.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vnw.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qnk.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xmd.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sfs.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dlw.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ftp.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://znv.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gad.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://chf.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://jhe.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aqf.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nmj.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vhy.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qom.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sde.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lnf.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hvg.jinqigfzy.top

================================================================================
来源：http://rud.iojbl.cn

K. JSON 与序列化
来源：http://ajs.gotoacloud.top

================================================================================
来源：http://rpj.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://ixu.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gdy.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jco.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://jlo.tanke756.top

TS:   JSON.stringify(obj)
来源：http://ryl.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lrn.yfazqb.com

Go:   json.Marshal(obj)
来源：http://pog.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://dcy.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kjr.yongpay.top

[K02] JSON 字符串转对象
来源：http://iaw.sysykeji.top

Py:   json.loads(s)
来源：http://yqr.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eum.pycfn.com

JS:   JSON.parse(s)
来源：http://etj.0kj1m.cn

TS:   JSON.parse(s)
来源：http://hvw.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nut.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://uwb.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://pfg.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gfk.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://kfe.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pkb.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://izx.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oux.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://gox.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tgj.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pky.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jsr.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hdm.shuidangran.top

[K04] 读取 JSON 文件
来源：http://xlp.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fvw.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qlk.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rbn.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vkx.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ofg.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wzc.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gjj.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fci.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://dny.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://pix.hnqzz.top

PHP:  unserialize(serialize($obj));
来源：http://hvt.sysykeji.top

JS:   structuredClone(obj)
来源：http://pcs.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://sbv.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pik.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jwf.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iay.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fhe.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://zlx.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jbm.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gmn.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mns.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mdi.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://riq.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dro.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dyr.andypj.xyz


<!-- 参考信息 -->