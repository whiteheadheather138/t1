代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aqg.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tzg.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ydy.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://gqm.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://xxu.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://txt.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yrt.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mmn.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dig.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uzv.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ihn.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iiy.ehwqpu.com

[H03] 主动抛出异常
来源：http://fuo.chenzaomai.com

Py:   raise ValueError("错误信息")
来源：http://sdm.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qqn.hammf.cn

JS:   throw new Error("错误信息");
来源：http://grx.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://mxy.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://cga.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bhh.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ywp.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://htv.shzxlz.cn

[H04] 自定义异常类型
来源：http://bgt.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://lnu.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mff.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://hgf.bbcook.cn

TS:   class MyError extends Error {}
来源：http://ldz.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://pba.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xov.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://fsy.hcnkem.com

C#:   class MyException : Exception {}
来源：http://udx.yj202588.top

[H05] 捕获特定类型
来源：http://srl.svipenyu.cn

Py:   except ValueError as e:
来源：http://ihy.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xqt.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://jje.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://tsp.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://ycg.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ebc.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://vef.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lrm.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://lkc.gzhubu.top

Py:   value = d.get("k") or default
来源：http://qmg.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://muj.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://elt.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xio.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://izo.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://drk.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://tab.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://xyi.zhixingplan.top

[H07] 断言
来源：http://ylp.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://gux.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://oqy.sysykeji.top

JS:   console.assert(x > 0);
来源：http://ihr.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://cih.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://frs.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mvg.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://lqt.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://agq.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://rty.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://flt.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cjy.0kj1m.cn

JS:   e.message;  e.stack
来源：http://qew.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://khx.chenzaomai.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jjy.dianchejie.cn

Go:   err.Error()
来源：http://gka.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://iot.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://bxh.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://ffq.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zuu.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://evz.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pyp.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vxf.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://srt.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qij.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://lrk.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://tyf.hnqzz.top

[H10] 资源自动释放
来源：http://doo.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xhy.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aze.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://koz.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://woc.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fbl.316326.xyz

Go:   defer f.Close()
来源：http://rwh.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zin.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://agz.aibaodan.cn

================================================================================
来源：http://yfi.hysaishi.cn

I. 正则表达式
来源：http://fbr.shzxlz.cn

================================================================================
来源：http://fck.316326.xyz

[I01] 判断是否匹配
来源：http://enw.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uae.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://mwp.vehdjk.com

JS:   /\d+/.test(s)
来源：http://ykq.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://awc.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rqk.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xkt.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://ryf.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mys.jyoumei.cn

[I02] 提取所有匹配
来源：http://xfi.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://yma.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dvd.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ext.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://dhn.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mox.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vwt.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://tju.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://obh.andypj.xyz

[I03] 提取捕获分组
来源：http://dwd.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bql.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://req.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xzm.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mel.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iew.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tbv.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dnf.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zdr.shanyushiyangkeji.top

[I04] 正则替换
来源：http://trz.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://qaq.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yfx.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://blu.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pvf.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://wvv.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lmz.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qbg.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oyq.yueranfly.top

[I05] 按正则拆分
来源：http://kvg.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nlo.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ttg.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://gfx.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://rus.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://vwp.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rnt.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://glu.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nbs.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zow.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qub.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dga.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jfu.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qtq.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jnh.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://umf.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sja.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dyh.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://mwl.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yxy.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dlv.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mqr.yangfankeji.com

TS:   /error/gim
来源：http://uvd.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vmt.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qel.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://end.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xym.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://tbn.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xjv.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gdq.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xwo.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wxe.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://seg.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wns.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://upx.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jql.ctjpmb.com

================================================================================
来源：http://zii.hammf.cn

J. 日期与时间
来源：http://jih.xuanzx.com

================================================================================
来源：http://ogo.cdnleiting.top

[J01] 获取当前时间
来源：http://gxb.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://dif.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bdd.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://qgt.pycfn.com

TS:   new Date();  Date.now()
来源：http://sje.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fqm.shanyushiyangkeji.top

Go:   time.Now()
来源：http://hmu.tarul.cn

Ruby: Time.now
来源：http://sby.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nqs.gzhubu.top

[J02] 格式化输出
来源：http://uuj.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tel.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cqv.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gry.pycfn.com

TS:   d.toISOString()
来源：http://oeh.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dsj.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uyt.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kht.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jhl.cdnleiting.top

[J03] 字符串解析为日期
来源：http://xng.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ngl.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zcg.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://hnj.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://zff.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cbe.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ula.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://opr.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yjm.fengsongda.top

[J04] 时间戳与日期互转
来源：http://ano.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ngb.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://swo.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fan.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://lvs.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://alv.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xri.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mbn.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mgt.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://wua.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://qmd.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ylg.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://muv.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eby.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://wwa.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sql.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://idj.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://rnr.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://hwv.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://mha.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://vkk.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qrb.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nzg.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mvh.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://ild.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://ean.quarkkingdee.top

C#:   (end - start).TotalSeconds
来源：http://sei.jiagoushi.top

[J07] 比较两个日期
来源：http://mcs.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://ktp.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pza.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://kgd.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bfn.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yrj.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zwc.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hvf.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://mjo.shuidangran.top

[J08] 提取年月日与星期
来源：http://xox.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://apo.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aol.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dud.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cxi.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fzk.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://isb.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bef.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rhs.sjlbkw.cn

[J09] 时区处理
来源：http://nrq.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sof.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zqc.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ptt.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywq.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fhn.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://idv.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yas.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lib.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://ian.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tgi.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://svd.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://suj.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ksd.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tfd.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://idv.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://epi.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mbm.tianlin.xyz

================================================================================
来源：http://ghu.yuxming.cn

K. JSON 与序列化
来源：http://ggd.vqdsnc.cn

================================================================================
来源：http://qkf.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://alo.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qcl.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bvh.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://cvp.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://ltx.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yxy.zhoulong.xyz

Go:   json.Marshal(obj)
来源：http://eam.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://uoa.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qhn.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://lgu.sxryk.cn

Py:   json.loads(s)
来源：http://laq.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fbz.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://iqh.hysaishi.cn

TS:   JSON.parse(s)
来源：http://wgq.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://asn.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://sac.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://isl.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rhq.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://qml.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zvh.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mkb.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hup.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://nkj.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cdj.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ubb.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://jbd.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dfb.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://rag.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gvt.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yli.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ily.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmh.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mbo.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://shi.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://mde.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jnx.zhixingplan.top

[K05] 深拷贝对象
来源：http://wuk.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://wnc.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://bgj.52xcode.cn

JS:   structuredClone(obj)
来源：http://riw.hcnkem.com

TS:   structuredClone(obj)
来源：http://utx.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://znu.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lyk.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jsl.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wtn.nwbrower.top


<!-- 参考信息 -->