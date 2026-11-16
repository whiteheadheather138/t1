代发 wailian999

[H03] 主动抛出异常
来源：http://hcv.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://rym.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lol.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://czd.tanke756.top

TS:   throw new Error("错误信息");
来源：http://ptv.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mer.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pel.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://khq.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://qqf.52xcode.cn

[H04] 自定义异常类型
来源：http://jkc.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://kdm.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://pnz.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://pjw.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://iif.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://qkl.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wdi.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://kit.cheryme.top

C#:   class MyException : Exception {}
来源：http://gir.zhoulong.xyz

[H05] 捕获特定类型
来源：http://cjc.cdnleiting.top

Py:   except ValueError as e:
来源：http://hjw.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ldc.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://xvz.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://bmm.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://ecy.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ebn.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://ptl.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zhp.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://iot.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://kgw.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://khr.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://lfz.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://zjj.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ugh.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lsp.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://unr.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://irz.cashguo.top

[H07] 断言
来源：http://mws.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://zkp.jyoumei.cn

PHP:  assert($x > 0);
来源：http://zcf.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://bia.uphjek.com

TS:   console.assert(x > 0);
来源：http://uvd.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://nha.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nyx.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pxa.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://lcw.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://znz.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://syk.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hfe.svipenyu.cn

JS:   e.message;  e.stack
来源：http://sfn.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://vcs.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pyd.zhixingplan.top

Go:   err.Error()
来源：http://yzf.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://bzm.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://tuw.zhongyouzk.top

[H09] 带错误码的异常
来源：http://ylf.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fdv.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://spe.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cps.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tud.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ldg.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qzl.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://mcj.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xny.jqgfzy.top

[H10] 资源自动释放
来源：http://sox.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zng.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ajs.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ona.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://edh.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fmi.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://wwx.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dlg.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rtn.xingfuxueyuan.xyz

================================================================================
来源：http://uhb.jinqigfzy.top

I. 正则表达式
来源：http://ise.sjlbkw.cn

================================================================================
来源：http://pdz.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://mbn.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nsk.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://plz.uphjek.com

JS:   /\d+/.test(s)
来源：http://gds.tian-w.cn

TS:   /\d+/.test(s)
来源：http://xtu.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vxy.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oge.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://swt.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xsi.ppjwa.cn

[I02] 提取所有匹配
来源：http://kob.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://fnj.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://joi.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jae.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://exm.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kzl.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://liz.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://cnb.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kzx.316326.xyz

[I03] 提取捕获分组
来源：http://edl.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://txl.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://quu.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lzy.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gbh.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aoc.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ynm.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uvq.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nbt.hesvh.cn

[I04] 正则替换
来源：http://duh.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rbz.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xxp.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fhv.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://ukd.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://ckg.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://awg.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://crt.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wcm.gaohongyu789.top

[I05] 按正则拆分
来源：http://wwi.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ulk.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://apr.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://blo.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://imf.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://cyx.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rtg.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://kev.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gmx.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://juq.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dpf.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fud.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xdx.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wmo.chenjidiqi.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bux.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mpj.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kug.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://phb.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://amk.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jcl.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aet.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nyj.ywan-chungtsiang.top

TS:   /error/gim
来源：http://qzb.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://smo.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jao.ivvv.top

Ruby: s.scan(/error/i)
来源：http://ccw.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nkc.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://tnk.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://skt.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hzr.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ivs.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://usv.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qhs.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://coj.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qhb.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rap.jianghu66.top

================================================================================
来源：http://uue.ywan-chungtsiang.top

J. 日期与时间
来源：http://whm.xingfuxueyuan.xyz

================================================================================
来源：http://lha.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://mbr.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://kdw.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rzf.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://rxu.yfazqb.com

TS:   new Date();  Date.now()
来源：http://pif.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bdy.cashguo.top

Go:   time.Now()
来源：http://riq.birdmap.top

Ruby: Time.now
来源：http://hfj.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zaq.yueranfly.top

[J02] 格式化输出
来源：http://nfh.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zwj.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uhu.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://guf.pengpengdd.cyou

TS:   d.toISOString()
来源：http://wpo.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wel.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nap.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bgn.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dzt.zdbjq.cn

[J03] 字符串解析为日期
来源：http://gkk.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xrk.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jaz.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://tbf.pycfn.com

TS:   new Date("2024-01-02")
来源：http://cyf.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://foq.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gqh.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://kvm.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fup.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://xwu.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gdm.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vzm.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jcb.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dzj.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gal.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qhw.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://acj.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vrx.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://vqg.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://civ.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yio.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjj.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kat.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://xnh.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://raa.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://nov.sufxvd.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iov.epnwcf.com

[J06] 计算两时间之差
来源：http://zbz.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://mrt.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://cgi.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rah.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://txf.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://skp.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://aik.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://nlb.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://eor.hcnkem.com

[J07] 比较两个日期
来源：http://khr.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://xvc.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fan.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://fpe.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://vmp.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://llt.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://orl.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://orf.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://ecd.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://xja.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qcw.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ilc.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cnk.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cqn.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dqg.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ztc.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dyh.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sci.yuanzhike.top

[J09] 时区处理
来源：http://eyv.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pck.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ota.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://azn.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdq.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hgi.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uep.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ozt.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nhl.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://bfo.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jul.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dwr.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vws.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eys.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tzp.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zar.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cjc.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lbo.ybcxt.top

================================================================================
来源：http://rmq.jianghu66.top

K. JSON 与序列化
来源：http://and.0kj1m.cn

================================================================================
来源：http://qrn.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://kur.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://owy.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hah.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://qem.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://yqt.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wab.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://oup.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://wyl.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://xqf.xylfe.cn

[K02] JSON 字符串转对象
来源：http://dfi.ybcxt.top

Py:   json.loads(s)
来源：http://lpn.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hsw.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://ooo.yvedp.cn

TS:   JSON.parse(s)
来源：http://bte.nanxuanxn.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hrl.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://qdd.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://sbn.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tto.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://zqn.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pud.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://osr.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://brn.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mur.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mha.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nlg.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://pem.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bsn.meibo888.top

[K04] 读取 JSON 文件
来源：http://czt.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jbe.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xta.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xcw.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://juz.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zmh.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wuu.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xlu.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dun.zhengqikj.top

[K05] 深拷贝对象
来源：http://age.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://sby.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://zms.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://hbe.yj20258.top

TS:   structuredClone(obj)
来源：http://yko.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://obt.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://njv.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cbd.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fey.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://yhp.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rbq.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aye.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://llo.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opp.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iem.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ijc.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lim.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zur.kuanghao11.cn

[K07] 进制转换
来源：http://sjm.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wsu.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://knf.yanxiufei.cn


<!-- 参考信息 -->