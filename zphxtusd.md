代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dcu.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tps.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dsb.shuidangran.top

[H02] finally / ensure 收尾
来源：http://jni.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://hri.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://hhc.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lmf.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qpg.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ygv.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://tbf.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zko.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aqz.jiagoushi.top

[H03] 主动抛出异常
来源：http://ytv.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://ser.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mpx.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://bap.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://gfn.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nxw.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kmt.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://zjn.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lsc.kuanghao11.cn

[H04] 自定义异常类型
来源：http://khf.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://mlz.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bcf.jianghu66.top

JS:   class MyError extends Error {}
来源：http://vif.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://uxb.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://uwq.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uxs.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://qon.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://dkr.hnxiangtu.top

[H05] 捕获特定类型
来源：http://rlg.yuxming.cn

Py:   except ValueError as e:
来源：http://vzo.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tnj.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://dip.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://rko.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://xpr.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fuo.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://maj.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ssp.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://rqw.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://sgf.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://hep.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qfv.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://kqy.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://whe.fengsongda.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kob.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://rwd.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://khk.ehwqpu.com

[H07] 断言
来源：http://fpk.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://dbj.vehdjk.com

PHP:  assert($x > 0);
来源：http://ube.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://qgi.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://srz.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://vlu.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xsj.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tbd.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://jvm.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://eag.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://jqc.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dwg.yvedp.cn

JS:   e.message;  e.stack
来源：http://eqk.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ymv.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sna.hysaishi.cn

Go:   err.Error()
来源：http://rgw.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://ryn.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://jex.iojbl.cn

[H09] 带错误码的异常
来源：http://efa.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cjp.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yvp.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lxl.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qnp.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dxt.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lwu.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zbs.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nwn.zdqjudy.top

[H10] 资源自动释放
来源：http://xxe.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qit.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nty.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vtd.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pya.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jtj.vehdjk.com

Go:   defer f.Close()
来源：http://enx.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ilz.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://prq.ctjpmb.com

================================================================================
来源：http://bcp.hammf.cn

I. 正则表达式
来源：http://vpz.fengsongda.top

================================================================================
来源：http://iuu.jiagoushi.top

[I01] 判断是否匹配
来源：http://nuo.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pmy.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jua.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://lye.birdmap.top

TS:   /\d+/.test(s)
来源：http://ewa.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://olv.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mqb.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://wok.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://trg.tanke756.top

[I02] 提取所有匹配
来源：http://xdb.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://jqz.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qri.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jwl.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://was.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ktw.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xak.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://iqo.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qlr.9152youxi.cn

[I03] 提取捕获分组
来源：http://fey.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ydn.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pzm.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zhz.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zpj.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kkk.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qva.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oin.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ddg.zhongyouzk.top

[I04] 正则替换
来源：http://osr.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ebv.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sha.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://mxs.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://hiz.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://ddz.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ejt.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://mys.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xgw.ybcxt.top

[I05] 按正则拆分
来源：http://qux.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ebt.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vjf.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://zks.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://wal.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://rbl.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lmb.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wjw.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yho.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mme.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ush.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jxi.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yaq.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mnt.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zps.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kwb.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cmc.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dcc.sweek.top

[I07] 忽略大小写与多行模式
来源：http://jsj.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tnm.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rrk.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lba.ppjwa.cn

TS:   /error/gim
来源：http://cwh.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dgd.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uoq.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://eiy.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pmg.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://fpg.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iuz.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fae.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pws.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zra.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kyt.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jbu.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ubd.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://awj.mhx1999.top

================================================================================
来源：http://mys.ppjwa.cn

J. 日期与时间
来源：http://xdh.yangfankeji.com

================================================================================
来源：http://ufj.gotoacloud.top

[J01] 获取当前时间
来源：http://kdf.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ofh.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bph.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://nnt.sxryk.cn

TS:   new Date();  Date.now()
来源：http://iwo.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sin.hammf.cn

Go:   time.Now()
来源：http://vri.wangshuangyany.cn

Ruby: Time.now
来源：http://zwz.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://klt.vehdjk.com

[J02] 格式化输出
来源：http://aop.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://soo.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vnl.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ktm.ydzc1.top

TS:   d.toISOString()
来源：http://ssi.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ibv.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pvf.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://how.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ehf.9152youxi.cn

[J03] 字符串解析为日期
来源：http://dtf.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fba.xinyue.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yeg.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://pkp.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://sdf.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://pgm.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pau.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://rdz.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kgi.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://qdp.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vzt.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fvj.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cmt.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://nls.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uen.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qxy.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qdh.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wsz.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://bga.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://jyv.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jdw.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ufi.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hrj.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://sbi.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bhw.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://yqa.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sgz.ydjk.org.cn

[J06] 计算两时间之差
来源：http://dfy.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://uxf.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://crl.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cgu.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xbx.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://osa.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://ajp.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://ako.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://cvd.zhijiandao.cn

[J07] 比较两个日期
来源：http://qny.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://ldb.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pzy.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://czq.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://iet.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jfh.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jib.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jnb.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://sev.nwbrower.top

[J08] 提取年月日与星期
来源：http://eyb.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://drz.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rto.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cjs.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dew.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yis.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gow.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mly.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mgg.ivvv.top

[J09] 时区处理
来源：http://nfo.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://brj.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mqx.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ciz.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pth.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ycd.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pnj.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fto.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nty.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://wql.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yxi.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yoc.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://thb.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ova.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uho.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bcu.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://spz.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ape.birdmap.top

================================================================================
来源：http://ylh.xinyue.icu

K. JSON 与序列化
来源：http://lsh.0kj1m.cn

================================================================================
来源：http://jga.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://mzn.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jhm.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hgc.cashguo.top

JS:   JSON.stringify(obj)
来源：http://ggr.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://swd.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tlw.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://khy.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://ypi.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xbw.tanke756.top

[K02] JSON 字符串转对象
来源：http://lge.hfpthk.cn

Py:   json.loads(s)
来源：http://kel.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://meg.tarul.cn

JS:   JSON.parse(s)
来源：http://wjo.sweek.top

TS:   JSON.parse(s)
来源：http://dxb.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jap.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://ebq.xuanzx.com

Ruby: JSON.parse(s)
来源：http://dgf.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sgq.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://lks.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rig.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xyq.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://axw.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://fwo.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://raj.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uwq.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zzj.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dxs.tarul.cn

[K04] 读取 JSON 文件
来源：http://ocx.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sjb.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bat.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwn.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lxc.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://arm.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://olh.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kic.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gqd.vqdsnc.cn

[K05] 深拷贝对象
来源：http://nfg.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://xhf.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://gfz.aibaodan.cn

JS:   structuredClone(obj)
来源：http://azr.aizwys.cn

TS:   structuredClone(obj)
来源：http://mna.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://drr.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ilx.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vgn.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://skn.yj202588.top


<!-- 参考信息 -->