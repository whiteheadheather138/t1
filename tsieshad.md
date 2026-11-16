代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://gib.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://xvf.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gep.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://gvf.fengsongda.top

[H03] 主动抛出异常
来源：http://wxf.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://hho.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zto.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://iza.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://oie.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tvt.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fab.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uye.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hnf.chenzaomai.com

[H04] 自定义异常类型
来源：http://tzp.cashguo.top

Py:   class MyError(Exception): pass
来源：http://ceh.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://pfc.fehbvm.com

JS:   class MyError extends Error {}
来源：http://ond.sweek.top

TS:   class MyError extends Error {}
来源：http://xrb.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://vyh.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jix.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://upq.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://fmh.hesvh.cn

[H05] 捕获特定类型
来源：http://ilx.hesvh.cn

Py:   except ValueError as e:
来源：http://gzm.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gob.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://wwt.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://frz.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://oku.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ovs.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://byv.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bft.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://qqz.sweek.top

Py:   value = d.get("k") or default
来源：http://eja.cucudq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ufd.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://aor.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://pui.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lrh.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://avm.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://zds.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://dkn.yuxming.cn

[H07] 断言
来源：http://vmo.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://kmv.cashguo.top

PHP:  assert($x > 0);
来源：http://eqn.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://apo.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://hpk.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://tzp.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jpx.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ufw.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://guo.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://qjd.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://agj.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uah.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://jln.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wqp.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vuc.yfazqb.com

Go:   err.Error()
来源：http://hjz.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://bmy.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://yao.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://fol.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://itz.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ola.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mkt.0kj1m.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zdv.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qfm.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uge.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hom.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://uiz.fzhhl.top

[H10] 资源自动释放
来源：http://moi.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ljn.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rcc.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bej.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vxm.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uhb.tian-w.cn

Go:   defer f.Close()
来源：http://usq.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qng.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jrz.chenjidiqi.icu

================================================================================
来源：http://lxm.xinyue.icu

I. 正则表达式
来源：http://fot.jyoumei.cn

================================================================================
来源：http://rrx.sjlbkw.cn

[I01] 判断是否匹配
来源：http://jjc.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cjm.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vdk.hammf.cn

JS:   /\d+/.test(s)
来源：http://nab.hcnkem.com

TS:   /\d+/.test(s)
来源：http://jzl.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hek.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fij.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://oqu.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zcj.yongpay.top

[I02] 提取所有匹配
来源：http://env.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://dch.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yye.aibaodan.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aiz.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://qup.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pni.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oip.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://iql.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uyw.9152youxi.cn

[I03] 提取捕获分组
来源：http://fvy.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rjy.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vpb.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://soj.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fht.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yud.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bsf.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://def.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://piu.bbcook.cn

[I04] 正则替换
来源：http://gef.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://alq.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ibx.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://jdt.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lss.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://dvu.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://fft.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://epr.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ufl.kuanghao11.cn

[I05] 按正则拆分
来源：http://vgp.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eyq.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ibi.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://emn.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://vyo.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://wnl.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ysg.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://yke.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ema.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ifb.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zwk.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ezm.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ics.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://deq.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tiq.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://agw.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wxb.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qnh.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://kbz.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xtl.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dzu.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nut.zhongyouzk.top

TS:   /error/gim
来源：http://rfb.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fbx.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://epf.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://wmj.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://edx.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://bog.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jxl.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ezz.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://adp.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtj.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hbk.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hei.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://avp.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ogs.andypj.xyz

================================================================================
来源：http://nhp.zycfv.cn

J. 日期与时间
来源：http://lmq.chenzaomai.com

================================================================================
来源：http://uus.gotoacloud.top

[J01] 获取当前时间
来源：http://qak.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xel.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aiy.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://gtr.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://cyh.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://egq.gzhubu.top

Go:   time.Now()
来源：http://nhw.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://joj.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iht.shanyushiyangtech.top

[J02] 格式化输出
来源：http://oxo.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yol.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eui.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://icr.xuanzx.com

TS:   d.toISOString()
来源：http://zzl.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hoy.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hvi.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://byu.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zxh.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://mlf.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rvl.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zdh.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://jih.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://mjh.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://zhf.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tvs.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://fdc.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kqu.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://kwq.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cvc.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bzf.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iha.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://pca.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qyv.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hbc.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://udy.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hbg.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://xhz.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://bqc.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mrq.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://udf.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vki.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://ekg.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gtu.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://ahr.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://mla.yj202588.top

[J06] 计算两时间之差
来源：http://vet.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://ayv.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://ljr.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iqk.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://emq.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://fhz.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://xqt.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://yvh.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://dqg.aizwys.cn

[J07] 比较两个日期
来源：http://oxf.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://efc.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jjk.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://gdt.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://cei.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jsc.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bus.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yfs.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://gmr.zhengqikj.top

[J08] 提取年月日与星期
来源：http://lnt.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xwx.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lhh.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vht.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://azy.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://leh.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yjc.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rbg.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wxy.ivvv.top

[J09] 时区处理
来源：http://mrd.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://luq.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xgt.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xpm.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eax.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qgd.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vwj.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sou.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cze.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://iha.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dys.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fdo.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jzd.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yeu.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qvt.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://anb.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://abs.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nyv.52xcode.cn

================================================================================
来源：http://sya.wangshuangyany.cn

K. JSON 与序列化
来源：http://dtb.wangshuangyany.cn

================================================================================
来源：http://gnd.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://hco.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ytt.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hlz.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://vig.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://tar.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ege.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://rks.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://dqh.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mly.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://aar.dianchejie.cn

Py:   json.loads(s)
来源：http://vqt.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hxn.cucudq.cn

JS:   JSON.parse(s)
来源：http://vba.uphjek.com

TS:   JSON.parse(s)
来源：http://ydn.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://srb.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://bcg.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://bou.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://thc.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://zjk.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hac.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bqc.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ylg.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lnb.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xpz.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gyw.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://fbn.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hsi.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://yew.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cnq.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ufi.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cgm.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://spk.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mdu.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kps.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jkp.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mqw.fengsongda.top

[K05] 深拷贝对象
来源：http://ufk.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://fqj.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://clm.dashuyun.cn

JS:   structuredClone(obj)
来源：http://fhb.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://cwb.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://anr.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rea.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lrb.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://zhi.havefunace.top

[K06] 解析 URL 查询串
来源：http://dlq.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vrb.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qch.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://efz.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://enq.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nlm.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://phr.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cat.yonumen.top


<!-- 参考信息 -->