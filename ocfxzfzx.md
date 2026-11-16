代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fxp.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jsz.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tau.gzhubu.top

[H02] finally / ensure 收尾
来源：http://crn.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://wur.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ugx.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cwu.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lsf.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://jzt.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hjb.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sxo.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lrw.havefunace.top

[H03] 主动抛出异常
来源：http://pqu.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://itm.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tsc.hammf.cn

JS:   throw new Error("错误信息");
来源：http://cpj.hammf.cn

TS:   throw new Error("错误信息");
来源：http://dar.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pbu.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qcy.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hyd.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://wsq.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://lmw.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://hwc.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hza.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://nlq.tian-w.cn

TS:   class MyError extends Error {}
来源：http://syw.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://tsd.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hmz.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://wuc.smart0.xyz

C#:   class MyException : Exception {}
来源：http://umz.hfpthk.cn

[H05] 捕获特定类型
来源：http://mhe.chenzaomai.com

Py:   except ValueError as e:
来源：http://fyg.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hwe.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://xfa.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://bxb.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://bhh.nwbrower.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rzz.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://flg.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cuk.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://gme.hnqzz.top

Py:   value = d.get("k") or default
来源：http://trh.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://djr.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uoa.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://tzc.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fky.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qjt.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://mtl.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://pko.xuanzx.com

[H07] 断言
来源：http://ubb.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://tnn.316326.xyz

PHP:  assert($x > 0);
来源：http://dda.cashguo.top

JS:   console.assert(x > 0);
来源：http://ohb.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://vjk.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://esa.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://goz.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://xzp.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://mnv.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://qwl.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://gaq.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xar.xinyue.icu

JS:   e.message;  e.stack
来源：http://mdo.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://vio.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://drb.havefunace.top

Go:   err.Error()
来源：http://krf.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://obf.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://kqr.pycfn.com

[H09] 带错误码的异常
来源：http://qhh.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xss.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ufz.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rau.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qby.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xae.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rby.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qmu.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://pty.xuetiantiany.cn

[H10] 资源自动释放
来源：http://dfq.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zrz.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sgl.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oen.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vus.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmy.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://pbp.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dur.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tkl.guowangkeji.top

================================================================================
来源：http://qkr.zhijiandao.cn

I. 正则表达式
来源：http://gqq.wangshuangyany.cn

================================================================================
来源：http://qlo.cdnleiting.top

[I01] 判断是否匹配
来源：http://tzt.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bzy.xuetiantiany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kbm.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://iyn.jianghu66.top

TS:   /\d+/.test(s)
来源：http://mft.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uyn.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xew.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://dvg.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hrs.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://csk.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://chs.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://llm.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ipk.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://qxe.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jnf.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ojz.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://yvg.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ksa.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://meo.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xdh.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dwu.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://alq.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zif.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rdm.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rxs.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xym.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ann.ehwqpu.com

[I04] 正则替换
来源：http://rgl.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aod.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xxx.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://oiy.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://xsc.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://otb.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uac.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eqr.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ijm.cdnleiting.top

[I05] 按正则拆分
来源：http://yop.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cbh.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fpr.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://iqy.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://tve.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://yph.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kjm.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hrj.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qsx.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ljr.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jvc.zdqjudy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ddk.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gzl.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pup.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xsa.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gox.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lpe.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bnx.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://hev.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xbx.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://let.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nkr.shangyingyoupin.top

TS:   /error/gim
来源：http://bxw.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://utt.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://npd.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://trv.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qpp.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://tta.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ads.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tvi.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://orx.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mkz.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://bzl.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ipc.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tox.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ope.pycfn.com

================================================================================
来源：http://yuw.tian-w.cn

J. 日期与时间
来源：http://mbl.yuxming.cn

================================================================================
来源：http://slu.snrcjt.cn

[J01] 获取当前时间
来源：http://wzb.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://usy.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rsh.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://slo.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://ffr.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://evh.52xcode.cn

Go:   time.Now()
来源：http://ncc.cheryme.top

Ruby: Time.now
来源：http://pfj.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jfj.pengpengdd.cyou

[J02] 格式化输出
来源：http://age.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qkm.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wnz.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lmq.nanxuanxn.top

TS:   d.toISOString()
来源：http://bcr.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wth.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yws.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ltd.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://glb.jinqigufen.top

[J03] 字符串解析为日期
来源：http://gqe.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yqb.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://skt.pycfn.com

JS:   new Date("2024-01-02")
来源：http://jup.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://rju.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://zyk.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cow.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://psg.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://upj.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://ddz.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nno.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wjg.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kgq.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ddz.pengpengdd.cyou

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nge.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://opa.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oam.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ymj.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://ggd.316326.xyz

Py:   now + timedelta(days=7)
来源：http://ipg.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://weg.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wdr.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xst.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://mcq.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fav.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://otw.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://hir.aizwys.cn

[J06] 计算两时间之差
来源：http://hww.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://eec.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://qeq.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tbk.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://phn.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://zsg.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://pgo.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://enl.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://vdb.jqgfzy.top

[J07] 比较两个日期
来源：http://buo.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://phe.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nmn.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://obm.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mkx.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lfs.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oze.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://adp.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://kxp.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://bfh.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iar.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yls.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxv.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vrc.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lox.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hgj.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iyc.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lie.sjlbkw.cn

[J09] 时区处理
来源：http://swd.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://opy.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ebk.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbw.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gxc.fktsv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yif.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://epq.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vce.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rlq.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://plx.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cpn.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://joe.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iom.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wmp.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hrv.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rmm.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tzz.jianghu66.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ftv.jiagoushi.top

================================================================================
来源：http://yfg.fzhhl.top

K. JSON 与序列化
来源：http://lgs.yj20258.top

================================================================================
来源：http://uxr.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://eoj.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cbz.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ixc.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://xva.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://kma.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sua.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://klv.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://xsf.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lhm.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://fje.zdqjudy.top

Py:   json.loads(s)
来源：http://ayu.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wvz.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://djp.uphjek.com

TS:   JSON.parse(s)
来源：http://eqv.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://meb.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://gya.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://uwc.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dsu.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://eic.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://klx.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yzm.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pgo.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://vkz.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rqc.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mid.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ula.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nlu.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://bbi.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ryn.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vpy.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dox.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://foa.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cmj.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kzz.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pir.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xhx.wangdashe.top

[K05] 深拷贝对象
来源：http://oxs.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://mcw.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://ave.epnwcf.com

JS:   structuredClone(obj)
来源：http://edw.daria6918.cn

TS:   structuredClone(obj)
来源：http://ywe.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://mzf.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://juu.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iln.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tpf.wangdashe.top


<!-- 参考信息 -->