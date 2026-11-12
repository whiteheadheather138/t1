代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://rin.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lfe.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://noj.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://twp.nwbrower.top

[H03] 主动抛出异常
来源：http://zjv.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://lyq.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yez.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://fgc.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://woa.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kgr.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yjg.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ads.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://fyg.ivvv.top

[H04] 自定义异常类型
来源：http://pvv.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://hmk.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yin.guannengcc.top

JS:   class MyError extends Error {}
来源：http://grf.xinyue.icu

TS:   class MyError extends Error {}
来源：http://fse.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://jlr.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vff.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://trr.xuanzx.com

C#:   class MyException : Exception {}
来源：http://vqx.vehdjk.com

[H05] 捕获特定类型
来源：http://hjl.cashguo.top

Py:   except ValueError as e:
来源：http://mek.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eia.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://zpt.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://ozi.nwbrower.top

Java: catch (IOException | SQLException e) {}
来源：http://smj.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hoo.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://cau.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gcl.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://hwu.yj20258.top

Py:   value = d.get("k") or default
来源：http://ymm.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ono.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://chr.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vul.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cov.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vrz.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://sfn.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://clz.zdqjudy.top

[H07] 断言
来源：http://rgi.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://zey.shuidangran.top

PHP:  assert($x > 0);
来源：http://izz.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://xnw.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://ppt.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://mpc.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kwo.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vmx.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://scf.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://usb.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://xrs.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rvx.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://nkm.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qdz.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cgx.tanke756.top

Go:   err.Error()
来源：http://vtu.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://irw.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://snn.ydzc1.top

[H09] 带错误码的异常
来源：http://nxy.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wyu.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ltd.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://voi.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jpb.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pzb.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lzp.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://pie.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lql.yanxiufei.cn

[H10] 资源自动释放
来源：http://fnk.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zwe.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ush.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lpd.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fcw.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vsa.zhongyouzk.top

Go:   defer f.Close()
来源：http://jvp.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzi.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uno.meibo888.top

================================================================================
来源：http://jgj.cqqwz.cn

I. 正则表达式
来源：http://pba.hywenlv.cn

================================================================================
来源：http://aey.sjlbkw.cn

[I01] 判断是否匹配
来源：http://nat.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tpd.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://utl.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://auk.tanke756.top

TS:   /\d+/.test(s)
来源：http://zag.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zog.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tqv.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://vlh.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://plz.yangfankeji.com

[I02] 提取所有匹配
来源：http://gzx.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://mle.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://etu.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mml.cashguo.top

TS:   s.match(/\d+/g)
来源：http://tbx.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dwk.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ynr.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://ioi.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ktv.sufxvd.cn

[I03] 提取捕获分组
来源：http://xli.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ugj.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qye.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://caj.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://idl.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ukd.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gsb.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yun.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ghn.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://pma.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qhn.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gde.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://nrx.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://wno.iojbl.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gvq.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ipz.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sah.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://heg.tianlin.xyz

[I05] 按正则拆分
来源：http://nsr.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gpj.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hpu.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://vbl.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://cze.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://mni.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ldi.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://avg.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vyc.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://psf.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wfv.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wbc.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kwl.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nds.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wqj.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ewb.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ewb.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wsr.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://uip.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wpn.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sbh.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://khk.chenlongwang.top

TS:   /error/gim
来源：http://str.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://npj.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xsm.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://ujl.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jfs.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://ayw.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://szc.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nml.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gcv.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxo.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fgk.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qwu.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wcy.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ejh.jinqigfzy.top

================================================================================
来源：http://rxk.tarul.cn

J. 日期与时间
来源：http://wfp.jyoumei.cn

================================================================================
来源：http://hfl.xylfe.cn

[J01] 获取当前时间
来源：http://ude.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://cvs.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wys.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://lrj.zycfv.cn

TS:   new Date();  Date.now()
来源：http://inm.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cny.hesvh.cn

Go:   time.Now()
来源：http://vfm.zhijiandao.cn

Ruby: Time.now
来源：http://rbv.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sjx.jinghuilouyu.cn

[J02] 格式化输出
来源：http://yxx.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vgj.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jmt.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fls.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://ibd.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xuf.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zjc.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlu.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gjs.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://hex.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xud.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tck.ivvv.top

JS:   new Date("2024-01-02")
来源：http://que.uphjek.com

TS:   new Date("2024-01-02")
来源：http://ckb.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jqp.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oba.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://gxi.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cph.guowangkeji.top

[J04] 时间戳与日期互转
来源：http://qcz.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rcl.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hwh.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://msw.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lzm.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xpo.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://msn.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sou.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qjk.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://zlo.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://omp.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kqk.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jru.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gep.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://bod.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lyv.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://lxh.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hxe.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://jfj.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://ffw.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://ohg.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mnz.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ysq.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uds.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://tkt.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://mnx.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://sdv.redwolf501.top

[J07] 比较两个日期
来源：http://kyt.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://pcw.fengsongda.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gwh.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://wcr.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://jap.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xwd.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ijs.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://fbx.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://nuf.ydzc1.top

[J08] 提取年月日与星期
来源：http://xex.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://owo.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://amf.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xsk.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qmn.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kbj.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://djc.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kbu.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rmb.hfpthk.cn

[J09] 时区处理
来源：http://klp.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zow.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://spy.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ieg.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dbn.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gzk.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sgh.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mof.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rnm.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://gct.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uup.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lfm.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ems.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qfh.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xxx.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xgy.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://krp.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.yj20258.top

================================================================================
来源：http://wbd.snrcjt.cn

K. JSON 与序列化
来源：http://cnv.cucudq.cn

================================================================================
来源：http://nve.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://yaq.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://phc.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://faz.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://xdx.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://qsq.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jll.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://zug.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://wtt.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vfm.iojbl.cn

[K02] JSON 字符串转对象
来源：http://znn.bjfxy.top

Py:   json.loads(s)
来源：http://wtk.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gtl.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://xbv.dashuyun.cn

TS:   JSON.parse(s)
来源：http://gmm.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bom.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://ioo.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://jut.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xnt.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://cmy.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cdt.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tpn.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wih.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://xwo.bjfxy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://apy.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gta.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://xna.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qoa.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://fhb.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vru.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kxl.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hop.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vag.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kzc.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bka.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jew.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://euz.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://mlw.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://hms.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://gkw.hysaishi.cn

JS:   structuredClone(obj)
来源：http://wxi.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://msp.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zmy.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sls.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bbc.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qrx.fzhhl.top

[K06] 解析 URL 查询串
来源：http://qxy.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://abb.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rob.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wqp.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdf.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uaf.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ztd.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://scv.pengpengdd.cyou


<!-- 参考信息 -->