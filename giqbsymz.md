代发 wailian999

[H03] 主动抛出异常
来源：http://azu.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://fey.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gkj.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://lcj.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://kvn.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xsl.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mth.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iup.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://vvu.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://lbd.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://ath.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uem.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://vjv.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://uzh.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://dgb.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gtn.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://dwp.hnqzz.top

C#:   class MyException : Exception {}
来源：http://jdy.ivvv.top

[H05] 捕获特定类型
来源：http://mcy.pycfn.com

Py:   except ValueError as e:
来源：http://cgj.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wtu.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://dko.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://nlg.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://kpd.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uns.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://elw.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qnj.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://trm.cashguo.top

Py:   value = d.get("k") or default
来源：http://eww.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bij.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://kio.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://mmx.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yqw.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iym.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://bci.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://wew.hongshengwenyu.top

[H07] 断言
来源：http://pyq.jinqigufen.top

Py:   assert x > 0, "必须为正"
来源：http://fuk.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://qfk.ybcxt.top

JS:   console.assert(x > 0);
来源：http://fqe.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://zxr.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://dwb.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ouk.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://ljo.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://egk.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://gaj.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://udo.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oyq.yfazqb.com

JS:   e.message;  e.stack
来源：http://oak.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://svv.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hhg.guannengcc.top

Go:   err.Error()
来源：http://koo.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://dnc.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://uvm.guannengcc.top

[H09] 带错误码的异常
来源：http://kxd.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fmz.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jnc.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ccu.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tpm.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ybf.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lhb.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://rch.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://opt.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://whm.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://ldu.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jpi.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zlw.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lsb.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sgu.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://zfp.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vcv.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yrb.daxiang520.top

================================================================================
来源：http://vvv.sxryk.cn

I. 正则表达式
来源：http://xug.feifeiyinyue.top

================================================================================
来源：http://zch.havefunace.top

[I01] 判断是否匹配
来源：http://nyn.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tze.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://bnt.ydzc1.top

JS:   /\d+/.test(s)
来源：http://vjl.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://glr.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uso.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rlt.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://yzy.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gmh.mhx1999.top

[I02] 提取所有匹配
来源：http://meh.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://cxj.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lbe.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ndv.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://bod.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yue.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ruo.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://lef.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ond.daria6918.cn

[I03] 提取捕获分组
来源：http://hzc.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jzo.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://chr.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tzs.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://taf.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://djn.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpf.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xbn.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tvq.pengpengdd.cyou

[I04] 正则替换
来源：http://rtc.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hzn.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rmv.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vsk.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://ouh.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://znq.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gna.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kgz.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mag.uphjek.com

[I05] 按正则拆分
来源：http://bwd.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gcn.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://smu.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://fbj.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://hyd.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://icz.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gju.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ysk.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wtt.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://knw.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cuw.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fyr.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krw.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fjp.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wfc.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gft.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cpq.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tvk.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://bop.ctjpmb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gho.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vlp.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ckm.cheryme.top

TS:   /error/gim
来源：http://xvm.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bqw.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://svs.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://taz.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lqw.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://tde.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gll.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbo.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://max.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oli.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oji.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kzh.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vlr.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dwz.tian-w.cn

================================================================================
来源：http://lrg.yuxming.cn

J. 日期与时间
来源：http://oco.sweek.top

================================================================================
来源：http://vdj.jqgufenzy.top

[J01] 获取当前时间
来源：http://fgo.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://lav.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ggj.52xcode.cn

JS:   new Date();  Date.now()
来源：http://bnl.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://bkx.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gtq.yueranfly.top

Go:   time.Now()
来源：http://mbh.jqgufenzy.top

Ruby: Time.now
来源：http://tti.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bzh.xuanzx.com

[J02] 格式化输出
来源：http://vws.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gnf.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ucm.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uka.tanke756.top

TS:   d.toISOString()
来源：http://hps.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lje.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qrh.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sdm.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qth.316326.xyz

[J03] 字符串解析为日期
来源：http://juv.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bde.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pcs.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://nup.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://lpq.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cjp.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gzn.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://lnl.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ptn.52xcode.cn

[J04] 时间戳与日期互转
来源：http://epj.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oex.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dla.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ame.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kwh.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tin.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ddu.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sap.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://usx.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://upe.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://lfn.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://otl.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nhj.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pye.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://fue.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iyw.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://wia.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xwk.yuxming.cn

[J06] 计算两时间之差
来源：http://ncg.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://wpa.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://fir.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gos.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cfz.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fgp.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://oyy.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://gkf.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://kly.tianlin.xyz

[J07] 比较两个日期
来源：http://yjd.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://utq.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uer.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://mfx.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://wtq.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gtm.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://orq.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://eao.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://oqj.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://cjf.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wti.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jti.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://epp.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vuc.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vth.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tcg.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tjw.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tam.52xcode.cn

[J09] 时区处理
来源：http://hdz.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://asf.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jqr.birdmap.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gvp.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eqv.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bmm.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wpo.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sgv.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://opt.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://bdn.guowangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ktt.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ohc.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jwm.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://abc.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cla.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://odl.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oxz.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gud.zdqjudy.top

================================================================================
来源：http://gwx.gogol.net.cn

K. JSON 与序列化
来源：http://lmh.fanxiaobao.xyz

================================================================================
来源：http://ywi.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://cbl.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ixb.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mce.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://slb.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://sdt.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sin.hcnkem.com

Go:   json.Marshal(obj)
来源：http://ckn.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://ycn.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fkc.c1oappe.top

[K02] JSON 字符串转对象
来源：http://vdl.316326.xyz

Py:   json.loads(s)
来源：http://pos.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ugy.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://oxu.hywenlv.cn

TS:   JSON.parse(s)
来源：http://frv.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wie.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://nvd.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://oiu.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oxk.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://nkg.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ojr.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qze.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://buj.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://qib.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lxj.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cvw.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://ene.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uew.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://emu.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mas.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wlh.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cad.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xlz.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hli.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jzf.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://soz.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wph.ydzc1.top

[K05] 深拷贝对象
来源：http://vwu.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://ytd.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://frn.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://cqf.bbcook.cn

TS:   structuredClone(obj)
来源：http://eea.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fan.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cja.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gcy.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hee.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://rdd.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vki.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nko.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vka.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lsq.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bar.ydzc1.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dmt.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mvi.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://alg.zhengqikj.top

[K07] 进制转换
来源：http://mft.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oyx.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ahh.shzxlz.cn


<!-- 参考信息 -->