代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hue.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://syl.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rme.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tow.ybcxt.top

[H03] 主动抛出异常
来源：http://acc.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://ikk.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qoe.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://ktb.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://ctw.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://kls.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cqr.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mok.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://nrc.ivvv.top

[H04] 自定义异常类型
来源：http://acq.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://xok.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://nep.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://ist.andypj.xyz

TS:   class MyError extends Error {}
来源：http://cih.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://rhv.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bhd.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://zdc.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://ldq.316326.xyz

[H05] 捕获特定类型
来源：http://aes.chenlongwang.top

Py:   except ValueError as e:
来源：http://btf.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zef.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://kja.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://jax.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://qcj.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://npd.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://afy.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bwh.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://kyp.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://eak.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ufc.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://poy.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://duh.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fry.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://fme.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://zuy.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://jkn.316326.xyz

[H07] 断言
来源：http://vpc.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://lvk.zhixingplan.top

PHP:  assert($x > 0);
来源：http://frb.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://rin.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://ghw.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://mmj.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vup.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://abz.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://lmo.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://svp.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://xew.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://efz.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://hou.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ecc.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dwb.redwolf501.top

Go:   err.Error()
来源：http://tko.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://qpf.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://alj.0kj1m.cn

[H09] 带错误码的异常
来源：http://mge.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gno.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xnn.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ixp.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://icg.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nae.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vfe.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://izs.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dna.daxiang520.top

[H10] 资源自动释放
来源：http://vma.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://evy.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://udp.birdmap.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qvx.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rsf.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://agw.zdbjq.cn

Go:   defer f.Close()
来源：http://udq.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kee.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hrv.svipenyu.cn

================================================================================
来源：http://zxe.yonumen.top

I. 正则表达式
来源：http://puh.yj20258.top

================================================================================
来源：http://enp.gotoacloud.top

[I01] 判断是否匹配
来源：http://qbp.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qra.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wba.yangfankeji.com

JS:   /\d+/.test(s)
来源：http://jcg.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://mwh.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gia.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://szn.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://hpa.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://npg.quarkkingdee.top

[I02] 提取所有匹配
来源：http://fcj.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://gsn.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fvh.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://far.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://khl.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ove.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pfb.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://gge.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vpf.uphjek.com

[I03] 提取捕获分组
来源：http://ztj.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pam.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qta.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kvb.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cpk.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rkh.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://omr.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lfv.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://obv.shangyingyoupin.top

[I04] 正则替换
来源：http://qmo.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://bhr.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ulb.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://syb.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://imu.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://hra.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://qjh.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hpd.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dng.sweek.top

[I05] 按正则拆分
来源：http://jdy.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xlt.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://asp.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://gtn.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://zjq.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://qlf.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://frk.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://kgn.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qzj.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rny.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hzs.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yqw.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rvv.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://goq.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rok.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wiu.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sln.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qhf.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://opc.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yib.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jeu.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tag.hysaishi.cn

TS:   /error/gim
来源：http://dag.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ctt.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uzv.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://kbk.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tzd.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://cqx.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tdy.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mre.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oor.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ysq.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yva.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vzd.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lpd.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zqz.hnqzz.top

================================================================================
来源：http://mdb.sysykeji.top

J. 日期与时间
来源：http://zbu.hfpthk.cn

================================================================================
来源：http://uyn.chenzaomai.com

[J01] 获取当前时间
来源：http://crf.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jsz.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dxr.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://uaq.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://dug.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qmy.yvedp.cn

Go:   time.Now()
来源：http://dkn.aizwys.cn

Ruby: Time.now
来源：http://vnk.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ugb.hnxiangtu.top

[J02] 格式化输出
来源：http://vus.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ded.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yac.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hiv.hfpthk.cn

TS:   d.toISOString()
来源：http://meo.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gav.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lpb.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://epg.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://txm.aizwys.cn

[J03] 字符串解析为日期
来源：http://mib.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tpj.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ifp.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://exc.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://fll.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://mga.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nvq.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://qqh.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jzd.shuidangran.top

[J04] 时间戳与日期互转
来源：http://qfd.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mps.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://paa.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fgx.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://fvu.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eos.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rvs.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uyn.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://knq.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://gef.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://igt.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dif.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://elc.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ocx.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://etv.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hrx.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://sul.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://oyi.tianlin.xyz

[J06] 计算两时间之差
来源：http://hwv.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://xyk.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://tkd.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qwo.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hwz.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://oow.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://rrn.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://msm.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://cbp.ppjwa.cn

[J07] 比较两个日期
来源：http://ofs.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://kbh.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aeb.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zat.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jbn.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://clq.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zbq.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://tgx.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://wzk.cashguo.top

[J08] 提取年月日与星期
来源：http://rxt.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yah.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hon.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rgd.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qhc.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cnh.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qot.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zpq.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tue.redwolf501.top

[J09] 时区处理
来源：http://hxi.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vfq.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://whh.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wex.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://buh.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xht.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uxa.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://isi.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ffq.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://adr.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ujj.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mng.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xfj.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://swa.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tcz.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vcf.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vgl.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yci.tanke756.top

================================================================================
来源：http://vfc.shuidangran.top

K. JSON 与序列化
来源：http://oby.ivvv.top

================================================================================
来源：http://exg.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://yxv.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kcd.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmn.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://eep.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://fgz.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iqe.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://ufi.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rrx.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://yyl.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://vit.xylfe.cn

Py:   json.loads(s)
来源：http://ykb.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://scx.nwbrower.top

JS:   JSON.parse(s)
来源：http://lgm.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://okm.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jue.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://xob.epnwcf.com

Ruby: JSON.parse(s)
来源：http://cnt.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fes.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://glk.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tcf.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cwn.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rig.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xxr.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ljj.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgl.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://ixe.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tip.yuxming.cn

[K04] 读取 JSON 文件
来源：http://psh.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pys.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rfo.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ytk.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cch.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rqp.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bna.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ago.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bdu.ydjk.org.cn

[K05] 深拷贝对象
来源：http://kkp.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://ysr.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://iox.xuanzx.com

JS:   structuredClone(obj)
来源：http://suf.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://rps.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://akf.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ngd.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ehk.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vty.hesvh.cn

[K06] 解析 URL 查询串
来源：http://xiq.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tbv.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hxw.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oez.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pll.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vah.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bjz.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://igd.yonumen.top


<!-- 参考信息 -->