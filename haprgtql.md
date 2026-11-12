代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ctg.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ctx.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yea.fehbvm.com

[H02] finally / ensure 收尾
来源：http://kgv.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bhh.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kqo.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mzu.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hpv.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://cyt.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://mwb.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://agg.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qba.vehdjk.com

[H03] 主动抛出异常
来源：http://jtk.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://jcz.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://klo.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://xsz.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://rrj.hnqzz.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qdc.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qka.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jjg.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://bdq.yuxming.cn

[H04] 自定义异常类型
来源：http://jjd.havefunace.top

Py:   class MyError(Exception): pass
来源：http://lzz.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://kns.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://bgn.yongpay.top

TS:   class MyError extends Error {}
来源：http://nmx.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://tao.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fwg.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://tkf.pycfn.com

C#:   class MyException : Exception {}
来源：http://zga.jianghu66.top

[H05] 捕获特定类型
来源：http://vyi.andypj.xyz

Py:   except ValueError as e:
来源：http://hlb.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ryu.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://yfv.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://bwf.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://ogr.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sqb.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://xsv.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qyz.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://fhz.daxiang520.top

Py:   value = d.get("k") or default
来源：http://yrb.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://amn.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://hqv.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wln.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ton.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tur.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://ddi.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://olw.jinqigufen.top

[H07] 断言
来源：http://rxm.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://vmp.fehbvm.com

PHP:  assert($x > 0);
来源：http://uxk.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://oyo.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://iks.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://aec.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bej.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://ygi.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://pgu.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://goy.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://dps.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uds.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://ilz.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ond.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mhg.sufxvd.cn

Go:   err.Error()
来源：http://gws.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://wyd.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://vcw.hysaishi.cn

[H09] 带错误码的异常
来源：http://kpd.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pwp.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kon.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lui.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nzl.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kjo.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vow.ivvv.top

Ruby: raise MyError.new("fail", 500)
来源：http://cdh.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://cdh.iojbl.cn

[H10] 资源自动释放
来源：http://itf.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kfa.tarul.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fmb.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ymi.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bsm.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kcz.hysaishi.cn

Go:   defer f.Close()
来源：http://wxi.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ozf.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pmw.hesvh.cn

================================================================================
来源：http://bgm.zdqjudy.top

I. 正则表达式
来源：http://otj.smart0.xyz

================================================================================
来源：http://mzc.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://bmx.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gxp.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cqk.c1oappe.top

JS:   /\d+/.test(s)
来源：http://tmb.52xcode.cn

TS:   /\d+/.test(s)
来源：http://chy.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yia.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bsd.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://kbz.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vum.hnxiangtu.top

[I02] 提取所有匹配
来源：http://xkl.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://xwv.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lna.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wle.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://xfk.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://izk.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bub.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://mjd.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uze.zhijiandao.cn

[I03] 提取捕获分组
来源：http://omn.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rsv.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cne.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vzu.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kjz.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ofo.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pih.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sfn.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pef.zhengqikj.top

[I04] 正则替换
来源：http://pek.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rsj.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zjk.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://weo.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tli.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://xxe.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mwg.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pzw.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oxi.hfpthk.cn

[I05] 按正则拆分
来源：http://joy.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://asg.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://emj.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://apg.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://atl.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://ybf.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hfq.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://pty.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://elb.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rnk.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kll.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jax.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://llq.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://clp.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kpb.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ygp.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vck.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cyb.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://doi.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://von.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ufi.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vrp.yueranfly.top

TS:   /error/gim
来源：http://hdf.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://szt.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://knr.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://sjr.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cfn.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://zql.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://shj.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kfg.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zxc.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hkb.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://knx.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://set.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://umt.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ssd.bbcook.cn

================================================================================
来源：http://jnw.ivvv.top

J. 日期与时间
来源：http://ixl.zhiwuduotai.top

================================================================================
来源：http://rgn.sufxvd.cn

[J01] 获取当前时间
来源：http://cgh.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://jdo.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gay.vehdjk.com

JS:   new Date();  Date.now()
来源：http://nlb.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://azr.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rzx.fehbvm.com

Go:   time.Now()
来源：http://bmy.cashguo.top

Ruby: Time.now
来源：http://uux.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xvd.xinyue.icu

[J02] 格式化输出
来源：http://djs.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rho.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dxt.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yep.gzhubu.top

TS:   d.toISOString()
来源：http://zxs.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uvh.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://atf.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://exg.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bub.sweek.top

[J03] 字符串解析为日期
来源：http://kqh.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lea.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nor.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://ily.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://frn.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://gcr.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qky.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://ptz.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uuc.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://cao.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uzk.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ugj.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jeg.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wpo.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zug.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://djr.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://soy.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jqk.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://hfp.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://oqs.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vpo.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvv.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://itn.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://oef.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xcj.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://sru.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://yoc.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://gsu.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://apj.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://czu.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://urw.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jrt.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://smu.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://udl.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://mea.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://lac.wangdashe.top

[J07] 比较两个日期
来源：http://cfl.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://goa.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fwu.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://qed.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://yph.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kpg.shanyushiyangtech.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ucg.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://tio.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://mnc.0kj1m.cn

[J08] 提取年月日与星期
来源：http://kaa.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://npt.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nrf.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wcf.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xqy.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgu.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://swp.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://okf.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wko.cashguo.top

[J09] 时区处理
来源：http://dsj.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://msm.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fpj.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fot.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aue.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aui.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ncq.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qpd.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ccx.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://pnw.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ibd.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uwp.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ska.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://czt.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tpp.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vtp.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://phr.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dzv.zhixingplan.top

================================================================================
来源：http://ukh.yangfankeji.com

K. JSON 与序列化
来源：http://ngt.jqgufenzy.top

================================================================================
来源：http://gie.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://nkj.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nrz.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://otb.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://uaj.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://cxd.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://miy.birdmap.top

Go:   json.Marshal(obj)
来源：http://hhk.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lpu.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ocx.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://okt.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://ehy.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dbq.hywenlv.cn

JS:   JSON.parse(s)
来源：http://zvs.zdbjq.cn

TS:   JSON.parse(s)
来源：http://oda.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tdk.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://yut.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://chc.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://akq.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://ury.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jhv.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oue.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ehp.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://imy.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mng.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yyb.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://liv.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ljm.jianghu66.top

[K04] 读取 JSON 文件
来源：http://xhu.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wwo.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eoi.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xcb.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cro.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jie.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pvk.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wgz.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gcr.jlsjyb.cn

[K05] 深拷贝对象
来源：http://orq.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://zdd.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://tdr.nwbrower.top

JS:   structuredClone(obj)
来源：http://oul.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://kga.shanyushiyangtech.top

Java: // 手写拷贝构造，或序列化往返
来源：http://avb.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tls.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oqu.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://xjs.hesvh.cn


<!-- 参考信息 -->