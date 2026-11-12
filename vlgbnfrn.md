代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://wpx.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://trl.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fyv.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mlx.mhx1999.top

[H03] 主动抛出异常
来源：http://gsq.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://wgb.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ial.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://wsp.cashguo.top

TS:   throw new Error("错误信息");
来源：http://rkp.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aoj.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oyg.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bxb.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://juo.sxryk.cn

[H04] 自定义异常类型
来源：http://ssf.316326.xyz

Py:   class MyError(Exception): pass
来源：http://pot.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zrw.yfazqb.com

JS:   class MyError extends Error {}
来源：http://dbj.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://aru.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://ijs.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aqn.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://aih.tian-w.cn

C#:   class MyException : Exception {}
来源：http://zdz.ppjwa.cn

[H05] 捕获特定类型
来源：http://stj.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://ifw.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mgb.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://wpr.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://kuw.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://uty.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mvw.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://cgf.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gfe.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://xbj.fengsongda.top

Py:   value = d.get("k") or default
来源：http://kob.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sjp.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://mjg.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://qqf.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vio.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://tlf.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://sew.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://mig.feifeiyinyue.top

[H07] 断言
来源：http://nxi.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://yce.cucudq.cn

PHP:  assert($x > 0);
来源：http://zmu.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://nrc.yj20258888.top

TS:   console.assert(x > 0);
来源：http://rgy.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://hag.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tag.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://itn.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://csk.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://ybt.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://pcq.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uxn.jyoumei.cn

JS:   e.message;  e.stack
来源：http://qmq.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zzc.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ozd.shanyushiyangkeji.top

Go:   err.Error()
来源：http://byq.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://zmg.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://rbe.cucudq.cn

[H09] 带错误码的异常
来源：http://jns.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vdm.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sho.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://try.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lyt.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://asv.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qsc.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://xnx.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kzy.havefunace.top

[H10] 资源自动释放
来源：http://mgl.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yjq.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://njk.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qyf.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gxn.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pwc.haohaochexian.top

Go:   defer f.Close()
来源：http://bea.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uiz.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xka.52xcode.cn

================================================================================
来源：http://yuj.kuanghao11.cn

I. 正则表达式
来源：http://ael.smart0.xyz

================================================================================
来源：http://tst.hnqzz.top

[I01] 判断是否匹配
来源：http://zih.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://way.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://otx.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://dxa.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://bdb.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lfx.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mpo.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://oat.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qxv.sufxvd.cn

[I02] 提取所有匹配
来源：http://lhr.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://ams.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://edw.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://clw.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://wiu.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lsg.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vef.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://cpc.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ajr.zhixingplan.top

[I03] 提取捕获分组
来源：http://tol.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tqt.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ygq.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://beg.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jux.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mik.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sxw.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gnn.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xsn.shanyushiyangkeji.top

[I04] 正则替换
来源：http://dmu.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aii.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xbn.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://qmn.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://afb.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://mwb.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pvb.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pgz.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ils.yfazqb.com

[I05] 按正则拆分
来源：http://ndo.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sjk.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fgd.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://trt.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://iuy.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://hvy.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bxx.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ipo.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://brq.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://woh.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lom.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bju.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yap.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bls.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dya.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zkg.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://adl.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iyw.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://pfn.0kj1m.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jwn.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xqa.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fdq.xylfe.cn

TS:   /error/gim
来源：http://poq.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ueu.zhaomingkeji.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uyg.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://thn.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://trw.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://gfq.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hdk.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gfv.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkb.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cvk.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ela.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hps.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://acg.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ytg.yj20258.top

================================================================================
来源：http://aje.cheryme.top

J. 日期与时间
来源：http://ifd.c1oappe.top

================================================================================
来源：http://iin.quarkkingdee.top

[J01] 获取当前时间
来源：http://ysc.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tkc.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ldb.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://wzh.fzhhl.top

TS:   new Date();  Date.now()
来源：http://hdr.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ooc.pycfn.com

Go:   time.Now()
来源：http://rkp.smart0.xyz

Ruby: Time.now
来源：http://zmy.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zhg.fengsongda.top

[J02] 格式化输出
来源：http://grg.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tbl.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gkw.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rqv.fktsv.cn

TS:   d.toISOString()
来源：http://vcn.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vpt.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mhk.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbm.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hib.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://yyd.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gyz.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fwz.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://kkm.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://ouo.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://vsd.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lnq.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://jcm.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ysh.pycfn.com

[J04] 时间戳与日期互转
来源：http://bax.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vej.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rgx.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xnr.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cce.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qnt.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jku.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://twt.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xnj.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://uhl.yongpay.top

Py:   now + timedelta(days=7)
来源：http://jso.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://log.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ols.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qnh.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://wph.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bib.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://waj.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://srl.haohaochexian.top

[J06] 计算两时间之差
来源：http://ugg.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://vib.sweek.top

PHP:  $end->diff($start)->days;
来源：http://gpd.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cxn.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vjg.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://pwd.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://eqr.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://vmt.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://lja.ydzc1.top

[J07] 比较两个日期
来源：http://ivd.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://xuz.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nae.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://igc.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://boj.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://adn.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nzq.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://kod.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://zaf.zdbjq.cn

[J08] 提取年月日与星期
来源：http://ywz.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dhs.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ykv.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jjl.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mno.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dot.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://slv.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rch.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ntj.smart0.xyz

[J09] 时区处理
来源：http://heb.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aif.yueranfly.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cjk.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zrc.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tom.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xpu.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zxo.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://cva.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nih.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://ugn.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yvf.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qrk.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tmb.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://haq.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tzs.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tbf.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xgw.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cnt.zhongyouzk.top

================================================================================
来源：http://qgx.gaohongyu789.top

K. JSON 与序列化
来源：http://yxz.zhijiandao.cn

================================================================================
来源：http://ijy.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://hpg.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pwz.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bzf.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://weh.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://hjo.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mip.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://xrc.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://dhf.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://tps.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://ddt.hongshengwenyu.top

Py:   json.loads(s)
来源：http://tlr.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ugi.xziqi.cn

JS:   JSON.parse(s)
来源：http://mic.vehdjk.com

TS:   JSON.parse(s)
来源：http://amc.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lso.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://kbo.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://pla.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://glh.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://icr.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ltx.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lvl.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uth.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vtt.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bdt.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hgq.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://pls.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oyj.yj202588.top

[K04] 读取 JSON 文件
来源：http://xzi.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ztk.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bkn.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dcm.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hnx.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sjd.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nan.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfz.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ydf.gzhubu.top

[K05] 深拷贝对象
来源：http://vnr.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://vvp.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://whe.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://cuw.ivvv.top

TS:   structuredClone(obj)
来源：http://udd.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zdp.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nbt.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gcv.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://czq.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://bbp.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bsy.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qjs.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zon.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hqb.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pna.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xmm.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eyc.xinyue.icu


<!-- 参考信息 -->