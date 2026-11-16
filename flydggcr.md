代发 wailian999

[H03] 主动抛出异常
来源：http://zfl.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://shw.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixl.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://abo.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://zaq.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://npe.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zfx.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vkp.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://vbh.hfpthk.cn

[H04] 自定义异常类型
来源：http://ajc.yongpay.top

Py:   class MyError(Exception): pass
来源：http://rst.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://dlh.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://izt.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://nus.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://isf.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aza.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://jus.guannengcc.top

C#:   class MyException : Exception {}
来源：http://llo.nanxuanxn.top

[H05] 捕获特定类型
来源：http://ruu.jianghu66.top

Py:   except ValueError as e:
来源：http://cji.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jfr.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://rnf.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://cno.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://qxp.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dpz.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://taz.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ita.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://sxn.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://kqi.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lfp.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://uhb.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://taq.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nmr.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tiu.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://ekg.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://jdh.0kj1m.cn

[H07] 断言
来源：http://jnx.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://cvz.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://qkw.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://nqp.jianghu66.top

TS:   console.assert(x > 0);
来源：http://hmr.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://lsf.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qoh.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://lvv.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://qho.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://fla.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://kuq.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jqr.ctjpmb.com

JS:   e.message;  e.stack
来源：http://kob.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ibi.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dvo.zdqjudy.top

Go:   err.Error()
来源：http://ymk.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://qhc.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://ouz.yuanzhike.top

[H09] 带错误码的异常
来源：http://pbh.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ydj.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rla.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bji.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xpe.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mmw.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zpv.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lck.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pdg.yanxiufei.cn

[H10] 资源自动释放
来源：http://smk.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eti.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tro.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tlv.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qqj.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://psx.zdqjudy.top

Go:   defer f.Close()
来源：http://nmv.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yfy.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qdt.ybcxt.top

================================================================================
来源：http://dcd.hnqzz.top

I. 正则表达式
来源：http://hnk.shuidangran.top

================================================================================
来源：http://lsm.jinqigufen.top

[I01] 判断是否匹配
来源：http://ucq.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rig.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jsu.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://siu.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://gbq.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://udy.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ikg.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://uml.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vra.svipenyu.cn

[I02] 提取所有匹配
来源：http://nri.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://tig.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sbz.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pox.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://qcy.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kus.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ahp.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://erd.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rdy.jiagoushi.top

[I03] 提取捕获分组
来源：http://kcq.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ajs.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uod.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://flv.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bjx.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wed.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hin.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hkl.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gam.wangshuangyany.cn

[I04] 正则替换
来源：http://ixj.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zwb.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iky.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://kpe.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jyv.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://naa.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zrd.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ltx.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vjs.wangshuangyany.cn

[I05] 按正则拆分
来源：http://fpb.kuanghao11.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fit.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gyf.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://try.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://qoz.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://cht.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pmr.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://suu.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hsw.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bhf.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bpd.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tio.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iyo.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mgl.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dvw.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vhd.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://niq.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yca.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://ijd.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fmk.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bap.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pfv.shzxlz.cn

TS:   /error/gim
来源：http://nan.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qgg.wangshuangyany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xso.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://sce.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mmh.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://dxi.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uss.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://upp.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qzl.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://acx.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://iiu.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dkq.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nyb.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tez.c1oappe.top

================================================================================
来源：http://ykz.jyoumei.cn

J. 日期与时间
来源：http://wws.ehwqpu.com

================================================================================
来源：http://lau.9152youxi.cn

[J01] 获取当前时间
来源：http://ows.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fmq.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fvz.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://tur.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://ftv.iojbl.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zlt.snrcjt.cn

Go:   time.Now()
来源：http://qrh.dashuyun.cn

Ruby: Time.now
来源：http://fvp.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vpc.gaohongyu789.top

[J02] 格式化输出
来源：http://uxq.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqn.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cfx.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://znf.smart0.xyz

TS:   d.toISOString()
来源：http://tto.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jnc.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pbk.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxv.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bcf.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://qxr.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://psb.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://smp.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://dga.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://tbx.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://vaq.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uiy.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://geb.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qcx.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://ryq.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baq.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://taz.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qxk.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hfb.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uie.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tdj.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://inp.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rti.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://zom.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://fnw.chenlongwang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vcr.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://glh.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqs.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://lsw.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uwx.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://cfe.0kj1m.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ivi.iojbl.cn

[J06] 计算两时间之差
来源：http://dob.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://gca.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://fwf.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ldb.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kbb.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://rab.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://lbd.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://mvc.yuxming.cn

C#:   (end - start).TotalSeconds
来源：http://cgh.fktsv.cn

[J07] 比较两个日期
来源：http://lvl.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ecy.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sky.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://lfb.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://nfy.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nfx.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qfq.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://tof.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://cmt.cdnleiting.top

[J08] 提取年月日与星期
来源：http://bkd.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ynf.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdb.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fpd.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wcf.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yto.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rnd.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ytd.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oqp.hammf.cn

[J09] 时区处理
来源：http://nmi.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wha.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pmm.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gft.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://azj.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bso.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xmh.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uij.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vgz.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://fyc.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fdl.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lnj.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bgv.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xap.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://whk.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fph.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zlk.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vsp.cashguo.top

================================================================================
来源：http://pap.sjlbkw.cn

K. JSON 与序列化
来源：http://lhv.yongpay.top

================================================================================
来源：http://ozi.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://hgc.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mte.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fsc.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://sxx.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://eay.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://znf.iojbl.cn

Go:   json.Marshal(obj)
来源：http://ohq.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://njj.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://irh.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://sex.tanke756.top

Py:   json.loads(s)
来源：http://vsx.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ftr.sufxvd.cn

JS:   JSON.parse(s)
来源：http://ddo.mhx1999.top

TS:   JSON.parse(s)
来源：http://eux.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wxj.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://ycv.fktsv.cn

Ruby: JSON.parse(s)
来源：http://xet.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aae.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://byn.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pzx.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fur.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ren.guowangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kzk.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jtc.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vxb.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mwt.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cna.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://jgh.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tnl.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ksr.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://agp.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nrt.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rbu.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pkj.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bsd.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hdz.smart0.xyz

[K05] 深拷贝对象
来源：http://zvu.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://fvc.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://zuw.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://guq.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://luk.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jrg.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jxa.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://waw.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hra.ivvv.top

[K06] 解析 URL 查询串
来源：http://qmz.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vfq.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wkd.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://twi.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqs.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://saf.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://djf.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dlq.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kwj.shanyushiyangkeji.top

[K07] 进制转换
来源：http://aom.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eyg.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oek.yj202588.top


<!-- 参考信息 -->