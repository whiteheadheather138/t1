代发 wailian999

[H03] 主动抛出异常
来源：http://dkg.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://yhn.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hlx.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://pih.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://wvk.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://epy.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fya.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ish.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://vln.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://yty.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://qyc.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ccr.shuidangran.top

JS:   class MyError extends Error {}
来源：http://fpn.smart0.xyz

TS:   class MyError extends Error {}
来源：http://ukh.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://wre.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zek.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://tba.daria6918.cn

C#:   class MyException : Exception {}
来源：http://ixs.daxiang520.top

[H05] 捕获特定类型
来源：http://bbv.yangfankeji.com

Py:   except ValueError as e:
来源：http://anu.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://apk.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://tku.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://fmr.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://ggs.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uuz.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://rqj.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lpd.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://vvx.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://osx.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://huu.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jky.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://hoy.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://srd.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vda.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://lsp.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://oes.ppjwa.cn

[H07] 断言
来源：http://dit.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://mww.haohaochexian.top

PHP:  assert($x > 0);
来源：http://kdw.andypj.xyz

JS:   console.assert(x > 0);
来源：http://fuc.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://juf.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://qlg.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gvu.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://yen.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://hah.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://ktt.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://poi.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://spt.svipenyu.cn

JS:   e.message;  e.stack
来源：http://suo.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kwo.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vim.jinyuanbaomall.cn

Go:   err.Error()
来源：http://pun.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://ske.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://mbh.aizwys.cn

[H09] 带错误码的异常
来源：http://qxe.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fey.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rho.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xkl.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://udd.nwbrower.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sxu.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vgw.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eef.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gle.daxiang520.top

[H10] 资源自动释放
来源：http://zqt.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hwk.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://him.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://smr.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kvi.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vya.fengsongda.top

Go:   defer f.Close()
来源：http://vfd.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dul.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bso.yfazqb.com

================================================================================
来源：http://nhd.cdnleiting.top

I. 正则表达式
来源：http://fpq.fktsv.cn

================================================================================
来源：http://ljb.nanxinkj.top

[I01] 判断是否匹配
来源：http://yzt.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nqb.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fyb.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://jai.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://gvl.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yvn.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nbn.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://arv.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ptj.hesvh.cn

[I02] 提取所有匹配
来源：http://ibx.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://ted.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://odg.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://akp.yj202588.top

TS:   s.match(/\d+/g)
来源：http://zus.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kqb.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mhm.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://pet.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://omk.yanxiufei.cn

[I03] 提取捕获分组
来源：http://dyf.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ztp.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ldr.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ico.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mae.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nwa.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rbq.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://whm.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hbz.redwolf501.top

[I04] 正则替换
来源：http://cez.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wne.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://imu.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://amx.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kan.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://pia.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zov.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://usf.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://knv.316326.xyz

[I05] 按正则拆分
来源：http://prf.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bjm.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wms.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://hlk.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://moj.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://tkk.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lif.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://lkk.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bjl.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mxs.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://frc.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mqt.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzc.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lwj.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jdz.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jdw.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qsv.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yzj.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://yqm.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://moy.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dyq.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ztq.zdqjudy.top

TS:   /error/gim
来源：http://foi.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tbl.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kyc.316326.xyz

Ruby: s.scan(/error/i)
来源：http://lif.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pfr.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://qof.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ojj.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qdl.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://avk.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://csr.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://pvr.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yqs.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hfc.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dbu.jqgfzy.top

================================================================================
来源：http://hqp.nanxinkj.top

J. 日期与时间
来源：http://lgl.feifeiyinyue.top

================================================================================
来源：http://sdj.sufxvd.cn

[J01] 获取当前时间
来源：http://izr.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://une.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://btl.xinyue.icu

JS:   new Date();  Date.now()
来源：http://zcx.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://zrg.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dxb.xinyue.icu

Go:   time.Now()
来源：http://bel.dashuyun.cn

Ruby: Time.now
来源：http://eqp.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lvy.hcnkem.com

[J02] 格式化输出
来源：http://vvx.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ozh.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://esc.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://meh.xuetiantiany.cn

TS:   d.toISOString()
来源：http://qcj.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lvs.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mko.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mhc.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yvj.daxiang520.top

[J03] 字符串解析为日期
来源：http://nfm.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ebq.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jnl.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://atp.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://aup.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://spz.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nig.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://afc.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mcv.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://qqe.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fes.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nwv.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://exc.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ool.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pjx.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ppo.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mwd.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aqg.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://vhs.cheryme.top

Py:   now + timedelta(days=7)
来源：http://bda.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vqq.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zxn.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zhu.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://yea.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iyd.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://bxs.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ubl.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://mcf.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://bri.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://ntf.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hbt.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://prc.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://raz.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://fpy.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://tkz.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://rym.vehdjk.com

[J07] 比较两个日期
来源：http://pgd.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://iep.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eml.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://tnr.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uji.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yug.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://amq.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://msi.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://gag.havefunace.top

[J08] 提取年月日与星期
来源：http://kgc.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wyb.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hfx.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dzc.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oxe.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qsb.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ufn.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://frz.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://byt.aibaodan.cn

[J09] 时区处理
来源：http://knh.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aui.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://twd.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rvh.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqh.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nap.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pry.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iyr.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://plk.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://rxg.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://icv.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hpa.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ikd.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ioa.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://shb.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gxu.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ajk.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kuv.gzhubu.top

================================================================================
来源：http://qpi.jinqigfzy.top

K. JSON 与序列化
来源：http://vyf.sufxvd.cn

================================================================================
来源：http://nxk.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://kdt.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://stx.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ihn.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://zvh.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://sut.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kwp.gzhubu.top

Go:   json.Marshal(obj)
来源：http://cdv.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://hsd.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rua.smart0.xyz

[K02] JSON 字符串转对象
来源：http://mww.zdqjudy.top

Py:   json.loads(s)
来源：http://xjf.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://shz.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://znd.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://nlg.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://luo.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://uvo.aizwys.cn

Ruby: JSON.parse(s)
来源：http://xdr.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hcw.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://xzn.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eyn.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cab.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://avh.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nxh.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qja.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qap.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wur.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gls.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://aet.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cuq.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yex.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jaf.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mnm.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vtl.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tpm.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://ann.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://van.hfpthk.cn

[K05] 深拷贝对象
来源：http://nol.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://etx.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://ovp.havefunace.top

JS:   structuredClone(obj)
来源：http://kyu.mhx1999.top

TS:   structuredClone(obj)
来源：http://suk.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ejy.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://anb.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sxd.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://jsx.yongpay.top

[K06] 解析 URL 查询串
来源：http://ccw.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sfp.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nra.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tsz.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zqy.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lng.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hdb.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zwv.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mic.gogol.net.cn

[K07] 进制转换
来源：http://xxp.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jxg.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://man.havefunace.top


<!-- 参考信息 -->