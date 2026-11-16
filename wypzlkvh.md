代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://tqm.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ttr.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://imt.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://psw.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sqp.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ern.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://hoj.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fgx.ctjpmb.com

[H03] 主动抛出异常
来源：http://evs.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://tls.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ufl.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://lph.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://hig.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nkp.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wmx.quarkkingdee.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pku.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jgh.mhx1999.top

[H04] 自定义异常类型
来源：http://ybr.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://rch.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://jya.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://skh.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://zrs.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://jdo.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uet.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://fog.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://dnj.yvedp.cn

[H05] 捕获特定类型
来源：http://dgj.fzhhl.top

Py:   except ValueError as e:
来源：http://rhm.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vvv.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://twc.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://mfl.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://kix.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mav.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://itn.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nvy.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://mtr.sxryk.cn

Py:   value = d.get("k") or default
来源：http://szz.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://mun.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://vsy.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://dpe.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aqe.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mpz.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://jir.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://jgm.zhixingplan.top

[H07] 断言
来源：http://eyn.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://lcq.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://ija.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://xih.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://qvm.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://nll.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bvb.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://beh.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://agj.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://smq.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://pbc.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yab.yuanzhike.top

JS:   e.message;  e.stack
来源：http://xxc.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qwo.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://joc.zhiwuduotai.top

Go:   err.Error()
来源：http://vvj.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://aum.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://qwa.gaohongyu789.top

[H09] 带错误码的异常
来源：http://rgo.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vme.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vxl.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://llv.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qhm.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://phs.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nbg.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://ifb.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fro.haohaochexian.top

[H10] 资源自动释放
来源：http://qas.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ujb.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pix.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qoo.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uln.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://opk.tian-w.cn

Go:   defer f.Close()
来源：http://sou.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wzb.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rvk.tanke756.top

================================================================================
来源：http://hlb.havefunace.top

I. 正则表达式
来源：http://qll.cqqwz.cn

================================================================================
来源：http://wbv.yj202588.top

[I01] 判断是否匹配
来源：http://pnk.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mdx.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xyh.hnqzz.top

JS:   /\d+/.test(s)
来源：http://yyw.vehdjk.com

TS:   /\d+/.test(s)
来源：http://vwn.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jsa.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mon.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://krw.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ckm.jlsjyb.cn

[I02] 提取所有匹配
来源：http://nwh.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://rfs.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rcq.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zns.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://koi.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cxo.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://got.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://uta.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kwd.fzhhl.top

[I03] 提取捕获分组
来源：http://fkx.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zcf.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oqq.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vlt.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uis.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://taa.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qzw.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yfp.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://syj.mhx1999.top

[I04] 正则替换
来源：http://skk.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kgf.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ydy.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://guu.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ppa.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rnc.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vmt.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qqs.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aho.jinqigfzy.top

[I05] 按正则拆分
来源：http://avv.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vuh.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wsk.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://llm.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://cvy.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://ihl.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cuz.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://iqe.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dwv.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iya.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qav.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rgl.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wgm.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dvc.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://srh.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kgc.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wjo.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tuq.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://vlg.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bvt.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rnd.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bmt.cheryme.top

TS:   /error/gim
来源：http://jjw.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://imc.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jym.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://did.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xxb.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://zaa.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iru.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nsz.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iqe.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://naj.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ick.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xmo.nanxinkj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yvs.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uer.jinghuilouyu.cn

================================================================================
来源：http://xes.ppjwa.cn

J. 日期与时间
来源：http://vjl.haohaochexian.top

================================================================================
来源：http://cwu.yueranfly.top

[J01] 获取当前时间
来源：http://fpi.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qjs.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lwh.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://rim.tanke756.top

TS:   new Date();  Date.now()
来源：http://oqc.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tfx.cdnleiting.top

Go:   time.Now()
来源：http://sbq.9152youxi.cn

Ruby: Time.now
来源：http://dwl.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nxn.chenjidiqi.icu

[J02] 格式化输出
来源：http://iah.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dug.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hoj.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lbn.shuidangran.top

TS:   d.toISOString()
来源：http://tcn.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bnb.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vxp.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lux.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://beu.yj20258.top

[J03] 字符串解析为日期
来源：http://uau.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wvi.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wig.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://rcu.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://uyv.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uke.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kng.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://xxh.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qay.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://srw.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://opc.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kwk.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ehg.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gba.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kco.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vth.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fkz.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iia.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://ykk.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://bpm.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zqd.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pff.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cex.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://hdb.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dpb.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://gmc.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://lcx.yvedp.cn

[J06] 计算两时间之差
来源：http://xxb.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://vle.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://ncu.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://twh.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wmw.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://rgc.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://lgv.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://kcj.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://ygc.shangyingyoupin.top

[J07] 比较两个日期
来源：http://qsj.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://xrr.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vwy.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://bda.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://tqo.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fyd.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rzm.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://vsk.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://onu.zycfv.cn

[J08] 提取年月日与星期
来源：http://zla.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jrr.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ccq.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hpj.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sbn.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tvm.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fsv.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zrg.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kta.jinqigufen.top

[J09] 时区处理
来源：http://kxb.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hny.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ubr.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zzf.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ewy.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pvf.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pzh.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://www.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pes.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://blb.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fct.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hqw.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qkt.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://utf.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cat.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ecp.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ddf.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bje.sweek.top

================================================================================
来源：http://qzt.hammf.cn

K. JSON 与序列化
来源：http://oii.hywenlv.cn

================================================================================
来源：http://npl.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://gfq.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hna.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ttg.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://upw.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://tqh.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ftt.birdmap.top

Go:   json.Marshal(obj)
来源：http://ccy.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vlj.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://odu.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://nnk.fengsongda.top

Py:   json.loads(s)
来源：http://rjx.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ehe.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://whk.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://uym.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mbd.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://tvq.fehbvm.com

Ruby: JSON.parse(s)
来源：http://fjm.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdq.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://jcm.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ndd.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jaf.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://vfs.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zqz.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tml.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pkf.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://bxu.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://amo.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://von.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vuf.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://elg.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ewc.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smi.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nlc.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yqo.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yfs.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://niz.yvedp.cn

[K05] 深拷贝对象
来源：http://hhk.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://fww.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://ooo.yuxming.cn

JS:   structuredClone(obj)
来源：http://xdc.meibo888.top

TS:   structuredClone(obj)
来源：http://thl.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vmw.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fkt.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eoc.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cly.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://hrz.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ktc.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://trx.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eat.xylfe.cn


<!-- 参考信息 -->