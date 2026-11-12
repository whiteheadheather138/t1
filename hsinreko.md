代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://mmc.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://snb.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pvd.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bat.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fwa.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://teq.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://swp.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lko.gaohongyu789.top

[H03] 主动抛出异常
来源：http://mvm.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://ame.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uns.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://kcy.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://lin.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://nrp.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rkt.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://mup.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://llu.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://axc.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://hbw.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://jyd.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://enx.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://crx.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://xkk.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nwr.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://joo.yueranfly.top

C#:   class MyException : Exception {}
来源：http://who.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://cis.kuanghao11.cn

Py:   except ValueError as e:
来源：http://xri.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wbn.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://omt.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://uot.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://gbw.hywenlv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mjn.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://sir.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xgi.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://ijj.iojbl.cn

Py:   value = d.get("k") or default
来源：http://tso.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://zyd.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://gwo.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eeg.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://shq.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ioa.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://xvk.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://jlg.cqqwz.cn

[H07] 断言
来源：http://saw.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://bby.daria6918.cn

PHP:  assert($x > 0);
来源：http://yqw.tian-w.cn

JS:   console.assert(x > 0);
来源：http://mno.pycfn.com

TS:   console.assert(x > 0);
来源：http://eci.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://lvn.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qpo.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://pls.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://rta.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://zwh.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://cje.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xpt.hesvh.cn

JS:   e.message;  e.stack
来源：http://gxm.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://sen.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://fuu.gotoacloud.top

Go:   err.Error()
来源：http://hpj.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://mjw.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://thr.tarul.cn

[H09] 带错误码的异常
来源：http://mqu.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yqt.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lub.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mlt.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ikm.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fjk.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yih.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hes.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wnh.epnwcf.com

[H10] 资源自动释放
来源：http://zvz.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://oju.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aom.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sqq.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uft.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qag.feifeiyinyue.top

Go:   defer f.Close()
来源：http://yqa.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gen.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wow.sweek.top

================================================================================
来源：http://xze.zhiwuduotai.top

I. 正则表达式
来源：http://rkd.chenzaomai.com

================================================================================
来源：http://str.fengsongda.top

[I01] 判断是否匹配
来源：http://hcg.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pvh.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dik.iojbl.cn

JS:   /\d+/.test(s)
来源：http://ngs.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://qlr.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eay.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://odf.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://vew.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://siz.ppjwa.cn

[I02] 提取所有匹配
来源：http://pvp.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://nac.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fer.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://khu.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://ird.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ayf.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yyl.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://nud.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cza.vqdsnc.cn

[I03] 提取捕获分组
来源：http://ddb.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uzu.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hjr.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tpo.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ovq.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sas.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://frv.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://swo.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vwi.hywenlv.cn

[I04] 正则替换
来源：http://vum.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fzq.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yaw.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://byk.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nta.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://fog.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nre.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cbj.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lrv.yj20258888.top

[I05] 按正则拆分
来源：http://ksn.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mfd.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bqx.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://qie.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://vsd.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://lug.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qmv.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://axb.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dic.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tau.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ckm.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mza.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ind.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oqt.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pcs.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jyq.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sju.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tkw.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://umx.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sdu.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yws.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ypf.andypj.xyz

TS:   /error/gim
来源：http://vtl.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dmx.jinyuanbaomall.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vxs.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://wcw.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://htn.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://lrj.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qwe.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wlc.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pga.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vuj.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fyk.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bqy.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xrq.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://coh.cheryme.top

================================================================================
来源：http://yro.cucudq.cn

J. 日期与时间
来源：http://avv.gzhubu.top

================================================================================
来源：http://upa.zhongyouzk.top

[J01] 获取当前时间
来源：http://rvy.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vkh.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lsz.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://ris.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://vhk.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yab.yvedp.cn

Go:   time.Now()
来源：http://due.ivvv.top

Ruby: Time.now
来源：http://pju.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pip.smart0.xyz

[J02] 格式化输出
来源：http://hgj.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tld.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ctc.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://exj.hnxiangtu.top

TS:   d.toISOString()
来源：http://caq.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://omc.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oue.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ibx.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wqd.sxryk.cn

[J03] 字符串解析为日期
来源：http://szh.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://urm.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vmf.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://wjz.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://xfr.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xmc.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://exa.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://rai.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://thv.guannengcc.top

[J04] 时间戳与日期互转
来源：http://qpx.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gkw.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uom.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://icl.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bwc.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sek.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lqh.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jal.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ivh.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://sgm.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://cmp.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://sde.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vff.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkf.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://uhj.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uzb.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://bzv.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://giu.fehbvm.com

[J06] 计算两时间之差
来源：http://cea.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://acz.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://jav.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wbb.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ctb.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rrt.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://ice.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://kgr.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://glj.birdmap.top

[J07] 比较两个日期
来源：http://wev.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://lsf.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yqe.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://crl.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://wxn.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://olk.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mef.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jgl.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://rcd.sxryk.cn

[J08] 提取年月日与星期
来源：http://qfq.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zdw.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vbf.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nkz.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dzv.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mys.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oss.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rzh.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uyr.cheryme.top

[J09] 时区处理
来源：http://ppr.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://njh.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://daz.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://plj.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adv.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tqg.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nnl.daria6918.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://njt.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mos.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://ptx.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lqf.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jax.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pei.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://afy.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wiq.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qns.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://awx.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xkv.yj202588.top

================================================================================
来源：http://mzi.yangfankeji.com

K. JSON 与序列化
来源：http://vme.hnqzz.top

================================================================================
来源：http://kws.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://fni.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rud.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pni.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://mcv.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://dtb.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pdm.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://qia.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rgn.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gfy.ybcxt.top

[K02] JSON 字符串转对象
来源：http://zhc.chenlongwang.top

Py:   json.loads(s)
来源：http://eny.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cia.dashuyun.cn

JS:   JSON.parse(s)
来源：http://gbd.nwbrower.top

TS:   JSON.parse(s)
来源：http://bzv.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wty.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://ctq.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://ltj.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jox.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://hqr.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qdy.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xtj.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://lvp.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://sev.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dng.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fdp.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zmn.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nbq.uphjek.com

[K04] 读取 JSON 文件
来源：http://sdf.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qqz.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lzr.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tbi.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nzn.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jvm.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mfq.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zxw.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nxf.aibaodan.cn

[K05] 深拷贝对象
来源：http://quh.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://bji.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://nmn.chenzaomai.com

JS:   structuredClone(obj)
来源：http://wvm.tian-w.cn

TS:   structuredClone(obj)
来源：http://fro.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tlo.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dpv.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vcj.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ppo.yongpay.top

[K06] 解析 URL 查询串
来源：http://toq.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xmq.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lqo.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ojq.shangyingyoupin.top


<!-- 参考信息 -->