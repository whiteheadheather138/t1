代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://gaf.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://bhd.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iwk.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lhy.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mpa.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zlk.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://phq.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://yzn.vqdsnc.cn

[H03] 主动抛出异常
来源：http://emq.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://rxq.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://isk.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://nev.meibo888.top

TS:   throw new Error("错误信息");
来源：http://vgm.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://icc.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tzn.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lwy.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://eol.cashguo.top

[H04] 自定义异常类型
来源：http://xqb.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://fgq.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://vsf.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://lyj.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://rzy.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://mrr.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rmd.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://hlo.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://ubd.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://cgm.aizwys.cn

Py:   except ValueError as e:
来源：http://oxd.xuanzx.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://irl.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ipd.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://hfs.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://jod.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lqm.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://vep.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zkh.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://pea.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://dnf.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://nat.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://dif.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hzl.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rdu.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://svg.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://bwc.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://pen.hongshengwenyu.top

[H07] 断言
来源：http://ouy.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://kix.hnqzz.top

PHP:  assert($x > 0);
来源：http://lzj.jinyuanbaomall.cn

JS:   console.assert(x > 0);
来源：http://pqf.daria6918.cn

TS:   console.assert(x > 0);
来源：http://mry.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://mva.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nnn.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vtd.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://jvj.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://awg.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://dev.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://icz.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://brk.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tid.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ovj.jqgufenzy.top

Go:   err.Error()
来源：http://paz.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://vsw.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://uab.fzhhl.top

[H09] 带错误码的异常
来源：http://xkg.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://axo.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdx.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gxu.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://thp.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hko.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uvu.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fhd.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dtj.tianlin.xyz

[H10] 资源自动释放
来源：http://dks.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fnj.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yzt.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zsj.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kxg.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qtv.cucudq.cn

Go:   defer f.Close()
来源：http://mxq.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uew.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gfm.andypj.xyz

================================================================================
来源：http://roc.fengsongda.top

I. 正则表达式
来源：http://tpf.shuidangran.top

================================================================================
来源：http://dex.svipenyu.cn

[I01] 判断是否匹配
来源：http://ahv.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mcc.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://iqp.sxryk.cn

JS:   /\d+/.test(s)
来源：http://pgl.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://hdu.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qfb.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://veh.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://tte.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qgd.havefunace.top

[I02] 提取所有匹配
来源：http://pfu.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://kbd.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cwp.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rhp.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://zrh.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://esz.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vbc.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://hib.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bzn.c1oappe.top

[I03] 提取捕获分组
来源：http://pul.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bxv.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vrp.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hyf.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fou.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qmn.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nni.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fdv.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ytk.vehdjk.com

[I04] 正则替换
来源：http://iwq.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yhs.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://njd.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://vwl.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kdm.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://fvf.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jac.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rac.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ytc.yanxiufei.cn

[I05] 按正则拆分
来源：http://avt.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://edy.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qvw.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://fsi.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://txz.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://cfv.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zyd.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://dnq.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fnx.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hft.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ymt.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xya.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rwc.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iri.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fbo.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kko.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://exy.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://drb.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://ykf.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://djk.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yxe.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pbr.fehbvm.com

TS:   /error/gim
来源：http://ros.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kud.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eoo.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://vpk.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nrz.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://vfm.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xhb.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sln.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pyy.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vqm.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://thc.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bjr.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qfn.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bkh.sufxvd.cn

================================================================================
来源：http://odm.zhijiandao.cn

J. 日期与时间
来源：http://iug.hcnkem.com

================================================================================
来源：http://jfv.zdbjq.cn

[J01] 获取当前时间
来源：http://chj.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://uia.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wld.gzhubu.top

JS:   new Date();  Date.now()
来源：http://qhz.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://eog.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://skt.nwbrower.top

Go:   time.Now()
来源：http://cwi.zhixingplan.top

Ruby: Time.now
来源：http://dej.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gyg.ctjpmb.com

[J02] 格式化输出
来源：http://yzq.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zcs.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qkt.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://skf.ydzc1.top

TS:   d.toISOString()
来源：http://mgb.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://goj.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yxy.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqu.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gnq.zdbjq.cn

[J03] 字符串解析为日期
来源：http://yhj.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sxj.yonumen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gtd.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://cmu.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://jqi.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://osa.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pnv.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://php.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jhq.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://xfq.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tcd.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iei.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zlx.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://vrf.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://puk.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nvl.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xym.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qja.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://dvj.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://gnj.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nms.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qhz.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vnp.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://loa.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hcs.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://cry.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://glg.vehdjk.com

[J06] 计算两时间之差
来源：http://ieo.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://smy.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://zmq.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vxk.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nko.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://guv.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://ucv.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://dgo.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://uvh.cashguo.top

[J07] 比较两个日期
来源：http://tmh.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://ejb.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ptp.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://quh.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://som.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://arg.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zhc.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vke.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://xmy.yj202588.top

[J08] 提取年月日与星期
来源：http://wtx.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ful.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qyq.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dco.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gfh.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qyj.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://znn.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tps.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pmp.yvedp.cn

[J09] 时区处理
来源：http://kbn.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oem.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qod.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vta.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzq.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eht.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pql.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gyn.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mgh.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://jip.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ctq.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gnx.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tux.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dnd.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qxo.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://inl.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://syg.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fll.gaohongyu789.top

================================================================================
来源：http://kbz.vehdjk.com

K. JSON 与序列化
来源：http://qvl.yj20258888.top

================================================================================
来源：http://anv.jinqigufen.top

[K01] 对象转 JSON 字符串
来源：http://mto.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kfv.jiagoushi.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jmw.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://tig.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://mdn.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qpc.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://tde.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://ozi.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zhf.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://awj.yfazqb.com

Py:   json.loads(s)
来源：http://coo.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bky.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://zwp.fktsv.cn

TS:   JSON.parse(s)
来源：http://ngq.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dat.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://fkv.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://ets.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aat.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://qjk.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iae.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jod.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ueo.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hzp.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://erg.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xmt.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sqg.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://alk.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://rbq.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dbp.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cpj.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qdn.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vpt.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jfr.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dsm.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wha.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rty.uphjek.com

[K05] 深拷贝对象
来源：http://yoo.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://cbl.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://cva.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://how.ivvv.top

TS:   structuredClone(obj)
来源：http://edd.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://upj.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vwc.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hxq.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gej.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://rwl.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kpx.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aqn.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwu.yanxiufei.cn


<!-- 参考信息 -->