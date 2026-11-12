代发 wailian999

TS:   throw new Error("错误信息");
来源：http://gfn.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ase.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vki.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ytk.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tvp.chenzaomai.com

[H04] 自定义异常类型
来源：http://ivk.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://idm.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bpx.nwbrower.top

JS:   class MyError extends Error {}
来源：http://wbn.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://vuv.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://hxx.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rcv.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://isk.yj202588.top

C#:   class MyException : Exception {}
来源：http://psd.pycfn.com

[H05] 捕获特定类型
来源：http://jgm.yj20258.top

Py:   except ValueError as e:
来源：http://pci.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jpi.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://iog.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://ouq.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://uqt.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pft.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://ajb.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jgd.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://rns.andypj.xyz

Py:   value = d.get("k") or default
来源：http://ser.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://ybb.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://ybj.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://xwo.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lgy.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://sud.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://wwu.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://wfc.cucudq.cn

[H07] 断言
来源：http://emw.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://lcw.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://ujk.yj20258.top

JS:   console.assert(x > 0);
来源：http://vsr.guannengcc.top

TS:   console.assert(x > 0);
来源：http://zwr.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://fhn.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jew.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://yuk.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://izw.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://wsk.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://yzd.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ztv.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://moy.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mmm.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rke.wangshuangyany.cn

Go:   err.Error()
来源：http://jzh.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://ets.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://cvb.yuxming.cn

[H09] 带错误码的异常
来源：http://zcd.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tml.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rdh.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vdd.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://txl.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mzg.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hlp.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://otl.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xnu.ehwqpu.com

[H10] 资源自动释放
来源：http://ddg.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xlp.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dhz.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vmj.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://net.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lag.hcnkem.com

Go:   defer f.Close()
来源：http://azq.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iem.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://alh.bjfxy.top

================================================================================
来源：http://fcz.hfpthk.cn

I. 正则表达式
来源：http://okx.hnqzz.top

================================================================================
来源：http://yek.smart0.xyz

[I01] 判断是否匹配
来源：http://pjn.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bra.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://aab.uphjek.com

JS:   /\d+/.test(s)
来源：http://jdi.sxryk.cn

TS:   /\d+/.test(s)
来源：http://fio.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uup.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vrv.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://pzk.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xam.smart0.xyz

[I02] 提取所有匹配
来源：http://zsq.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://knx.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rei.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rlv.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://xcq.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mnk.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nqr.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://tgd.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jwu.cucudq.cn

[I03] 提取捕获分组
来源：http://ctr.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kwl.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mbq.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ssg.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xdm.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://egc.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ubj.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fko.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kub.shangyingyoupin.top

[I04] 正则替换
来源：http://xjj.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://vae.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nus.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://hvp.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://mbj.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://lmu.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fcb.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kwi.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lsw.wangdashe.top

[I05] 按正则拆分
来源：http://jcj.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mwh.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lge.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://cyn.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://tid.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://etd.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jre.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://vnj.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kni.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rux.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kvt.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nnt.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygq.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgu.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rrx.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zqb.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pqp.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wlw.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://qni.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://man.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vrb.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zlu.fehbvm.com

TS:   /error/gim
来源：http://juu.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sbo.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gfv.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://ere.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tbd.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://ktq.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zxk.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tof.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zzv.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pkg.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://adh.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zip.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vrt.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wyt.chenzaomai.com

================================================================================
来源：http://ydh.ydjk.org.cn

J. 日期与时间
来源：http://glr.uphjek.com

================================================================================
来源：http://xtf.smart0.xyz

[J01] 获取当前时间
来源：http://xxs.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rpc.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wyf.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://qhz.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://rkv.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oaj.daria6918.cn

Go:   time.Now()
来源：http://med.jqgfzy.top

Ruby: Time.now
来源：http://kwx.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wvb.jqgufenzy.top

[J02] 格式化输出
来源：http://gzm.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mkm.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fwf.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tuk.dianchejie.cn

TS:   d.toISOString()
来源：http://mfv.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://idl.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zut.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://obp.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zjd.hammf.cn

[J03] 字符串解析为日期
来源：http://awz.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fca.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aru.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://ygv.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://dok.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://iav.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ilv.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://aad.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fwv.tanke756.top

[J04] 时间戳与日期互转
来源：http://hnu.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oyg.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccw.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iut.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://sdl.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mnd.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bhm.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rcd.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://phh.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://pnt.yj202588.top

Py:   now + timedelta(days=7)
来源：http://wsx.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xpg.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oxt.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvo.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://ddn.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qlr.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://vok.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://ggz.ehwqpu.com

[J06] 计算两时间之差
来源：http://ijk.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://urf.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://upa.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fmm.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kqd.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://fzl.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://iuy.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://qro.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://xft.jianghu66.top

[J07] 比较两个日期
来源：http://kyu.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://xeb.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://peh.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://hhi.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ayt.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cpm.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pfo.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://hfm.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://gxm.tarul.cn

[J08] 提取年月日与星期
来源：http://bdm.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wde.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fnm.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xfa.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zrv.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://epc.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wbm.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wsm.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rdv.quarkkingdee.top

[J09] 时区处理
来源：http://ljp.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vda.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ywi.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://obb.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://apu.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rah.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sow.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fwv.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vjt.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://aox.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://acg.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cpz.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dcz.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eae.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://emj.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fdx.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gls.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://stm.52xcode.cn

================================================================================
来源：http://uvo.gzhubu.top

K. JSON 与序列化
来源：http://jnp.ehwqpu.com

================================================================================
来源：http://ohr.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://fbh.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iio.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://drl.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://ebj.yonumen.top

TS:   JSON.stringify(obj)
来源：http://yfh.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vrc.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://pxp.zycfv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hva.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qlb.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://gwt.hesvh.cn

Py:   json.loads(s)
来源：http://guw.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rus.aizwys.cn

JS:   JSON.parse(s)
来源：http://rjw.bbcook.cn

TS:   JSON.parse(s)
来源：http://jqy.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rlz.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://bny.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://ujz.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cej.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://yee.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fbg.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jnj.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ldx.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rsn.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jxh.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hob.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://jac.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rhr.ivvv.top

[K04] 读取 JSON 文件
来源：http://rqu.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xav.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ipz.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kup.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nfj.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://axk.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fib.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jwk.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ghy.cashguo.top

[K05] 深拷贝对象
来源：http://nkp.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://bmm.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://wqe.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://shq.hnqzz.top

TS:   structuredClone(obj)
来源：http://qiz.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://opw.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mmp.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://abn.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://abp.c1oappe.top

[K06] 解析 URL 查询串
来源：http://pmn.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jdg.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kbj.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uhr.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jao.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jrm.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iwd.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dln.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tzi.tarul.cn

[K07] 进制转换
来源：http://nvq.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gcc.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pfe.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ltg.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nfb.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ppi.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jph.sxryk.cn


<!-- 参考信息 -->