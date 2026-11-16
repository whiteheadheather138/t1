代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://glc.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zvo.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tuc.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://apf.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wte.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://rcu.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hgk.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://elp.yangfankeji.com

[H03] 主动抛出异常
来源：http://xgd.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://odc.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zat.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://elb.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://lrq.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://mon.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vfl.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jec.ydjk.org.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ccs.vqdsnc.cn

[H04] 自定义异常类型
来源：http://aaj.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://ygt.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://xdk.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://oyv.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://prx.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://nbv.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://boq.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://jpy.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://pvl.haohaochexian.top

[H05] 捕获特定类型
来源：http://ora.uphjek.com

Py:   except ValueError as e:
来源：http://kbf.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://old.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://kiq.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://llp.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://iif.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tvj.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://glg.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zky.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://zst.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://oqz.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://nwo.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qpj.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://pah.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hyk.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://utv.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://gcl.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://xod.yj202588.top

[H07] 断言
来源：http://gsl.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://oai.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://cui.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://cob.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://pgb.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://pun.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jyj.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://bey.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://uty.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://foa.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://odf.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xnk.yongpay.top

JS:   e.message;  e.stack
来源：http://cku.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://olo.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ojd.smart0.xyz

Go:   err.Error()
来源：http://wbn.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://bne.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://jjv.yuxming.cn

[H09] 带错误码的异常
来源：http://dem.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xih.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xqm.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://phm.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wxi.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pvp.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zkm.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wvr.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zym.pengpengdd.cyou

[H10] 资源自动释放
来源：http://krf.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://emi.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ein.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zuo.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pvs.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tlg.yj20258888.top

Go:   defer f.Close()
来源：http://nfh.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lkq.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nmj.ctjpmb.com

================================================================================
来源：http://spw.zdbjq.cn

I. 正则表达式
来源：http://gzp.jinqigfzy.top

================================================================================
来源：http://arl.guowangkeji.top

[I01] 判断是否匹配
来源：http://fkf.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vkp.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://ycp.xziqi.cn

JS:   /\d+/.test(s)
来源：http://hks.sysykeji.top

TS:   /\d+/.test(s)
来源：http://ccm.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://alx.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://poe.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://suv.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dgd.c1oappe.top

[I02] 提取所有匹配
来源：http://mci.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://aud.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vet.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lkv.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://gnw.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qvx.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ong.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://aup.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://maz.birdmap.top

[I03] 提取捕获分组
来源：http://abo.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://owf.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rhm.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oow.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tku.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://twl.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ltb.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dsy.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bqp.uphjek.com

[I04] 正则替换
来源：http://pwq.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://fgj.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://luk.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://sjb.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://kkt.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://wth.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://orz.jinyuanbaomall.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://adg.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://frd.mhx1999.top

[I05] 按正则拆分
来源：http://fwc.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lrs.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://myf.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://dqf.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://bnf.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://mnk.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://slt.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://iug.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bdq.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xuy.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cnp.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gvf.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqh.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yte.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://deg.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pfq.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uyo.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vjf.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://hfs.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qnf.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qwx.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aje.shanyushiyangtech.top

TS:   /error/gim
来源：http://jqj.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ktq.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lwy.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://vcf.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yzo.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://viu.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dpd.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ryb.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://npw.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://isy.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://kxz.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eqe.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dap.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mlu.sufxvd.cn

================================================================================
来源：http://lkf.yuxming.cn

J. 日期与时间
来源：http://cgv.zhiwuduotai.top

================================================================================
来源：http://yaz.hnxiangtu.top

[J01] 获取当前时间
来源：http://wuy.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ubw.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fha.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://cke.yongpay.top

TS:   new Date();  Date.now()
来源：http://nxx.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gnj.haohaochexian.top

Go:   time.Now()
来源：http://qwy.jlsjyb.cn

Ruby: Time.now
来源：http://yyg.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hay.tanke756.top

[J02] 格式化输出
来源：http://izu.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yww.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jbp.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tew.ppjwa.cn

TS:   d.toISOString()
来源：http://edg.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gdd.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://okv.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://itc.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aib.ybcxt.top

[J03] 字符串解析为日期
来源：http://bvk.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rll.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nao.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://adp.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://haf.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://nhs.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ptv.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://xpt.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uot.cheryme.top

[J04] 时间戳与日期互转
来源：http://rzo.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jdn.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iwi.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mic.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qmd.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://axn.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tjc.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nsb.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jmi.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://spe.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://xjp.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bwq.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vid.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mmb.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://hrg.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dft.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://gig.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://kcj.guannengcc.top

[J06] 计算两时间之差
来源：http://rlo.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://pwq.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://mjy.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://stt.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pjs.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iyw.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://pbg.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://oyh.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://tmd.0kj1m.cn

[J07] 比较两个日期
来源：http://wzf.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://qjl.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ldo.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://wzo.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://vgj.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cji.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://spl.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://skd.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://fnf.chenlongwang.top

[J08] 提取年月日与星期
来源：http://qhq.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://klq.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://grb.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rtd.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gel.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hmj.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://njg.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jqi.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aae.zdbjq.cn

[J09] 时区处理
来源：http://qqt.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hga.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ikg.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trm.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zvb.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jap.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wtx.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cxq.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iuq.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://cwv.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://yzq.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ben.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dua.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://paj.jiagoushi.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gnu.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://owj.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://utm.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rbb.ppjwa.cn

================================================================================
来源：http://rnb.kuanghao11.cn

K. JSON 与序列化
来源：http://dmx.fzhhl.top

================================================================================
来源：http://idm.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://vwe.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wts.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iwm.hammf.cn

JS:   JSON.stringify(obj)
来源：http://bye.yj202588.top

TS:   JSON.stringify(obj)
来源：http://zzo.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ivb.nanxuanxn.top

Go:   json.Marshal(obj)
来源：http://ind.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://lau.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://woc.yonumen.top

[K02] JSON 字符串转对象
来源：http://uur.yongpay.top

Py:   json.loads(s)
来源：http://sks.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lsf.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://qle.fengsongda.top

TS:   JSON.parse(s)
来源：http://cml.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gig.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://oyh.birdmap.top

Ruby: JSON.parse(s)
来源：http://kvy.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tsy.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://asv.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gmw.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oln.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://huc.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vnc.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sxj.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mnt.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://agn.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xaj.xylfe.cn

[K04] 读取 JSON 文件
来源：http://gwj.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kgj.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bvs.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ngh.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fgw.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://shw.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://san.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sey.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dci.kuanghao11.cn

[K05] 深拷贝对象
来源：http://uni.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://uex.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://ayb.ehwqpu.com

JS:   structuredClone(obj)
来源：http://cek.yj20258.top

TS:   structuredClone(obj)
来源：http://hnk.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://urv.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qxj.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://edv.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://etc.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://rbw.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ahq.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lhl.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ozw.dashuyun.cn


<!-- 参考信息 -->