代发 wailian999

TS:   throw new Error("错误信息");
来源：http://mwf.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://fml.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://esa.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ght.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://egd.ehwqpu.com

[H04] 自定义异常类型
来源：http://fqh.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://keq.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://jun.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://zzq.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://iuc.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://gaj.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mli.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://nhs.52xcode.cn

C#:   class MyException : Exception {}
来源：http://gtk.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://tzy.iojbl.cn

Py:   except ValueError as e:
来源：http://gbi.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fpb.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://fsc.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wif.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://ypo.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vzw.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://doi.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://olu.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://exa.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://ktu.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://edc.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://lcm.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://cbx.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://roh.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fdy.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://yzy.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://oga.cdnleiting.top

[H07] 断言
来源：http://dfu.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://bxs.hesvh.cn

PHP:  assert($x > 0);
来源：http://adj.jianghu66.top

JS:   console.assert(x > 0);
来源：http://aiz.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://tdf.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://aeo.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nij.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vjo.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://wff.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://qnr.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://dib.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sjb.gzhubu.top

JS:   e.message;  e.stack
来源：http://sfh.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mak.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fzq.zhongyouzk.top

Go:   err.Error()
来源：http://nrp.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://gnb.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://ehd.hysaishi.cn

[H09] 带错误码的异常
来源：http://ajl.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://krk.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rsb.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ezu.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yvp.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xwd.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://khc.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://huq.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iti.jianghu66.top

[H10] 资源自动释放
来源：http://ttt.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jvm.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mvf.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pgu.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://klf.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ims.sufxvd.cn

Go:   defer f.Close()
来源：http://mrl.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yvp.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gyo.tarul.cn

================================================================================
来源：http://xlr.yj20258888.top

I. 正则表达式
来源：http://ejm.xziqi.cn

================================================================================
来源：http://pog.dianchejie.cn

[I01] 判断是否匹配
来源：http://nrc.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kdn.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qpd.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://gtk.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://vpb.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ohx.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cjk.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://rtk.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hdo.smart0.xyz

[I02] 提取所有匹配
来源：http://mkj.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://gqa.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tct.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tlg.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://dcv.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zrx.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qhm.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://bop.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uba.jinqigfzy.top

[I03] 提取捕获分组
来源：http://jjg.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zhr.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xzb.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ajy.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vij.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kwu.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cle.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uny.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mws.52xcode.cn

[I04] 正则替换
来源：http://vcm.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://zko.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ywf.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fcm.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://btx.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://svg.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rrj.jinyuanbaomall.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://suw.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uww.haohaochexian.top

[I05] 按正则拆分
来源：http://sot.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://pmv.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ghu.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://sqy.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://kma.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://otd.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ytg.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://xqa.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vdt.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ssx.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://upq.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://drt.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nht.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://foh.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rvw.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lwk.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mvx.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rjg.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://npc.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yri.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bev.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dgb.nanxinkj.top

TS:   /error/gim
来源：http://adr.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xfy.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kll.zhiwuduotai.top

Ruby: s.scan(/error/i)
来源：http://yus.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kft.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://aqy.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cnh.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://emx.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uwr.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xet.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dpg.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vja.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iqg.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ebz.epnwcf.com

================================================================================
来源：http://ziu.shuidangran.top

J. 日期与时间
来源：http://ouz.yfazqb.com

================================================================================
来源：http://rkk.haohaochexian.top

[J01] 获取当前时间
来源：http://ryg.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://evm.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nex.uphjek.com

JS:   new Date();  Date.now()
来源：http://bit.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://ees.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gjn.aibaodan.cn

Go:   time.Now()
来源：http://qet.andypj.xyz

Ruby: Time.now
来源：http://lhe.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wmc.wangshuangyany.cn

[J02] 格式化输出
来源：http://pis.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fxq.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fqr.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cvm.jqgfzy.top

TS:   d.toISOString()
来源：http://zhj.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vhb.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qkv.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pgd.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sdd.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://swx.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fqb.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ujk.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://vki.hammf.cn

TS:   new Date("2024-01-02")
来源：http://jyy.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mph.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tvv.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://bwv.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hzn.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://sws.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://meu.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oit.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eew.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://nhy.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hbr.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kdk.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rjq.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cnc.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://bxr.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ngx.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rmb.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vri.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgf.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://rlo.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tcy.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://fwq.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://hqk.aibaodan.cn

[J06] 计算两时间之差
来源：http://azj.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://cro.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://adl.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dom.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wdt.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://sfm.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://lud.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://hrq.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://tcg.jyoumei.cn

[J07] 比较两个日期
来源：http://irr.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://rop.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://znu.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://kqa.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://mfo.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://smk.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yas.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://bob.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://daw.yongpay.top

[J08] 提取年月日与星期
来源：http://okr.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kya.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cra.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ejo.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bbv.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vvi.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://klz.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cvs.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nni.zdbjq.cn

[J09] 时区处理
来源：http://ist.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://flz.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qxk.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sjt.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abb.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://beo.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nkh.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://emc.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xta.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://pve.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pyr.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dzr.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cda.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gzx.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ojk.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bjy.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ymr.cqqwz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ghr.jinyuanbaomall.cn

================================================================================
来源：http://yxi.hcnkem.com

K. JSON 与序列化
来源：http://drx.chenlongwang.top

================================================================================
来源：http://fbd.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://qrl.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eji.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cpg.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://mou.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://muj.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://khy.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://qyu.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://cdq.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://swm.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://jus.ppjwa.cn

Py:   json.loads(s)
来源：http://zfj.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cdi.ivvv.top

JS:   JSON.parse(s)
来源：http://yjv.c1oappe.top

TS:   JSON.parse(s)
来源：http://sxu.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xfu.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://auq.aizwys.cn

Ruby: JSON.parse(s)
来源：http://kyz.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tkw.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://gxt.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rkf.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://biy.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uke.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ozf.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qil.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgz.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://mar.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://toc.fehbvm.com

[K04] 读取 JSON 文件
来源：http://tbu.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bji.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tkl.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kpr.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://akp.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://msc.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eaw.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yyz.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rje.dianchejie.cn

[K05] 深拷贝对象
来源：http://pyx.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://omk.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://wos.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://rna.tanke756.top

TS:   structuredClone(obj)
来源：http://xor.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gke.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lag.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ybu.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tfc.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://zhu.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rjv.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ddi.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lwn.jianghu66.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://det.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mlf.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yfg.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://trx.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://svr.gzhubu.top

[K07] 进制转换
来源：http://djj.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yma.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yts.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hln.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vsd.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bbe.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://thh.snrcjt.cn


<!-- 参考信息 -->