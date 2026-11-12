代发 wailian999

TS:   throw new Error("错误信息");
来源：http://sul.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oaf.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pjr.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iiq.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nav.svipenyu.cn

[H04] 自定义异常类型
来源：http://cem.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://qtu.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pru.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://mvu.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://igx.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://pdk.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://czu.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://hog.meibo888.top

C#:   class MyException : Exception {}
来源：http://dla.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://qql.fzhhl.top

Py:   except ValueError as e:
来源：http://jnn.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ayi.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://zgs.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://abq.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://bzq.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ohh.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://qgx.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xsg.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://awy.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://rbc.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wyf.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ksw.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ztq.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rno.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pui.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://lpy.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://crs.xinyue.icu

[H07] 断言
来源：http://jhj.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://tdt.haohaochexian.top

PHP:  assert($x > 0);
来源：http://obg.shuidangran.top

JS:   console.assert(x > 0);
来源：http://qal.yonumen.top

TS:   console.assert(x > 0);
来源：http://gcl.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://imv.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nil.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://quf.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://lrl.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://awm.gaohongyu789.top

Py:   str(e);  traceback.format_exc()
来源：http://gfi.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://edq.ehwqpu.com

JS:   e.message;  e.stack
来源：http://zhb.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://mim.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oze.jinqigufen.top

Go:   err.Error()
来源：http://oym.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://nrn.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://ats.tianlin.xyz

[H09] 带错误码的异常
来源：http://wqv.zdqjudy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yiw.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eab.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hgp.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://thf.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://whn.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lip.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://yhq.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pdr.epnwcf.com

[H10] 资源自动释放
来源：http://rod.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dhp.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vst.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://guu.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fwo.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ryk.yangfankeji.com

Go:   defer f.Close()
来源：http://lnv.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wdl.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qlk.xylfe.cn

================================================================================
来源：http://qfi.nanxinkj.top

I. 正则表达式
来源：http://xki.yangfankeji.com

================================================================================
来源：http://ikp.smart0.xyz

[I01] 判断是否匹配
来源：http://ezs.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ani.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://pjw.gzhubu.top

JS:   /\d+/.test(s)
来源：http://yen.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://jxd.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cjc.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cos.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://xbq.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wxw.yuanzhike.top

[I02] 提取所有匹配
来源：http://dls.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://yga.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bzk.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gwk.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://ygy.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hzk.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zpi.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://tvm.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://taw.tanke756.top

[I03] 提取捕获分组
来源：http://whg.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oae.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://emc.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qnu.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dwz.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pio.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://voo.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bbc.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ubn.redwolf501.top

[I04] 正则替换
来源：http://zqn.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xta.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lzs.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://asq.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://xop.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://cuj.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uyv.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cmr.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iks.sysykeji.top

[I05] 按正则拆分
来源：http://nci.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bti.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://izh.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://khq.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://jeh.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://beb.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hrv.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://vdp.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bsc.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pvt.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mmf.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lda.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpw.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nff.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://poa.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dip.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fou.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uig.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://ckn.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tvl.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fde.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qjr.nanxuanxn.top

TS:   /error/gim
来源：http://yvs.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bqe.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wrn.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://nxf.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vnv.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://xfb.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lzi.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://swg.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycu.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vso.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dst.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rrp.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bau.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bkl.xinyue.icu

================================================================================
来源：http://pme.hesvh.cn

J. 日期与时间
来源：http://fyd.zhaomingkeji.xyz

================================================================================
来源：http://dmm.yanxiufei.cn

[J01] 获取当前时间
来源：http://zoh.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ogq.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ukk.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://pis.yj202588.top

TS:   new Date();  Date.now()
来源：http://cnp.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vvg.nanxuanxn.top

Go:   time.Now()
来源：http://dod.ywan-chungtsiang.top

Ruby: Time.now
来源：http://ywn.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://udd.cdnleiting.top

[J02] 格式化输出
来源：http://cui.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://brv.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mfk.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xyg.hfpthk.cn

TS:   d.toISOString()
来源：http://npz.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fak.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hpt.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bju.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://msa.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://pem.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bqu.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wmi.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://sst.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://fxo.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://hbi.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wdg.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://yon.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cis.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://qsq.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qqe.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lvw.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dfy.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://fsr.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gcr.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://onh.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sen.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://owo.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://sfx.cheryme.top

Py:   now + timedelta(days=7)
来源：http://wra.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dnh.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eis.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gge.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://zhf.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cye.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://cyf.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://kfg.tarul.cn

[J06] 计算两时间之差
来源：http://plw.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://wnh.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://zce.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tvj.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pan.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fuz.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://odu.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://nwt.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://ksh.redwolf501.top

[J07] 比较两个日期
来源：http://rkl.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://dsf.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ass.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://kxs.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://ykx.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tbm.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dyq.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://byh.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://lij.haohaochexian.top

[J08] 提取年月日与星期
来源：http://apu.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cmh.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ivz.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gcq.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pnq.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ebt.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lew.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gma.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cvl.gzhubu.top

[J09] 时区处理
来源：http://auy.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://owu.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rnh.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cob.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gdl.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fji.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yso.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://rld.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vxc.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://gzx.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ine.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iew.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://loe.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bfw.feifeiyinyue.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jnf.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bsw.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zsa.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gyb.zhijiandao.cn

================================================================================
来源：http://fpn.daxiang520.top

K. JSON 与序列化
来源：http://flw.yanxiufei.cn

================================================================================
来源：http://irs.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://ana.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kiy.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ldy.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://qav.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://yku.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gla.uphjek.com

Go:   json.Marshal(obj)
来源：http://unw.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://jvq.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oru.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://dqc.daria6918.cn

Py:   json.loads(s)
来源：http://kaj.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fjt.9152youxi.cn

JS:   JSON.parse(s)
来源：http://iup.cqqwz.cn

TS:   JSON.parse(s)
来源：http://omj.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pkq.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://plx.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://ktt.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://via.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://rmj.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gci.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oaa.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://mvr.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://coz.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bjy.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://osl.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://zrx.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qyd.smart0.xyz

[K04] 读取 JSON 文件
来源：http://zbb.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tqn.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kre.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rvl.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ovw.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sug.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ppv.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zol.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xls.gotoacloud.top

[K05] 深拷贝对象
来源：http://fua.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://kle.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://cmw.ivvv.top

JS:   structuredClone(obj)
来源：http://pbo.iojbl.cn

TS:   structuredClone(obj)
来源：http://ayt.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ueb.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sxh.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dud.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fuf.hcnkem.com

[K06] 解析 URL 查询串
来源：http://eoq.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gyr.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zvx.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhi.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://phx.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kow.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xel.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wim.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qdr.chenzaomai.com

[K07] 进制转换
来源：http://gmf.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cdn.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uew.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xmy.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ptt.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fwl.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cem.zdbjq.cn


<!-- 参考信息 -->