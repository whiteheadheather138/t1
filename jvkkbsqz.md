代发 wailian999

[H03] 主动抛出异常
来源：http://aiu.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://qko.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://grc.sweek.top

JS:   throw new Error("错误信息");
来源：http://icz.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://hbd.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wbq.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mgs.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bbe.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://ebn.yj20258888.top

[H04] 自定义异常类型
来源：http://trv.pycfn.com

Py:   class MyError(Exception): pass
来源：http://oxr.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://roq.meibo888.top

JS:   class MyError extends Error {}
来源：http://tql.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://iab.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://pxv.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mzm.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://oyh.bjfxy.top

C#:   class MyException : Exception {}
来源：http://pjt.hnqzz.top

[H05] 捕获特定类型
来源：http://wnt.jyoumei.cn

Py:   except ValueError as e:
来源：http://ded.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://riv.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://wpd.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://mfk.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://xbh.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pis.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://eiv.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sqa.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://foy.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://loq.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://owr.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://ikg.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ycj.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xio.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://jxd.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://rtc.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://gli.gotoacloud.top

[H07] 断言
来源：http://rpi.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://fob.svipenyu.cn

PHP:  assert($x > 0);
来源：http://wow.aizwys.cn

JS:   console.assert(x > 0);
来源：http://ztu.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://cjd.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://zmr.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xjr.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://poc.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://rmp.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://baa.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://oif.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xnk.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://bud.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://owm.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oni.nwbrower.top

Go:   err.Error()
来源：http://ixq.sweek.top

Ruby: e.message;  e.backtrace
来源：http://uei.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://lhc.aizwys.cn

[H09] 带错误码的异常
来源：http://ews.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aae.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dwc.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dsn.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mvn.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cif.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xjx.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ore.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hni.cdnleiting.top

[H10] 资源自动释放
来源：http://ase.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rhi.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jjw.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bjm.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kci.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vlf.sjlbkw.cn

Go:   defer f.Close()
来源：http://hcb.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fpq.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qws.xuetiantiany.cn

================================================================================
来源：http://nin.ivvv.top

I. 正则表达式
来源：http://cqi.svipenyu.cn

================================================================================
来源：http://fct.ivvv.top

[I01] 判断是否匹配
来源：http://luq.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fyn.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://ekp.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://fns.tanke756.top

TS:   /\d+/.test(s)
来源：http://zyq.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://psq.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://joe.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://xds.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dye.guannengcc.top

[I02] 提取所有匹配
来源：http://fwv.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://eyo.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ihg.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gpb.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://fgt.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ynz.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://veo.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://yul.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qfs.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://tpp.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fns.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zyy.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mhl.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xgs.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://drs.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ywz.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hkf.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uvv.jyoumei.cn

[I04] 正则替换
来源：http://bnp.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hql.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uxu.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://tpp.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hpc.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ivb.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ill.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pqx.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tlc.yangfankeji.com

[I05] 按正则拆分
来源：http://iop.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ets.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://upu.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://fyd.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://lcj.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://fly.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jwo.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kik.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jbk.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kns.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nyt.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ntg.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rpe.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xct.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lzs.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vwr.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cwx.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://itv.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://rwh.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nge.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://duv.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ufd.hongshengwenyu.top

TS:   /error/gim
来源：http://slq.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aro.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qcx.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://fol.xylfe.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://piu.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://qgv.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jxu.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://erv.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jus.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ztl.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uau.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ael.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fsf.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zpo.shanyushiyangtech.top

================================================================================
来源：http://she.xziqi.cn

J. 日期与时间
来源：http://ugy.svipenyu.cn

================================================================================
来源：http://nrb.hongshengwenyu.top

[J01] 获取当前时间
来源：http://sid.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aaz.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cgl.hammf.cn

JS:   new Date();  Date.now()
来源：http://agw.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://aoc.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cfj.zhongyouzk.top

Go:   time.Now()
来源：http://ikl.hongshengwenyu.top

Ruby: Time.now
来源：http://tbr.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lui.chenjidiqi.icu

[J02] 格式化输出
来源：http://vmg.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hot.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://suy.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sab.ppjwa.cn

TS:   d.toISOString()
来源：http://vri.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lvt.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qsn.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://onx.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zoa.hesvh.cn

[J03] 字符串解析为日期
来源：http://kmc.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uxp.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nzm.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://vbo.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://rfj.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://jgr.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cri.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://xky.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rzx.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://wgp.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wdb.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://prf.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lqa.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jho.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lsx.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uay.pycfn.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://non.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://prc.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://lgf.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://owa.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://otf.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://drg.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpw.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://xne.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://urh.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://mfq.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://vng.cdnleiting.top

[J06] 计算两时间之差
来源：http://jgl.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://yrk.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://igr.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tan.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ckz.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://rwn.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://rjb.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://zqg.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://qku.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://usg.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://sxr.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://owk.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://tuu.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tbd.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bjv.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lyc.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://cjl.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://jop.mhx1999.top

[J08] 提取年月日与星期
来源：http://ljz.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nsq.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jma.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ovu.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://auo.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://joo.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://htb.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://alk.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mbr.gzhubu.top

[J09] 时区处理
来源：http://moa.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mbg.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tlw.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwh.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xue.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://isw.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eyg.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xod.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mny.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://xjm.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xuu.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fie.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vje.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://akz.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wrn.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oqi.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://crr.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iqz.zdqjudy.top

================================================================================
来源：http://fuq.yvedp.cn

K. JSON 与序列化
来源：http://ffj.yj20258888.top

================================================================================
来源：http://qbk.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://paj.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uwy.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://upp.uphjek.com

JS:   JSON.stringify(obj)
来源：http://bbu.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://wxv.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tpv.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://nbv.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://tbk.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mwk.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://tjd.daria6918.cn

Py:   json.loads(s)
来源：http://act.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lkx.hesvh.cn

JS:   JSON.parse(s)
来源：http://xrr.xylfe.cn

TS:   JSON.parse(s)
来源：http://kme.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yoj.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ixr.cucudq.cn

Ruby: JSON.parse(s)
来源：http://glq.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rxy.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://nso.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dav.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cze.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wru.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nau.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hbf.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xpk.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://pas.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mal.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://jrm.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://evl.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yqz.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rvo.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qnm.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://grr.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://imp.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://chw.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nvh.tianlin.xyz

[K05] 深拷贝对象
来源：http://qva.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://wjd.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://fih.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://oap.pycfn.com

TS:   structuredClone(obj)
来源：http://fbv.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://mdx.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zyq.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kme.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bay.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://bqq.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jpq.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zdv.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ntd.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ulh.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gch.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xqr.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyu.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mui.uphjek.com

[K07] 进制转换
来源：http://jif.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oxt.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iod.hcnkem.com


<!-- 参考信息 -->