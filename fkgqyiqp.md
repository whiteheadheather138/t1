代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://bhm.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sje.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hkl.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pqk.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://xjx.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://fsw.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fay.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xbd.jinqigfzy.top

[H03] 主动抛出异常
来源：http://kdx.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://dhj.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gsl.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://zha.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://odr.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dcd.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jid.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://lqz.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://tqk.tarul.cn

[H04] 自定义异常类型
来源：http://uid.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://xpl.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aac.pycfn.com

JS:   class MyError extends Error {}
来源：http://pxq.daria6918.cn

TS:   class MyError extends Error {}
来源：http://ols.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://ecg.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://phr.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://fif.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://yyq.bbcook.cn

[H05] 捕获特定类型
来源：http://dro.redwolf501.top

Py:   except ValueError as e:
来源：http://sff.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://few.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://nji.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://kgb.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://dbw.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vou.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://dfw.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zby.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://onj.xylfe.cn

Py:   value = d.get("k") or default
来源：http://jpi.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://hot.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://rll.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lvq.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kkz.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vbn.yanxiufei.cn

Ruby: d&.dig(:a, :b)
来源：http://wqv.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://zmw.zycfv.cn

[H07] 断言
来源：http://rxe.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://glk.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://msz.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://qoa.sxryk.cn

TS:   console.assert(x > 0);
来源：http://hsr.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://zyw.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tgw.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://cec.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://lsx.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://poz.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://gxs.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ujm.gotoacloud.top

JS:   e.message;  e.stack
来源：http://exp.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ldf.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pnf.shangyingyoupin.top

Go:   err.Error()
来源：http://ybr.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://keb.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://gkc.cheryme.top

[H09] 带错误码的异常
来源：http://qiz.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tqa.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lqd.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://paf.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zrh.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vho.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iov.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://acm.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tay.vqdsnc.cn

[H10] 资源自动释放
来源：http://rzq.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zyo.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dvw.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ocm.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://owq.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gur.sxryk.cn

Go:   defer f.Close()
来源：http://pcy.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xsv.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://whs.xuanzx.com

================================================================================
来源：http://ylf.jinqigufen.top

I. 正则表达式
来源：http://zvz.andypj.xyz

================================================================================
来源：http://vcl.ppjwa.cn

[I01] 判断是否匹配
来源：http://dxk.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://whw.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://osw.wangdashe.top

JS:   /\d+/.test(s)
来源：http://wgp.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://lie.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pde.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cfn.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://azw.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://exo.xuanzx.com

[I02] 提取所有匹配
来源：http://owo.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://djv.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://poo.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gdl.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://agm.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wxm.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dvt.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://asl.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cjy.52xcode.cn

[I03] 提取捕获分组
来源：http://ptk.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qyo.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mnt.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xno.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cvt.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uds.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bas.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fgi.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://woa.fengsongda.top

[I04] 正则替换
来源：http://xlm.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xah.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ohf.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://lon.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://cgh.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://hux.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://bcb.chenzaomai.com

Ruby: s.gsub(/\d+/, "#")
来源：http://zsn.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tfk.hongshengwenyu.top

[I05] 按正则拆分
来源：http://unx.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kzx.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://edd.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://pzd.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://tpz.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://szy.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mrz.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fno.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sds.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gog.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wyj.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yzw.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbo.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jxo.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://syc.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zcz.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jfm.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kwp.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://ysr.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://taf.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lxr.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://upc.gotoacloud.top

TS:   /error/gim
来源：http://utm.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ewt.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ffw.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://mkp.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ccp.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://sgq.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dhy.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sqq.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://spd.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nyx.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fnk.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pye.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ref.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ukq.andypj.xyz

================================================================================
来源：http://ohc.jianghu66.top

J. 日期与时间
来源：http://nnf.zhaomingkeji.xyz

================================================================================
来源：http://vvg.bbcook.cn

[J01] 获取当前时间
来源：http://jqn.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://erc.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hdu.hesvh.cn

JS:   new Date();  Date.now()
来源：http://tbb.fktsv.cn

TS:   new Date();  Date.now()
来源：http://viu.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://fzr.birdmap.top

Go:   time.Now()
来源：http://nru.smart0.xyz

Ruby: Time.now
来源：http://hsw.chenlongwang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vqv.yvedp.cn

[J02] 格式化输出
来源：http://oul.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uns.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iya.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://omt.yangfankeji.com

TS:   d.toISOString()
来源：http://kds.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dvb.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://luu.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dto.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://evw.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://geg.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://arg.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://itw.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://bgw.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://kbv.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rrj.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ywd.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ovw.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bma.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://xhl.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ntf.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nll.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jtt.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tkt.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://egb.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wik.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ocm.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pdu.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://rfp.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://ats.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://duf.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdx.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kuz.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ahv.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxr.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://plh.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://lpg.ppjwa.cn

[J06] 计算两时间之差
来源：http://hqp.hammf.cn

Py:   (end - start).total_seconds()
来源：http://dyx.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://dwc.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ztp.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hxc.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wva.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://fdm.yongpay.top

Ruby: end - start                 # 返回秒数
来源：http://noa.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://yqv.cashguo.top

[J07] 比较两个日期
来源：http://kpl.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wxa.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ozq.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://ygb.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://xtr.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pfr.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vfl.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yov.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://foq.sysykeji.top

[J08] 提取年月日与星期
来源：http://jmm.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ojm.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qqo.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xtk.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gsv.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eat.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wul.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xzu.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://abb.dashuyun.cn

[J09] 时区处理
来源：http://idh.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://joi.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mvo.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ytw.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dja.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iub.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://clc.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://onn.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uok.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://dyd.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://aqp.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yif.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://abn.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://biq.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zrp.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pok.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xow.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ath.pycfn.com

================================================================================
来源：http://vpu.jinghuilouyu.cn

K. JSON 与序列化
来源：http://nlt.tanke756.top

================================================================================
来源：http://uzk.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://lcp.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qok.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qqk.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://msg.yj202588.top

TS:   JSON.stringify(obj)
来源：http://vjn.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ygt.pycfn.com

Go:   json.Marshal(obj)
来源：http://zbf.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://wex.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ifq.pycfn.com

[K02] JSON 字符串转对象
来源：http://abc.sysykeji.top

Py:   json.loads(s)
来源：http://ivo.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mkt.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://lsz.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://ord.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hnd.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://jrp.gzhubu.top

Ruby: JSON.parse(s)
来源：http://uur.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wws.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://bxi.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kni.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uyz.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hbn.hesvh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jms.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hjd.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://edw.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://csd.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ouz.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://ctw.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uum.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wlf.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pdq.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bxv.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ghs.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://esi.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qdu.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oku.yueranfly.top

[K05] 深拷贝对象
来源：http://rhh.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://tas.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://xbl.bjfxy.top

JS:   structuredClone(obj)
来源：http://dkr.dashuyun.cn

TS:   structuredClone(obj)
来源：http://ujm.shanyushiyangtech.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xxv.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lkb.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fbu.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dpr.sxryk.cn

[K06] 解析 URL 查询串
来源：http://sen.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uvr.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tja.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxi.xziqi.cn


<!-- 参考信息 -->