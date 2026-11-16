代发 wailian999

TS:   throw new Error("错误信息");
来源：http://mzm.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://glm.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mjv.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://acq.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://ndh.vqdsnc.cn

[H04] 自定义异常类型
来源：http://apa.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://dsq.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://twe.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://mhg.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://jpq.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://ded.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cwy.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://dlx.shuidangran.top

C#:   class MyException : Exception {}
来源：http://fgb.cqqwz.cn

[H05] 捕获特定类型
来源：http://fbs.pycfn.com

Py:   except ValueError as e:
来源：http://ean.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oef.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://fur.shzxlz.cn

TS:   if (e instanceof TypeError) {}
来源：http://vkz.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://kxm.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://koa.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://tit.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fwn.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://tcy.shuidangran.top

Py:   value = d.get("k") or default
来源：http://kok.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://qmp.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://fmo.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://ndr.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lgr.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wco.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://yrp.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://lbg.zhoulong.xyz

[H07] 断言
来源：http://pby.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://opn.yvedp.cn

PHP:  assert($x > 0);
来源：http://pgo.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://ndu.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://ldv.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://jik.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zqx.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://puw.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://fqd.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://skt.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://snj.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xem.redwolf501.top

JS:   e.message;  e.stack
来源：http://yjp.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://owx.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fge.andypj.xyz

Go:   err.Error()
来源：http://hlu.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://ivs.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://mxq.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://gzk.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bjr.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://iic.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://thu.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wfu.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xhk.zhixingplan.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://snw.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://utp.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ckl.tarul.cn

[H10] 资源自动释放
来源：http://nkf.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yrr.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gxu.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ibh.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ofz.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sgi.feifeiyinyue.top

Go:   defer f.Close()
来源：http://hsq.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zpv.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hcf.guannengcc.top

================================================================================
来源：http://ryq.shuidangran.top

I. 正则表达式
来源：http://qbw.jqgufenzy.top

================================================================================
来源：http://ops.andypj.xyz

[I01] 判断是否匹配
来源：http://ryh.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nfd.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ixj.fktsv.cn

JS:   /\d+/.test(s)
来源：http://vud.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://mff.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qkp.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bar.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://pcu.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wjf.zhijiandao.cn

[I02] 提取所有匹配
来源：http://alz.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://znm.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dey.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fnw.tanke756.top

TS:   s.match(/\d+/g)
来源：http://pti.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aov.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lqu.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://snt.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zds.dianchejie.cn

[I03] 提取捕获分组
来源：http://kdj.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mkg.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://odb.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://brs.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qqs.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mqp.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugx.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qfp.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mrw.316326.xyz

[I04] 正则替换
来源：http://udt.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vqf.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hsr.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://srx.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ktu.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://zgr.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cdm.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fng.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ixh.gzhubu.top

[I05] 按正则拆分
来源：http://cnq.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uci.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yob.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://mib.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://hvb.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://znc.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ffw.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nbt.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nwt.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://igr.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uuy.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nvv.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rtg.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://otn.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qcr.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iyu.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://peo.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ine.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://tis.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eed.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pmd.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://krq.daria6918.cn

TS:   /error/gim
来源：http://ggz.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uib.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ojh.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://ljk.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wcr.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://ayp.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://grj.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bng.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://twu.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://spj.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kac.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rrh.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://edu.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qvp.pengpengdd.cyou

================================================================================
来源：http://qoq.sweek.top

J. 日期与时间
来源：http://sgw.hcnkem.com

================================================================================
来源：http://wjc.yueranfly.top

[J01] 获取当前时间
来源：http://tbx.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pua.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://shq.tanke756.top

JS:   new Date();  Date.now()
来源：http://krh.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://uhc.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://cte.wangshuangyany.cn

Go:   time.Now()
来源：http://xja.shangyingyoupin.top

Ruby: Time.now
来源：http://ezk.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nnr.xuanzx.com

[J02] 格式化输出
来源：http://mlc.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vwe.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gks.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ybs.hywenlv.cn

TS:   d.toISOString()
来源：http://sek.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wny.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gvs.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qic.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yut.fzhhl.top

[J03] 字符串解析为日期
来源：http://aph.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jke.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://usq.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://rmx.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://pbr.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://hfd.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://egp.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://iyo.ivvv.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kyx.tarul.cn

[J04] 时间戳与日期互转
来源：http://oue.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kgy.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nkd.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://psx.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vlf.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pib.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fwb.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://syk.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://osr.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://dwc.ivvv.top

Py:   now + timedelta(days=7)
来源：http://vxf.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qnp.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xpt.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nly.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://yon.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://moc.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://hpx.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cwi.c1oappe.top

[J06] 计算两时间之差
来源：http://vey.yj202588.top

Py:   (end - start).total_seconds()
来源：http://fea.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://gjv.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://abj.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hyz.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://vvp.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://owi.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://pmz.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://xns.sjlbkw.cn

[J07] 比较两个日期
来源：http://blc.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://uyq.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zqj.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ebc.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://bil.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hgw.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hap.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://efq.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://qmk.tianlin.xyz

[J08] 提取年月日与星期
来源：http://nxj.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qxh.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xtr.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://egd.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tns.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bwc.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yre.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kdp.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sxq.xuetiantiany.cn

[J09] 时区处理
来源：http://cna.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yvo.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ijf.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://izu.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vif.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oyz.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ihf.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bxm.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ozf.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://pja.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jbd.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://owy.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nqr.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://alk.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qeg.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mzt.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wjk.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zez.haohaochexian.top

================================================================================
来源：http://udc.fanxiaobao.xyz

K. JSON 与序列化
来源：http://zhg.daxiang520.top

================================================================================
来源：http://daq.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://ofu.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ntq.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gqx.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://wnk.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://dnx.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kud.sufxvd.cn

Go:   json.Marshal(obj)
来源：http://niz.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://cop.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://shg.yj202588.top

[K02] JSON 字符串转对象
来源：http://jdl.hnqzz.top

Py:   json.loads(s)
来源：http://rmu.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mxm.vehdjk.com

JS:   JSON.parse(s)
来源：http://ied.bjfxy.top

TS:   JSON.parse(s)
来源：http://nrz.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wtz.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://cyu.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://rao.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ugm.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://rcr.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fci.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fkq.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fsl.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://egi.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://twr.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fxc.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://ihk.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gfb.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://ubs.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nph.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gml.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vbq.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sww.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uin.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tin.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://iwb.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blv.ydzc1.top

[K05] 深拷贝对象
来源：http://fcu.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://pev.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://isg.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://ekq.ppjwa.cn

TS:   structuredClone(obj)
来源：http://jye.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tkj.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vzc.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cco.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dek.ivvv.top

[K06] 解析 URL 查询串
来源：http://gdu.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://srb.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gnp.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ipu.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mqs.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cwq.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jzs.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bkk.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://glc.ctjpmb.com

[K07] 进制转换
来源：http://mci.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sbq.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://evd.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://azj.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mlu.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jto.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yko.0kj1m.cn


<!-- 参考信息 -->