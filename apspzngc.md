代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://qvh.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uho.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://eub.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://oew.bbcook.cn

[H03] 主动抛出异常
来源：http://tpx.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://zgu.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sgy.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://pfr.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://eeh.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://shc.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tgk.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rih.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://wdr.316326.xyz

[H04] 自定义异常类型
来源：http://yac.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://xjq.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hfi.birdmap.top

JS:   class MyError extends Error {}
来源：http://elr.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://uqp.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://kmv.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rol.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://vgy.yvedp.cn

C#:   class MyException : Exception {}
来源：http://ejd.52xcode.cn

[H05] 捕获特定类型
来源：http://psk.jinqigfzy.top

Py:   except ValueError as e:
来源：http://bci.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xzx.xinyue.icu

JS:   if (e instanceof TypeError) {}
来源：http://fdd.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://lxo.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://tkz.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bhc.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://dki.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qah.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://mqm.guannengcc.top

Py:   value = d.get("k") or default
来源：http://bhw.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yrg.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://mwm.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://wsp.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ywd.yonumen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qny.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://kvp.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://rkc.iojbl.cn

[H07] 断言
来源：http://erp.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://ezr.gogol.net.cn

PHP:  assert($x > 0);
来源：http://qhv.meibo888.top

JS:   console.assert(x > 0);
来源：http://kux.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://cel.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://rrs.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fci.xuetiantiany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dby.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://uqs.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://cqr.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://moa.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pph.ppjwa.cn

JS:   e.message;  e.stack
来源：http://pki.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kei.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zpv.fktsv.cn

Go:   err.Error()
来源：http://vpu.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://gll.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://tcd.chenzaomai.com

[H09] 带错误码的异常
来源：http://jxe.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pgy.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://agh.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tsw.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://njk.cashguo.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zgu.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zqg.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fwm.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ktk.nanxinkj.top

[H10] 资源自动释放
来源：http://vuu.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aoz.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fmm.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ecp.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qhh.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://poi.fzhhl.top

Go:   defer f.Close()
来源：http://gri.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jlk.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://niq.zdbjq.cn

================================================================================
来源：http://anf.tarul.cn

I. 正则表达式
来源：http://jjh.zdbjq.cn

================================================================================
来源：http://dtn.dashuyun.cn

[I01] 判断是否匹配
来源：http://fpx.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tgk.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://moj.ivvv.top

JS:   /\d+/.test(s)
来源：http://xww.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://yzt.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vdu.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pao.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://qug.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bsj.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://xqf.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://jjf.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wrt.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mcg.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://ogm.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hnb.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fbn.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://odm.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mvz.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://pal.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hqz.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xvg.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dfr.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gtn.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eyc.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yas.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://igc.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gng.sweek.top

[I04] 正则替换
来源：http://ewa.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sww.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uyp.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://jas.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://elo.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sfl.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zqp.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ucc.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rei.hnxiangtu.top

[I05] 按正则拆分
来源：http://ztu.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://rpg.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jat.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://qvs.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://zox.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://pkk.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://shb.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://qgs.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vmq.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dwj.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gjv.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eiy.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://src.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rso.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dhy.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tpg.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pei.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oev.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://qmm.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://plo.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tcc.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ale.zhixingplan.top

TS:   /error/gim
来源：http://aqf.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gud.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zed.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://umn.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pif.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://ljp.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ulk.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jvl.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xjb.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fig.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://psk.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vnk.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iab.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kon.ctjpmb.com

================================================================================
来源：http://tkp.ybcxt.top

J. 日期与时间
来源：http://oyt.epnwcf.com

================================================================================
来源：http://aja.ppjwa.cn

[J01] 获取当前时间
来源：http://jcy.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://umx.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iap.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://afu.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://okz.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tak.hongshengwenyu.top

Go:   time.Now()
来源：http://bzh.vehdjk.com

Ruby: Time.now
来源：http://xqy.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://stj.iojbl.cn

[J02] 格式化输出
来源：http://imk.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dyq.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://btq.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kba.nwbrower.top

TS:   d.toISOString()
来源：http://vjy.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sdj.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfm.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ggk.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jib.yj20258.top

[J03] 字符串解析为日期
来源：http://jyi.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nnm.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zgt.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://yjz.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://yix.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://cll.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rti.snrcjt.cn

Ruby: Date.parse("2024-01-02")
来源：http://hho.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kta.wangdashe.top

[J04] 时间戳与日期互转
来源：http://cxv.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yfk.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccy.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vwr.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bys.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lxx.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cfm.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gob.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hgf.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://ihl.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://ihq.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://uwh.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jim.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dfc.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://vax.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rpo.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://pql.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://gsz.vqdsnc.cn

[J06] 计算两时间之差
来源：http://bxg.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://tbc.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://kvb.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wmh.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dkx.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hca.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://fqi.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://sdi.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://uan.jianghu66.top

[J07] 比较两个日期
来源：http://hig.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://snl.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bhn.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://qet.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://koi.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mta.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ums.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mws.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://eli.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://aaf.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fca.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://knj.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ntq.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cix.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://owl.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pij.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zri.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lqk.0kj1m.cn

[J09] 时区处理
来源：http://uok.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fyu.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mln.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lcl.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bhp.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qru.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mdl.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://otb.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://slu.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://dww.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://aiq.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://whf.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lll.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ayc.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bfb.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fzz.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://syz.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ikc.havefunace.top

================================================================================
来源：http://xnx.daxiang520.top

K. JSON 与序列化
来源：http://jrs.c1oappe.top

================================================================================
来源：http://huf.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://hlq.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dpe.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gqr.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://edl.havefunace.top

TS:   JSON.stringify(obj)
来源：http://gsi.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ecg.fengsongda.top

Go:   json.Marshal(obj)
来源：http://cpl.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://wbg.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zua.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://twj.wangshuangyany.cn

Py:   json.loads(s)
来源：http://bpk.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cxn.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://tpz.cdnleiting.top

TS:   JSON.parse(s)
来源：http://pjq.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://brk.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://why.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://utk.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lti.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://phk.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://llb.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kqd.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://skw.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nik.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jll.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zgl.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://hik.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lbn.meibo888.top

[K04] 读取 JSON 文件
来源：http://hbp.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://irt.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ard.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rft.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://veu.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://htj.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mkg.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gdi.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mbb.gaohongyu789.top

[K05] 深拷贝对象
来源：http://srh.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://ldp.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://bof.yonumen.top

JS:   structuredClone(obj)
来源：http://rhm.epnwcf.com

TS:   structuredClone(obj)
来源：http://kwk.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qmc.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://svx.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ebv.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hwh.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://pmk.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fru.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lhh.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://luc.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lex.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hno.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tqi.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ypk.hnqzz.top


<!-- 参考信息 -->