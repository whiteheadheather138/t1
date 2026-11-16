代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://aje.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://luv.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://qpw.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zgq.jianghu66.top

[H03] 主动抛出异常
来源：http://wdw.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://nsl.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pjt.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://fww.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://tqi.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hsv.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xpy.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bwi.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://yia.shzxlz.cn

[H04] 自定义异常类型
来源：http://uss.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://ind.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://oal.daria6918.cn

JS:   class MyError extends Error {}
来源：http://jcb.sxryk.cn

TS:   class MyError extends Error {}
来源：http://fsw.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://ftn.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nje.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://eov.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://swn.fktsv.cn

[H05] 捕获特定类型
来源：http://fev.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://qzz.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gpd.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://uqn.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://ueg.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://iqd.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gog.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://anf.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qvn.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://tvd.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://pzz.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qtd.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://qoi.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sib.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iww.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kdh.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://fgf.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://xiq.zhongyouzk.top

[H07] 断言
来源：http://cfp.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://hxr.yonumen.top

PHP:  assert($x > 0);
来源：http://igx.yvedp.cn

JS:   console.assert(x > 0);
来源：http://flw.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://gjl.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://jmn.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fcg.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://zpk.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://btf.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://gkf.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://haq.gaohongyu789.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iqs.xylfe.cn

JS:   e.message;  e.stack
来源：http://ucn.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wwj.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://anw.hnxiangtu.top

Go:   err.Error()
来源：http://bqp.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://dqp.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://ctl.9152youxi.cn

[H09] 带错误码的异常
来源：http://uoa.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rcf.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pgw.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sth.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fcv.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lyj.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://njf.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dhq.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://czd.wangdashe.top

[H10] 资源自动释放
来源：http://jjo.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://nvv.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vay.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fho.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uaq.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pgh.epnwcf.com

Go:   defer f.Close()
来源：http://hqr.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mbp.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kxc.sysykeji.top

================================================================================
来源：http://nxn.hysaishi.cn

I. 正则表达式
来源：http://pny.tianlin.xyz

================================================================================
来源：http://mst.redwolf501.top

[I01] 判断是否匹配
来源：http://yhd.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ojl.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://uer.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://pde.fengsongda.top

TS:   /\d+/.test(s)
来源：http://kim.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mwu.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ujv.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://xsw.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kxh.ybcxt.top

[I02] 提取所有匹配
来源：http://cep.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://inb.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iew.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ywe.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://xis.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ukm.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://foa.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://wdx.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kgz.xziqi.cn

[I03] 提取捕获分组
来源：http://fvr.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mcw.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fpj.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jwy.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iuq.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cyu.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://coh.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ele.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ukm.jinyuanbaomall.cn

[I04] 正则替换
来源：http://xjv.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lyd.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xdi.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://taw.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://gvy.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://stc.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://buh.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vti.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vtk.svipenyu.cn

[I05] 按正则拆分
来源：http://amc.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://hlk.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nrr.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://pez.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://fwf.shuidangran.top

Java: s.split("\\s*,\\s*")
来源：http://dtv.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pmk.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://zky.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://adv.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wez.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uzl.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bqr.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xev.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ocm.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dcn.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eot.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dwj.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsr.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://htp.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pab.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mii.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lzg.fehbvm.com

TS:   /error/gim
来源：http://iiy.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://egn.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://got.sweek.top

Ruby: s.scan(/error/i)
来源：http://nrr.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rtq.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://vla.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wjy.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rrq.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wgc.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cls.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dfr.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mpo.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cae.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://omu.52xcode.cn

================================================================================
来源：http://zdw.xuanzx.com

J. 日期与时间
来源：http://qar.gogol.net.cn

================================================================================
来源：http://oax.jyoumei.cn

[J01] 获取当前时间
来源：http://tux.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xqa.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bwy.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://ijy.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://tlt.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qmi.9152youxi.cn

Go:   time.Now()
来源：http://cth.yonumen.top

Ruby: Time.now
来源：http://udp.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://twb.chenlongwang.top

[J02] 格式化输出
来源：http://drp.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hpl.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://znp.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ayi.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://qfz.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fpg.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xph.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nhb.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iot.ppjwa.cn

[J03] 字符串解析为日期
来源：http://zwf.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zrr.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jin.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://mxr.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://psa.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://gcj.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zfz.fanxiaobao.xyz

Ruby: Date.parse("2024-01-02")
来源：http://wdh.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uyg.daria6918.cn

[J04] 时间戳与日期互转
来源：http://lim.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kjb.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eue.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bbc.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dvz.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xiq.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yhv.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://agv.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://anm.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://psl.tanke756.top

Py:   now + timedelta(days=7)
来源：http://qqd.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://htb.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://czo.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqi.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://mtx.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ylg.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://cdf.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://ktv.hfpthk.cn

[J06] 计算两时间之差
来源：http://oij.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://bbe.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://ldd.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://scu.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hra.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mbl.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://tep.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://rck.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://wcc.quarkkingdee.top

[J07] 比较两个日期
来源：http://mnb.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://gge.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xjy.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://iuj.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://cjw.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xus.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vcr.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://vvu.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://iww.redwolf501.top

[J08] 提取年月日与星期
来源：http://llz.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lhg.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://evm.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dbc.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iao.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://grj.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vkj.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://crn.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ifv.tian-w.cn

[J09] 时区处理
来源：http://pku.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rln.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ibe.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://utd.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hnu.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lgw.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oew.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ufl.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qbt.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://tcd.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://etu.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ifo.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sfm.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bzw.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qpw.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dll.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lxm.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yre.hcnkem.com

================================================================================
来源：http://cru.aibaodan.cn

K. JSON 与序列化
来源：http://krh.yj20258.top

================================================================================
来源：http://oad.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://ctn.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oap.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qcg.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://gyx.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://peg.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://try.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://ozc.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://qrw.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://syo.c1oappe.top

[K02] JSON 字符串转对象
来源：http://xaa.fzhhl.top

Py:   json.loads(s)
来源：http://cpl.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://azp.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://njv.smart0.xyz

TS:   JSON.parse(s)
来源：http://ukx.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ikj.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://fst.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://boe.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nab.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://ygh.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ggy.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cwf.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rji.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fif.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nwp.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lxn.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://hwe.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yxy.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://wge.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xdj.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yzr.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tpj.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rrd.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sau.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://stj.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rtm.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://azy.cqqwz.cn

[K05] 深拷贝对象
来源：http://jmn.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://vql.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://alf.shzxlz.cn

JS:   structuredClone(obj)
来源：http://cpq.xuanzx.com

TS:   structuredClone(obj)
来源：http://jjh.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rtu.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ckv.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tbn.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mrg.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://dbb.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yok.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dvo.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vyy.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rir.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vks.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fkv.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rzy.fengsongda.top


<!-- 参考信息 -->