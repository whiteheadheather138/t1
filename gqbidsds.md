代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://fcy.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gzo.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sbd.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bnv.nanxuanxn.top

[H03] 主动抛出异常
来源：http://cfi.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://chn.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hju.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://vcr.meibo888.top

TS:   throw new Error("错误信息");
来源：http://dbo.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qou.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uai.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mhr.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://lks.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://wpo.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://bcu.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ypn.havefunace.top

JS:   class MyError extends Error {}
来源：http://lxv.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://xzp.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://mtw.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://avl.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://ztp.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://kka.zdbjq.cn

[H05] 捕获特定类型
来源：http://nbn.zdqjudy.top

Py:   except ValueError as e:
来源：http://hes.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qcm.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://dnp.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://xwv.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://yly.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pnp.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://lgn.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gim.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://oes.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://iyx.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gkx.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://boa.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://nds.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://log.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yua.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://sgd.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://ryw.sysykeji.top

[H07] 断言
来源：http://zgv.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://myy.nwbrower.top

PHP:  assert($x > 0);
来源：http://pso.mhx1999.top

JS:   console.assert(x > 0);
来源：http://vto.epnwcf.com

TS:   console.assert(x > 0);
来源：http://pnq.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://gaz.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jni.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://bwx.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://jrs.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://tcr.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://onh.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fjh.daria6918.cn

JS:   e.message;  e.stack
来源：http://lcz.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hsm.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://clf.iojbl.cn

Go:   err.Error()
来源：http://xhi.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://rvj.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://eqg.svipenyu.cn

[H09] 带错误码的异常
来源：http://mnj.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kau.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kjr.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tgh.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zzj.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://saa.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://guy.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://afw.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dcb.wangshuangyany.cn

[H10] 资源自动释放
来源：http://wut.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xqb.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jms.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://klz.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fse.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pdu.wangshuangyany.cn

Go:   defer f.Close()
来源：http://wrw.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://scm.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://evm.9152youxi.cn

================================================================================
来源：http://rqq.yangfankeji.com

I. 正则表达式
来源：http://tcs.zdqjudy.top

================================================================================
来源：http://wmh.guannengcc.top

[I01] 判断是否匹配
来源：http://mwt.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ujc.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://vtr.hammf.cn

JS:   /\d+/.test(s)
来源：http://xlu.cashguo.top

TS:   /\d+/.test(s)
来源：http://jon.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qmd.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zqo.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://kyy.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uuu.shzxlz.cn

[I02] 提取所有匹配
来源：http://fol.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://tha.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fdj.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fce.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://mhw.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://grr.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jzs.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://fft.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qkz.nanxuanxn.top

[I03] 提取捕获分组
来源：http://dbx.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fbq.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://krm.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://non.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qje.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rjc.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gba.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gib.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mei.jinqigufen.top

[I04] 正则替换
来源：http://jfx.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hvx.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gkc.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://fde.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://qdv.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dsa.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wyy.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vkz.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jgh.feifeiyinyue.top

[I05] 按正则拆分
来源：http://jfy.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://cuv.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tdp.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://guk.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://iom.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://zom.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nse.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://zmx.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dnm.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://frt.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xmo.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ngs.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xtg.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xpl.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zaa.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xqn.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dud.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mbd.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://mjs.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vjv.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kgb.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://spq.52xcode.cn

TS:   /error/gim
来源：http://kmk.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kpx.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ziq.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://oqs.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kym.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://mrk.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://whm.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sji.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://btv.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://unz.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nda.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vzz.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wpg.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bpo.chenzaomai.com

================================================================================
来源：http://rqz.hesvh.cn

J. 日期与时间
来源：http://wur.chenjidiqi.icu

================================================================================
来源：http://uya.cdnleiting.top

[J01] 获取当前时间
来源：http://vrw.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lqw.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yqy.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://cdu.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://isx.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qvc.ydzc1.top

Go:   time.Now()
来源：http://gxp.guannengcc.top

Ruby: Time.now
来源：http://mla.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qfg.hesvh.cn

[J02] 格式化输出
来源：http://pbv.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ewb.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rbk.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rqw.xziqi.cn

TS:   d.toISOString()
来源：http://rwg.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zaw.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ssc.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lko.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hoa.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://rpd.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hbc.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zne.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://utp.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://grw.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://ele.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zik.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://tod.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hco.guannengcc.top

[J04] 时间戳与日期互转
来源：http://lco.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://clu.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://htp.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cuk.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gsl.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fmb.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lan.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pyy.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ofm.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://krz.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://acx.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pgq.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kug.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://liu.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://jmu.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yjr.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://gpy.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://spr.sysykeji.top

[J06] 计算两时间之差
来源：http://dqu.havefunace.top

Py:   (end - start).total_seconds()
来源：http://iot.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://fxw.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rwm.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://noi.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://obl.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://ehx.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://vog.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://fbd.vqdsnc.cn

[J07] 比较两个日期
来源：http://vfq.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://htv.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jqa.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bkv.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tkb.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fop.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aoy.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zvx.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://ptt.zdbjq.cn

[J08] 提取年月日与星期
来源：http://xns.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://goq.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tum.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lbz.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iuu.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wfd.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pws.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mnm.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://boe.tianlin.xyz

[J09] 时区处理
来源：http://mlm.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qzh.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cyh.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvp.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cmu.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://riq.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aeo.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yol.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nby.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://igv.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ztc.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ghj.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hxm.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qeg.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://chw.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yzo.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iqv.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ytu.yonumen.top

================================================================================
来源：http://rrs.yanxiufei.cn

K. JSON 与序列化
来源：http://elg.52xcode.cn

================================================================================
来源：http://rtc.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://rbq.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sqp.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cvs.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://gwi.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://tpd.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lms.guannengcc.top

Go:   json.Marshal(obj)
来源：http://aea.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://gxj.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ppo.iojbl.cn

[K02] JSON 字符串转对象
来源：http://fxg.ehwqpu.com

Py:   json.loads(s)
来源：http://ddm.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://apj.52xcode.cn

JS:   JSON.parse(s)
来源：http://dbr.jianghu66.top

TS:   JSON.parse(s)
来源：http://vld.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pif.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://jqj.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://epx.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://btn.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://nao.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://joc.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dwt.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ggi.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lzm.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lus.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zmm.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://bsi.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://klb.yj20258888.top

[K04] 读取 JSON 文件
来源：http://ble.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fjc.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nat.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tuh.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mdk.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xuf.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rcz.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbh.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qeh.bjfxy.top

[K05] 深拷贝对象
来源：http://kcs.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://phd.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://wag.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://zgv.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://ygi.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://peu.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bct.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://egp.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rsk.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://fmf.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wis.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nfl.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fal.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbp.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mmo.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sqk.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gzw.kuanghao11.cn


<!-- 参考信息 -->