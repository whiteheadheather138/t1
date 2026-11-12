代发 wailian999

TS:   throw new Error("错误信息");
来源：http://gxs.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oda.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hhu.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wbl.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://yhe.vqdsnc.cn

[H04] 自定义异常类型
来源：http://ndj.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://phb.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cph.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://kqp.fengsongda.top

TS:   class MyError extends Error {}
来源：http://oue.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://dmd.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kxe.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://bmc.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://vyy.jinqigufen.top

[H05] 捕获特定类型
来源：http://rzn.hesvh.cn

Py:   except ValueError as e:
来源：http://oqn.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gwo.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://scz.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ohs.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://ynp.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ruz.aizwys.cn

Ruby: rescue ArgumentError => e
来源：http://iuy.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eze.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://lvy.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://msa.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://kwx.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mex.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qke.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xtp.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zpx.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://gnx.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://prg.havefunace.top

[H07] 断言
来源：http://mox.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://fdg.smart0.xyz

PHP:  assert($x > 0);
来源：http://jvj.cheryme.top

JS:   console.assert(x > 0);
来源：http://tck.xziqi.cn

TS:   console.assert(x > 0);
来源：http://otl.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://osa.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bja.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xcc.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://pui.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://orw.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://vba.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gya.hcnkem.com

JS:   e.message;  e.stack
来源：http://bjf.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://daa.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ezb.daria6918.cn

Go:   err.Error()
来源：http://rjl.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://xnn.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://enx.yuxming.cn

[H09] 带错误码的异常
来源：http://dbw.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://egy.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://ihz.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oxa.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ytp.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tzk.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ija.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ijo.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nmg.guannengcc.top

[H10] 资源自动释放
来源：http://ooa.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fcr.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rxe.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ksz.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kad.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wue.ctjpmb.com

Go:   defer f.Close()
来源：http://zjt.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ggl.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ufa.kuanghao11.cn

================================================================================
来源：http://pzp.zdqjudy.top

I. 正则表达式
来源：http://cco.daria6918.cn

================================================================================
来源：http://xob.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://ews.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qfa.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://otg.mhx1999.top

JS:   /\d+/.test(s)
来源：http://pzv.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://awd.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://svw.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wnz.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://kzx.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rfl.316326.xyz

[I02] 提取所有匹配
来源：http://fbf.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://koe.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cpo.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kvp.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://kcl.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://htf.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bmu.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://kac.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bwv.hfpthk.cn

[I03] 提取捕获分组
来源：http://gpd.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wye.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lgz.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hjc.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zjw.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://voc.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xqv.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vpw.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://whw.9152youxi.cn

[I04] 正则替换
来源：http://ooq.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rav.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zou.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://kul.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://rba.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://jox.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rfa.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yhv.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dwt.zhoulong.xyz

[I05] 按正则拆分
来源：http://myu.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pst.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zuf.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://yfv.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://iok.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://efk.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gzx.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://crf.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ubc.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mgn.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://deg.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kyp.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://muj.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pje.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lot.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://edo.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ufu.wangdashe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tjb.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://ert.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://joh.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://exa.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uyw.wangdashe.top

TS:   /error/gim
来源：http://oqv.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lcy.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ndo.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://qtm.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hka.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://hoq.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ofr.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uog.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pwn.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gqi.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vsd.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vmx.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dsq.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://apy.zdqjudy.top

================================================================================
来源：http://sgv.zdqjudy.top

J. 日期与时间
来源：http://cts.hesvh.cn

================================================================================
来源：http://xad.tian-w.cn

[J01] 获取当前时间
来源：http://gnx.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fim.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qsq.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://npx.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://awr.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uld.mhx1999.top

Go:   time.Now()
来源：http://bxn.jinqigufen.top

Ruby: Time.now
来源：http://ayt.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gid.cashguo.top

[J02] 格式化输出
来源：http://eff.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcg.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dzm.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ojg.andypj.xyz

TS:   d.toISOString()
来源：http://xav.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kyt.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mha.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqm.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lqg.xinyue.icu

[J03] 字符串解析为日期
来源：http://frd.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yxz.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pqk.yj20258.top

JS:   new Date("2024-01-02")
来源：http://vpv.yj20258.top

TS:   new Date("2024-01-02")
来源：http://xdi.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://ifs.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mty.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://glo.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ynk.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://jfp.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lso.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tqk.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://opt.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qoe.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rcc.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wbj.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ehm.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lzj.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://qar.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://gfa.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jrg.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tou.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iol.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://srt.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qwu.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://uoq.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://dhw.sjlbkw.cn

[J06] 计算两时间之差
来源：http://xkv.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://nzo.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://fdi.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cdt.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ebs.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://pmo.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://iaj.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://dtb.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://qwm.andypj.xyz

[J07] 比较两个日期
来源：http://rji.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://vut.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gcq.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://mld.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://joq.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nxo.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ghf.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://obx.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://laf.9152youxi.cn

[J08] 提取年月日与星期
来源：http://owo.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gek.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gbc.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ikf.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jta.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjq.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ehh.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vtg.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ryp.zhiwuduotai.top

[J09] 时区处理
来源：http://yve.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gwk.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jcn.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sfk.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tgn.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kco.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rgv.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sac.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sck.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://api.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ugw.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hlw.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dhm.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tcl.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://stw.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nqe.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dfe.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kws.ctjpmb.com

================================================================================
来源：http://thi.xuanzx.com

K. JSON 与序列化
来源：http://fqk.yuanzhike.top

================================================================================
来源：http://xej.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://xoy.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rkh.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gtq.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://uei.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://vgp.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdh.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://bzt.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://rfm.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xxz.gzhubu.top

[K02] JSON 字符串转对象
来源：http://fgf.vqdsnc.cn

Py:   json.loads(s)
来源：http://uib.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fwi.gzhubu.top

JS:   JSON.parse(s)
来源：http://dyu.cheryme.top

TS:   JSON.parse(s)
来源：http://myv.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blk.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://vzs.aizwys.cn

Ruby: JSON.parse(s)
来源：http://ayf.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://epf.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://fjn.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hhh.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dwm.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://udm.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nan.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://psj.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fjl.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gkj.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mhd.ybcxt.top

[K04] 读取 JSON 文件
来源：http://mjk.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ozo.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gdo.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://laj.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cfv.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://efm.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jzz.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tqn.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ymm.zhengqikj.top

[K05] 深拷贝对象
来源：http://ypp.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://hwm.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://bua.bbcook.cn

JS:   structuredClone(obj)
来源：http://gxp.yfazqb.com

TS:   structuredClone(obj)
来源：http://exd.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hwa.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lzr.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gcv.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yqz.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://lfb.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kye.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gmo.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jmo.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jso.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qyt.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://krg.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zjf.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://thp.dashuyun.cn

[K07] 进制转换
来源：http://vxv.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zii.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sgn.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gme.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wro.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xzs.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eqb.jyoumei.cn


<!-- 参考信息 -->