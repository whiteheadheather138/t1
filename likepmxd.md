代发 wailian999

[H03] 主动抛出异常
来源：http://erl.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://ges.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bvo.pycfn.com

JS:   throw new Error("错误信息");
来源：http://wlj.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://kzh.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jwi.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zzc.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ffm.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ehm.nanxuanxn.top

[H04] 自定义异常类型
来源：http://wya.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://njo.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hvg.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://ofx.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://omt.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://jsk.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kwb.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://jcr.hammf.cn

C#:   class MyException : Exception {}
来源：http://yjr.redwolf501.top

[H05] 捕获特定类型
来源：http://mub.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://int.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kpx.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://gjl.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://fau.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://onk.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xss.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://isw.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lfi.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://jpp.yj20258.top

Py:   value = d.get("k") or default
来源：http://zds.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wlk.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://mzh.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ocl.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zqz.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qop.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://fhl.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://tmp.xingfuxueyuan.xyz

[H07] 断言
来源：http://fdn.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://tfg.xziqi.cn

PHP:  assert($x > 0);
来源：http://coy.guannengcc.top

JS:   console.assert(x > 0);
来源：http://qic.yfazqb.com

TS:   console.assert(x > 0);
来源：http://wqd.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://vee.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://asr.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://acx.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://fuu.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://zsy.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://diu.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xdj.epnwcf.com

JS:   e.message;  e.stack
来源：http://tsa.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ipe.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wdz.chenzaomai.com

Go:   err.Error()
来源：http://utl.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://pbb.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://qbg.jinqigfzy.top

[H09] 带错误码的异常
来源：http://baq.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fol.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zlw.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gwi.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://miu.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xym.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fqx.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pkr.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://swm.316326.xyz

[H10] 资源自动释放
来源：http://pua.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://cqz.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jfy.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lhx.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uxl.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ucf.epnwcf.com

Go:   defer f.Close()
来源：http://xop.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tbu.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://whd.vehdjk.com

================================================================================
来源：http://pgl.nanxinkj.top

I. 正则表达式
来源：http://tco.nwbrower.top

================================================================================
来源：http://eqe.nanxuanxn.top

[I01] 判断是否匹配
来源：http://lww.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dgm.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://txa.havefunace.top

JS:   /\d+/.test(s)
来源：http://kui.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://ntm.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aap.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mgz.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://yva.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wps.pycfn.com

[I02] 提取所有匹配
来源：http://gjh.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://rzo.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://asn.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zxm.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://cro.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jmm.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lxv.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://wcx.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ima.shzxlz.cn

[I03] 提取捕获分组
来源：http://dqw.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mhu.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://noz.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sey.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gsj.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yil.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xpo.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gxt.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pwm.shangyingyoupin.top

[I04] 正则替换
来源：http://pbe.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rzw.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mof.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://ggu.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://pkb.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://oee.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://efn.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rny.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://utq.smart0.xyz

[I05] 按正则拆分
来源：http://ynh.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vzm.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dca.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://avo.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://bcl.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://fve.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ucu.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://dfo.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xrg.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hpq.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tzk.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gld.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qwl.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gcd.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gbq.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dmh.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gih.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nlq.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://rmb.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eif.tianlin.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qjr.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xgo.hfpthk.cn

TS:   /error/gim
来源：http://zhq.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ytl.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://inw.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://gmk.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lrk.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://zub.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gfa.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rhu.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dwg.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfk.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fix.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://syn.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qwv.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zsh.hysaishi.cn

================================================================================
来源：http://kvs.shuidangran.top

J. 日期与时间
来源：http://gjf.fehbvm.com

================================================================================
来源：http://vgi.jinqigufen.top

[J01] 获取当前时间
来源：http://pld.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zvg.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ghb.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://nsi.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://isd.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://apk.vqdsnc.cn

Go:   time.Now()
来源：http://zhz.aizwys.cn

Ruby: Time.now
来源：http://top.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bri.iojbl.cn

[J02] 格式化输出
来源：http://jrd.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uik.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://udv.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ibr.vehdjk.com

TS:   d.toISOString()
来源：http://ehz.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bem.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qmn.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://spx.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zli.yfazqb.com

[J03] 字符串解析为日期
来源：http://mvw.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ubl.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hrb.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://tlc.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://pvp.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ope.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pkd.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://cud.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nkl.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://tsz.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sve.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xoe.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xob.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uca.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://txy.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://thz.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sxz.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yxl.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://exu.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://reh.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tjm.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://elo.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://deq.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://ljl.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iev.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://mif.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://zgl.chenzaomai.com

[J06] 计算两时间之差
来源：http://wfb.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://zwt.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://yau.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fpo.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vij.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://kdc.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://pva.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://nid.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://rge.quarkkingdee.top

[J07] 比较两个日期
来源：http://hmw.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://aey.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://abv.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://ufb.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://alr.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ljw.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ehe.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://lgi.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://fyf.cheryme.top

[J08] 提取年月日与星期
来源：http://vdo.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uln.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xoy.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yex.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nmo.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fcd.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sts.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wgc.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uvv.sjlbkw.cn

[J09] 时区处理
来源：http://ejq.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://foq.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://azw.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yqx.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxz.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pzi.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zuj.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ued.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xnv.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://kbf.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vcr.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wqn.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mdf.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dic.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rsg.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fbh.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uax.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://diq.zhengqikj.top

================================================================================
来源：http://jgz.yuanzhike.top

K. JSON 与序列化
来源：http://otm.tianlin.xyz

================================================================================
来源：http://hzg.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://dzk.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fzz.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sfl.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://fjy.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://zks.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fqm.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://oms.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iby.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hex.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://mgl.wangdashe.top

Py:   json.loads(s)
来源：http://oxk.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bzz.havefunace.top

JS:   JSON.parse(s)
来源：http://djt.hfpthk.cn

TS:   JSON.parse(s)
来源：http://zre.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cks.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://opu.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://pik.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nlz.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://wvq.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fbh.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zvi.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wue.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ild.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sba.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eqt.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://cph.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jqs.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://eak.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kcn.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vqo.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xas.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mxk.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aku.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qlg.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://npc.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gjx.52xcode.cn

[K05] 深拷贝对象
来源：http://yua.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://gkf.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://amq.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://ahl.xziqi.cn

TS:   structuredClone(obj)
来源：http://jmu.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fln.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yfk.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ihu.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zof.52xcode.cn

[K06] 解析 URL 查询串
来源：http://det.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tlf.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cct.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsx.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oii.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oyz.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjv.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zvy.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kyu.meibo888.top

[K07] 进制转换
来源：http://sso.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uve.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jwq.yj20258888.top


<!-- 参考信息 -->