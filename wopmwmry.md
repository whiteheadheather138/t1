代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://oza.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wnk.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fmh.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hvr.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pru.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qln.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oub.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://yxw.hcnkem.com

[H03] 主动抛出异常
来源：http://wde.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://ewa.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xjl.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://dxm.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://nex.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://haq.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zer.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ewz.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dnk.yvedp.cn

[H04] 自定义异常类型
来源：http://ubc.cheryme.top

Py:   class MyError(Exception): pass
来源：http://usd.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://kfh.vehdjk.com

JS:   class MyError extends Error {}
来源：http://jhh.tian-w.cn

TS:   class MyError extends Error {}
来源：http://ymu.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://kjb.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pfz.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://hvz.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://lph.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://hng.quarkkingdee.top

Py:   except ValueError as e:
来源：http://gqd.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lrf.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://liw.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://mfl.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://nuz.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oaa.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://lte.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nnj.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://xbk.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://krz.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://can.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://uiw.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mjb.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rth.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iip.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://zkm.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://mml.sxryk.cn

[H07] 断言
来源：http://rgg.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://vre.cdnleiting.top

PHP:  assert($x > 0);
来源：http://fqx.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://vgb.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://tha.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://pnf.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iyr.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://oad.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://uzj.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://ltb.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://fic.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://apb.ctjpmb.com

JS:   e.message;  e.stack
来源：http://imw.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cmc.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vle.ppjwa.cn

Go:   err.Error()
来源：http://wmn.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://rqm.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://brt.ivvv.top

[H09] 带错误码的异常
来源：http://drp.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mkk.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uua.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yth.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mwj.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qfs.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ulj.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://nef.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eeg.shzxlz.cn

[H10] 资源自动释放
来源：http://yub.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vei.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xou.ivvv.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wql.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mri.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bmq.zhixingplan.top

Go:   defer f.Close()
来源：http://kih.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lmy.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jsd.wangdashe.top

================================================================================
来源：http://ccs.andypj.xyz

I. 正则表达式
来源：http://dqt.cdnleiting.top

================================================================================
来源：http://ssm.chenlongwang.top

[I01] 判断是否匹配
来源：http://vrm.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kdy.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://wpl.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://jfe.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://mue.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fzi.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://omo.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://tld.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dhq.ydjk.org.cn

[I02] 提取所有匹配
来源：http://wjf.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://fmz.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dsc.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yut.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://big.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hfk.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jug.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://hyz.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oba.jinqigfzy.top

[I03] 提取捕获分组
来源：http://jwq.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lvn.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://odl.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nzs.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aug.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cvd.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://irp.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kes.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jir.fehbvm.com

[I04] 正则替换
来源：http://xkj.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sck.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kvk.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://llf.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mqj.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bud.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bvq.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xpx.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nyb.cashguo.top

[I05] 按正则拆分
来源：http://ayp.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ubn.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mis.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://zti.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://eis.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://qxo.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://frk.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://jhv.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tkw.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hxe.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://new.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cwq.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://way.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hgb.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hir.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ida.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ntc.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fvu.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://mpu.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ggm.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fsj.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ejm.uphjek.com

TS:   /error/gim
来源：http://xis.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dfi.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mdd.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://oya.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lgj.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://mfs.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tab.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rjt.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lqj.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lkk.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://bzb.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ccq.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lrm.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xgh.9152youxi.cn

================================================================================
来源：http://txa.hongshengwenyu.top

J. 日期与时间
来源：http://lnr.yvedp.cn

================================================================================
来源：http://tuf.jiagoushi.top

[J01] 获取当前时间
来源：http://esh.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eua.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ltn.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://nyg.redwolf501.top

TS:   new Date();  Date.now()
来源：http://lzq.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pam.haohaochexian.top

Go:   time.Now()
来源：http://twb.tian-w.cn

Ruby: Time.now
来源：http://qqf.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ehy.xuanzx.com

[J02] 格式化输出
来源：http://hks.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jti.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gbq.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vgg.chenlongwang.top

TS:   d.toISOString()
来源：http://xbx.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qfi.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zpx.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://llj.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qlf.cashguo.top

[J03] 字符串解析为日期
来源：http://xag.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tlm.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ivr.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://vme.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://nbg.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://uxs.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wfs.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://zah.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfh.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://kof.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xld.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iaq.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rnn.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hky.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gmo.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rom.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nam.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iix.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://igk.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://jtj.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://plw.52xcode.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bqd.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lxf.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://qvv.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hkg.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://hys.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hsl.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://vyb.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://ijd.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://zah.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lwx.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nvj.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://msi.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://elz.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://elq.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://mwe.ppjwa.cn

[J07] 比较两个日期
来源：http://riq.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://cnr.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bdw.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://msi.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jwk.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cwh.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jgj.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://klg.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://twd.yongpay.top

[J08] 提取年月日与星期
来源：http://idb.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nig.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://txy.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bll.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aid.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qdt.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bhr.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iva.yueranfly.top

[J09] 时区处理
来源：http://xql.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mmp.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cie.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nak.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dkl.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cpd.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uon.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pui.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qkt.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://lfj.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hgh.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rmh.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://atm.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zza.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jbz.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://unu.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pwp.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mcj.pengpengdd.cyou

================================================================================
来源：http://prr.haohaochexian.top

K. JSON 与序列化
来源：http://wwz.fktsv.cn

================================================================================
来源：http://pct.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://mus.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iln.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ohl.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://dnm.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://vxw.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nbj.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://wgn.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oas.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pyw.tarul.cn

[K02] JSON 字符串转对象
来源：http://ogy.c1oappe.top

Py:   json.loads(s)
来源：http://mpu.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gkw.fktsv.cn

JS:   JSON.parse(s)
来源：http://ymb.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://dqi.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sij.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://pyc.fktsv.cn

Ruby: JSON.parse(s)
来源：http://gyt.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hnd.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://epu.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zji.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ihd.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://key.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wbx.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://osv.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xpc.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tkp.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ihj.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://ypr.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://anr.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blk.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pye.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzo.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jgs.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hok.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sqk.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rxl.c1oappe.top

[K05] 深拷贝对象
来源：http://asn.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://cya.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://uhd.c1oappe.top

JS:   structuredClone(obj)
来源：http://mwz.jinyuanbaomall.cn

TS:   structuredClone(obj)
来源：http://rqu.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ont.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xqe.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ncd.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xny.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://wcc.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tjp.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://htx.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmy.dianchejie.cn


<!-- 参考信息 -->