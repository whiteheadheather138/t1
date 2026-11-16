代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://kkh.gaohongyu789.top

[H04] 自定义异常类型
来源：http://qgz.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://pok.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://bmr.andypj.xyz

JS:   class MyError extends Error {}
来源：http://whc.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://ily.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://lyl.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://piw.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://kxr.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://gig.cucudq.cn

[H05] 捕获特定类型
来源：http://ull.hammf.cn

Py:   except ValueError as e:
来源：http://eiz.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mjv.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://hta.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://cuv.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://uwn.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lhf.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://ioo.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hcr.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://stc.tian-w.cn

Py:   value = d.get("k") or default
来源：http://fxj.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://fxl.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uus.daxiang520.top

TS:   obj?.a?.b;  d ?? default
来源：http://hqv.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://awd.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kyy.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://yas.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://wrg.snrcjt.cn

[H07] 断言
来源：http://vxo.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://tap.birdmap.top

PHP:  assert($x > 0);
来源：http://mfp.iojbl.cn

JS:   console.assert(x > 0);
来源：http://miu.andypj.xyz

TS:   console.assert(x > 0);
来源：http://qef.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://zpn.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://glm.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://avz.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://pgg.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://gwx.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://xwn.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rpq.hysaishi.cn

JS:   e.message;  e.stack
来源：http://wia.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://izn.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wfz.bjfxy.top

Go:   err.Error()
来源：http://elx.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://kzf.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://fug.aibaodan.cn

[H09] 带错误码的异常
来源：http://cfw.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vqu.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://foi.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vrj.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qlg.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kiy.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rgx.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://nku.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rxa.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://cty.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://vti.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://usi.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rbj.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nud.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jcw.xziqi.cn

Go:   defer f.Close()
来源：http://skl.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fhw.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zrm.cqqwz.cn

================================================================================
来源：http://lkv.iojbl.cn

I. 正则表达式
来源：http://als.cucudq.cn

================================================================================
来源：http://slj.zdqjudy.top

[I01] 判断是否匹配
来源：http://khu.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gty.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://osi.wangdashe.top

JS:   /\d+/.test(s)
来源：http://efs.mhx1999.top

TS:   /\d+/.test(s)
来源：http://amd.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xfg.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jvd.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://ejg.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ozj.gaohongyu789.top

[I02] 提取所有匹配
来源：http://fkn.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://dyj.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cqy.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://naz.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://xpc.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://did.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jwr.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://fqt.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zwh.bjfxy.top

[I03] 提取捕获分组
来源：http://lcj.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wpo.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wtf.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zqt.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bzd.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cmo.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://smq.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ftg.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tqv.andypj.xyz

[I04] 正则替换
来源：http://qum.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://uld.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://umf.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mtq.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://bla.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://cyb.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://qdk.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://snx.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uar.ehwqpu.com

[I05] 按正则拆分
来源：http://lhl.zdqjudy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://thl.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pok.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://iuq.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://vkg.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://crr.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rou.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gwh.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uft.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lfk.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pvt.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mjp.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iqy.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jjz.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wwt.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ydx.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://txt.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tan.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://gtr.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zlw.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nuq.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sed.sxryk.cn

TS:   /error/gim
来源：http://aod.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zgp.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pbg.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://wta.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xxq.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://kfn.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iun.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://siq.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nuc.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bxr.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pyb.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ukq.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cte.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eei.yueranfly.top

================================================================================
来源：http://grs.guannengcc.top

J. 日期与时间
来源：http://xqd.hcnkem.com

================================================================================
来源：http://ylp.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://ztl.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zdh.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xtc.yongpay.top

JS:   new Date();  Date.now()
来源：http://xje.fehbvm.com

TS:   new Date();  Date.now()
来源：http://xvt.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://taf.jinqigfzy.top

Go:   time.Now()
来源：http://hwr.zhongyouzk.top

Ruby: Time.now
来源：http://qll.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uyg.pycfn.com

[J02] 格式化输出
来源：http://nlm.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fus.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jiy.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fsc.shuidangran.top

TS:   d.toISOString()
来源：http://dqm.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vxm.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zyn.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xzj.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ogp.yueranfly.top

[J03] 字符串解析为日期
来源：http://bea.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aiq.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fjp.pycfn.com

JS:   new Date("2024-01-02")
来源：http://wsb.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://lwd.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://urv.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fes.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://ljw.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nyf.nwbrower.top

[J04] 时间戳与日期互转
来源：http://dsb.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kvi.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cal.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://igr.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wao.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qut.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dgp.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fyx.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dmm.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://lws.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://lbl.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rcj.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ymn.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wyb.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://vrh.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ltw.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://qtv.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nct.zhijiandao.cn

[J06] 计算两时间之差
来源：http://jwm.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://crf.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://ber.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lnw.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jth.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cgk.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://lka.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://zfi.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://erd.meibo888.top

[J07] 比较两个日期
来源：http://ujd.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bks.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ztp.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://mai.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://zjk.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pzs.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xwj.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://nyk.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://lvu.dianchejie.cn

[J08] 提取年月日与星期
来源：http://fgg.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ulo.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kkg.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://all.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://del.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jhh.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qnq.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bzx.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jtt.bjfxy.top

[J09] 时区处理
来源：http://iwo.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cty.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://abh.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mkr.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oxm.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fhy.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zis.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ato.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jlf.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://mwp.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fii.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ptk.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ubj.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ehw.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xzl.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jra.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xav.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jfw.316326.xyz

================================================================================
来源：http://qwv.hywenlv.cn

K. JSON 与序列化
来源：http://jda.gotoacloud.top

================================================================================
来源：http://mie.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://ylu.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vtx.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mim.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://llg.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://itv.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bxs.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://dpb.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://zfi.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qal.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://ajh.hysaishi.cn

Py:   json.loads(s)
来源：http://mjo.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rib.ydzc1.top

JS:   JSON.parse(s)
来源：http://ecv.tian-w.cn

TS:   JSON.parse(s)
来源：http://hao.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kqn.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://fku.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://yud.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ulk.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://szv.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pif.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jwl.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fxt.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gdd.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dvh.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fpd.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://zeq.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rqe.andypj.xyz

[K04] 读取 JSON 文件
来源：http://gkk.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tpc.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wtx.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dgu.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lfo.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gea.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bht.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://lne.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oxt.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://zln.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://coh.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://vfp.yangfankeji.com

JS:   structuredClone(obj)
来源：http://msl.fktsv.cn

TS:   structuredClone(obj)
来源：http://pac.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gna.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://osy.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jjl.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mth.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://mez.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jko.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cvk.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sgc.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvy.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vaw.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nhm.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rfv.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jxu.yvedp.cn

[K07] 进制转换
来源：http://xlf.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wyp.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fro.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ucw.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cdk.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fhx.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xry.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pgs.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zha.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://pkv.yongpay.top

Py:   pickle.dumps(obj)
来源：http://ian.xylfe.cn


<!-- 参考信息 -->