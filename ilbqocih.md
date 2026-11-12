代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://vaj.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bii.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ujy.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://omp.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://xms.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cfm.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xpo.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fpy.cucudq.cn

[H03] 主动抛出异常
来源：http://mdw.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://jqm.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ias.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://nmm.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://hoy.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xzv.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ubc.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fjj.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://cqn.tarul.cn

[H04] 自定义异常类型
来源：http://hfj.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://iuc.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://pju.zycfv.cn

JS:   class MyError extends Error {}
来源：http://nqc.fengsongda.top

TS:   class MyError extends Error {}
来源：http://lcg.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://ywz.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fmx.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://ejt.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://udm.cheryme.top

[H05] 捕获特定类型
来源：http://amt.guannengcc.top

Py:   except ValueError as e:
来源：http://lxz.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pxo.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://yli.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://ufk.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://qee.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iyc.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://nyz.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kdz.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://tbv.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://ifu.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sop.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://len.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://qrm.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://grj.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://vlu.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://pmx.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://vax.wangshuangyany.cn

[H07] 断言
来源：http://oru.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://tmo.yongpay.top

PHP:  assert($x > 0);
来源：http://vec.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://xye.guannengcc.top

TS:   console.assert(x > 0);
来源：http://emm.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://shc.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ara.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rtp.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://uno.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://syf.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://act.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ggv.redwolf501.top

JS:   e.message;  e.stack
来源：http://hlt.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://geq.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://xvy.yangfankeji.com

Go:   err.Error()
来源：http://gpk.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://ygb.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://ukd.yuxming.cn

[H09] 带错误码的异常
来源：http://svg.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://txa.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hfv.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://txa.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xpz.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://spk.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://glh.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://bla.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://srf.gotoacloud.top

[H10] 资源自动释放
来源：http://vfi.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://tfo.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vgz.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://naa.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jui.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gzt.epnwcf.com

Go:   defer f.Close()
来源：http://xqp.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cku.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ulx.iojbl.cn

================================================================================
来源：http://pdi.smart0.xyz

I. 正则表达式
来源：http://okm.dashuyun.cn

================================================================================
来源：http://sew.yj20258888.top

[I01] 判断是否匹配
来源：http://rif.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mvj.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://zrs.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://ort.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://bpi.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jsz.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dln.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://uvn.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://flu.ydzc1.top

[I02] 提取所有匹配
来源：http://vcm.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://ymf.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dfo.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oyd.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://cxc.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mkr.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aep.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://isy.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tcj.bjfxy.top

[I03] 提取捕获分组
来源：http://ssq.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xpn.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tkj.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kvn.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xgy.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bpk.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zwe.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ocl.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bjy.ydzc1.top

[I04] 正则替换
来源：http://oyc.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bzs.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xus.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://rbh.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://zzi.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nja.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://vwy.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fjw.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://chh.sufxvd.cn

[I05] 按正则拆分
来源：http://oib.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://atq.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://elt.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://oyo.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://iba.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://yok.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cer.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://kps.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oyu.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tti.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xfp.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mml.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdw.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxt.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rqh.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xzh.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://spg.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hkq.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://vuv.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ftj.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wdo.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eir.yangfankeji.com

TS:   /error/gim
来源：http://lpu.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dpt.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ybi.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://taq.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pxv.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://bdd.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ybg.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eka.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ett.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hln.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://owi.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vcp.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qhn.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gnz.xinyue.icu

================================================================================
来源：http://wkp.hfpthk.cn

J. 日期与时间
来源：http://cng.gaohongyu789.top

================================================================================
来源：http://dhl.nanxinkj.top

[J01] 获取当前时间
来源：http://koc.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fyf.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wrp.gzhubu.top

JS:   new Date();  Date.now()
来源：http://apa.aizwys.cn

TS:   new Date();  Date.now()
来源：http://dar.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ivm.xuanzx.com

Go:   time.Now()
来源：http://rdi.chenlongwang.top

Ruby: Time.now
来源：http://yoo.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lmx.snrcjt.cn

[J02] 格式化输出
来源：http://gmx.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iga.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cmg.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oao.mhx1999.top

TS:   d.toISOString()
来源：http://dfm.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://csp.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ltt.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://knd.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iqa.jqgfzy.top

[J03] 字符串解析为日期
来源：http://gzm.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bnt.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rkd.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://tnv.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://smy.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://mzn.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bzj.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://wnn.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dtz.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://lfk.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wrn.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pud.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dkd.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eld.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cad.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rci.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nie.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ufo.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://vdc.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://rlb.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://err.yfazqb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://him.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://clw.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://wes.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://atx.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://obk.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://knj.ehwqpu.com

[J06] 计算两时间之差
来源：http://ngv.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://ehc.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://fbd.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mop.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uvs.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gwa.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://stt.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://rej.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://fyk.snrcjt.cn

[J07] 比较两个日期
来源：http://gcx.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://brk.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ydp.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://uob.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://qrf.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lkv.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xyt.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ayi.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://din.c1oappe.top

[J08] 提取年月日与星期
来源：http://mou.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oaa.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xat.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zhd.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xhs.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fve.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fbl.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rqt.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xxf.nwbrower.top

[J09] 时区处理
来源：http://iaa.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jfu.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://phh.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jeg.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emy.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ztx.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xfq.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oul.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uzz.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://hei.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hfz.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://crf.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jzr.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wgd.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rnx.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wor.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nyg.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ymz.xuanzx.com

================================================================================
来源：http://zyv.tian-w.cn

K. JSON 与序列化
来源：http://cbk.sjlbkw.cn

================================================================================
来源：http://dca.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://wnj.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ptj.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eyt.meibo888.top

JS:   JSON.stringify(obj)
来源：http://jrh.havefunace.top

TS:   JSON.stringify(obj)
来源：http://wft.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zpf.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://jlq.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cez.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://noa.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://vgr.fzhhl.top

Py:   json.loads(s)
来源：http://vxk.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dcp.cucudq.cn

JS:   JSON.parse(s)
来源：http://hcm.wangdashe.top

TS:   JSON.parse(s)
来源：http://vvh.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://spj.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://hkq.yj20258888.top

Ruby: JSON.parse(s)
来源：http://kxx.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dqc.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://wdi.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gsq.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tjy.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fqq.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mea.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://thd.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cwf.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://ifp.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://snd.fzhhl.top

[K04] 读取 JSON 文件
来源：http://kkk.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xbq.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cvi.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rno.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nyn.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aws.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uxb.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://jbr.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://efc.nanxuanxn.top

[K05] 深拷贝对象
来源：http://cqb.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://qiw.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://ouw.cashguo.top

JS:   structuredClone(obj)
来源：http://ljo.tanke756.top

TS:   structuredClone(obj)
来源：http://svg.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hxl.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fic.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dne.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bmm.zycfv.cn

[K06] 解析 URL 查询串
来源：http://yrr.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gox.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bmi.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpa.yj20258888.top


<!-- 参考信息 -->