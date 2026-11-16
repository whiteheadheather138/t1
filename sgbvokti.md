代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fsn.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rcu.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lwj.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://oct.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://ove.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dnn.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lte.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dit.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://cwm.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ska.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tdt.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jnc.yvedp.cn

[H03] 主动抛出异常
来源：http://fwv.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://tfc.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zpa.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://mdt.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://rnn.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://idl.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ssq.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bji.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://kjm.sxryk.cn

[H04] 自定义异常类型
来源：http://scy.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://ndd.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fcs.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://mgw.ydzc1.top

TS:   class MyError extends Error {}
来源：http://zar.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://edg.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jao.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://tft.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://mli.fehbvm.com

[H05] 捕获特定类型
来源：http://nek.guowangkeji.top

Py:   except ValueError as e:
来源：http://gkp.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fpo.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://teu.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://xar.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://rlj.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vfu.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://jyg.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://osp.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://qvr.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://qiy.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://upk.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://lcr.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nce.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xzk.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qom.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://zzx.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://tkq.aizwys.cn

[H07] 断言
来源：http://bti.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://xvh.ctjpmb.com

PHP:  assert($x > 0);
来源：http://rwi.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://kla.shuidangran.top

TS:   console.assert(x > 0);
来源：http://saw.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://mmk.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://klc.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://uzb.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://ikp.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://swh.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://hyj.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rqs.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://qhs.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cvc.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sok.dianchejie.cn

Go:   err.Error()
来源：http://syp.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://mmo.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://mhk.dianchejie.cn

[H09] 带错误码的异常
来源：http://csx.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://orh.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tpq.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qmf.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qpt.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fzg.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zru.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://beb.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vqf.tianlin.xyz

[H10] 资源自动释放
来源：http://dji.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yho.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tpj.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jrm.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vuu.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zpv.yfazqb.com

Go:   defer f.Close()
来源：http://hip.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bau.jinyuanbaomall.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dlx.jinqigfzy.top

================================================================================
来源：http://edo.xuanzx.com

I. 正则表达式
来源：http://kei.jyoumei.cn

================================================================================
来源：http://mvp.ppjwa.cn

[I01] 判断是否匹配
来源：http://hzl.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ubn.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://cpb.vehdjk.com

JS:   /\d+/.test(s)
来源：http://wfr.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://uei.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sdp.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://odq.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://pec.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hqz.sufxvd.cn

[I02] 提取所有匹配
来源：http://yfk.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://jgp.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wkb.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ogk.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://klo.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vsy.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lfh.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://wmi.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ghs.c1oappe.top

[I03] 提取捕获分组
来源：http://qur.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qoa.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xqr.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sud.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tqd.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gvi.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uhd.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://teh.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kvo.nwbrower.top

[I04] 正则替换
来源：http://nha.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://duv.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tqk.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jsg.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bnc.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tyl.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hpp.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pmb.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eyi.dashuyun.cn

[I05] 按正则拆分
来源：http://vmv.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://roa.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tko.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://rim.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://ved.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://ufw.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://obc.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ata.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ibl.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wgk.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://scw.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hrg.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://osv.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vwz.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jwu.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dtj.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jak.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vaf.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://nkt.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bif.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://suq.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://goc.dianchejie.cn

TS:   /error/gim
来源：http://uoo.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aej.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xxi.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://xgq.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cme.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://vup.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://alj.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://poz.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iez.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dac.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fgi.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lgr.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fve.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dlu.haohaochexian.top

================================================================================
来源：http://vvq.wangshuangyany.cn

J. 日期与时间
来源：http://eok.snrcjt.cn

================================================================================
来源：http://bjl.cheryme.top

[J01] 获取当前时间
来源：http://ztc.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jrs.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rrd.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://hbe.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://cfa.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://asm.daria6918.cn

Go:   time.Now()
来源：http://afs.jinyuanbaomall.cn

Ruby: Time.now
来源：http://htu.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zsl.hesvh.cn

[J02] 格式化输出
来源：http://zsz.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ath.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zvu.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kmx.andypj.xyz

TS:   d.toISOString()
来源：http://zks.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rvt.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hlx.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pmv.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oiv.xuanzx.com

[J03] 字符串解析为日期
来源：http://lbq.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zpg.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://clt.uphjek.com

JS:   new Date("2024-01-02")
来源：http://vnx.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://wai.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aip.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cln.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://gvv.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ijm.yueranfly.top

[J04] 时间戳与日期互转
来源：http://uts.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pev.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nhc.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xix.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ocs.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awr.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ttw.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://agq.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://khc.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://rik.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://ycy.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bxc.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dju.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zhh.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://oph.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uem.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://ixi.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://qgz.jqgufenzy.top

[J06] 计算两时间之差
来源：http://jag.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://zqv.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://jsh.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vqk.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wrd.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://rwf.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://hcw.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://cel.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://vas.yj20258.top

[J07] 比较两个日期
来源：http://mwo.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://oui.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pwo.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mdt.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://ahf.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wjg.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bbt.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://aew.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://exx.zhongyouzk.top

[J08] 提取年月日与星期
来源：http://jdj.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cot.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nlv.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://add.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uui.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bue.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cxo.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eso.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://odd.hysaishi.cn

[J09] 时区处理
来源：http://sua.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ifa.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://otn.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvm.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rbh.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aey.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yol.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dwg.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mla.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://sya.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pmt.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bfw.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cjg.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lxn.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sjk.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://atn.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zve.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sfb.yfazqb.com

================================================================================
来源：http://ker.jlsjyb.cn

K. JSON 与序列化
来源：http://bte.mhx1999.top

================================================================================
来源：http://vqy.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://hbz.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kkc.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vvt.hammf.cn

JS:   JSON.stringify(obj)
来源：http://egc.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://wnd.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://new.xziqi.cn

Go:   json.Marshal(obj)
来源：http://dmx.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jnx.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vnr.zycfv.cn

[K02] JSON 字符串转对象
来源：http://tgp.haohaochexian.top

Py:   json.loads(s)
来源：http://qhm.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qhu.uphjek.com

JS:   JSON.parse(s)
来源：http://zzc.uphjek.com

TS:   JSON.parse(s)
来源：http://jrc.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uvu.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://voi.sysykeji.top

Ruby: JSON.parse(s)
来源：http://qqh.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nta.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://sqf.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rpp.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xyc.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gsf.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pgj.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dea.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hsg.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://bsn.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gqr.yfazqb.com

[K04] 读取 JSON 文件
来源：http://qro.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zgz.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jtu.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mlv.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rlu.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pvj.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dyd.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pom.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rsg.birdmap.top

[K05] 深拷贝对象
来源：http://qyv.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://log.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://wbv.cheryme.top

JS:   structuredClone(obj)
来源：http://hdz.cheryme.top

TS:   structuredClone(obj)
来源：http://qmg.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uim.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://trs.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rgx.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vlo.hfpthk.cn


<!-- 参考信息 -->