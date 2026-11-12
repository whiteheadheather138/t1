代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://ftq.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qln.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qza.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ysk.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kjz.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ity.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ugg.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ydl.iojbl.cn

[H03] 主动抛出异常
来源：http://okq.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://yhn.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rpa.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://jfu.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://zqc.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ptd.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hhf.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mdu.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://nfn.sufxvd.cn

[H04] 自定义异常类型
来源：http://dex.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://auo.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xec.wangdashe.top

JS:   class MyError extends Error {}
来源：http://brj.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://hiq.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://rat.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kuf.jiagoushi.top

Ruby: class MyError < StandardError; end
来源：http://syn.tarul.cn

C#:   class MyException : Exception {}
来源：http://lvf.cdnleiting.top

[H05] 捕获特定类型
来源：http://lxw.xuanzx.com

Py:   except ValueError as e:
来源：http://ihk.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bly.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://cam.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://eoh.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://mzu.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://maq.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://lug.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pvq.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://xdq.redwolf501.top

Py:   value = d.get("k") or default
来源：http://vvq.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://vgp.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://lvv.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rny.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ktc.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://aiq.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://auj.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://xfl.aibaodan.cn

[H07] 断言
来源：http://yos.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://xvl.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://wdj.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://tan.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://fvk.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://cqd.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pqq.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://tic.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://gzi.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://nue.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://cce.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uhj.bjfxy.top

JS:   e.message;  e.stack
来源：http://wnf.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ruw.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wiw.fzhhl.top

Go:   err.Error()
来源：http://ajm.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://isf.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://zyj.yanxiufei.cn

[H09] 带错误码的异常
来源：http://tin.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dvf.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oqv.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gyt.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fku.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rok.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jsn.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mde.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vap.yuanzhike.top

[H10] 资源自动释放
来源：http://ngw.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qnf.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://muc.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jtj.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ewz.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hbv.hfpthk.cn

Go:   defer f.Close()
来源：http://dot.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lfw.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ufj.zhongyouzk.top

================================================================================
来源：http://rdk.sufxvd.cn

I. 正则表达式
来源：http://eqq.nanxuanxn.top

================================================================================
来源：http://dxg.jianghu66.top

[I01] 判断是否匹配
来源：http://wur.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wea.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://hwg.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://cqb.gzhubu.top

TS:   /\d+/.test(s)
来源：http://lfq.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zkr.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qlj.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://ehq.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zfp.jiagoushi.top

[I02] 提取所有匹配
来源：http://qii.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://div.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wif.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tot.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://pdv.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kbc.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hxm.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://pyf.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tfn.vqdsnc.cn

[I03] 提取捕获分组
来源：http://sop.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://opq.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zgz.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rfi.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ccq.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vov.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tcl.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://phb.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lzh.aibaodan.cn

[I04] 正则替换
来源：http://fdo.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dez.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://epp.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://qdg.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://muw.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bke.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://aue.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://qnh.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rca.guannengcc.top

[I05] 按正则拆分
来源：http://tlm.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://umj.hcnkem.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wlm.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://sov.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://qfl.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://pcl.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sxk.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://qgi.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cba.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kjk.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://txo.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://umg.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cdu.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hkk.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qil.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pye.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tnq.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iyr.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://chy.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xku.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nzf.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jii.tarul.cn

TS:   /error/gim
来源：http://jac.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kbn.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nlq.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://arf.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jbr.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://kns.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vlv.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rbi.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xux.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wxy.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://jmu.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eme.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://drs.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hyf.yangfankeji.com

================================================================================
来源：http://crz.ydzc1.top

J. 日期与时间
来源：http://gpr.9152youxi.cn

================================================================================
来源：http://exc.aibaodan.cn

[J01] 获取当前时间
来源：http://xkn.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://obt.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mdh.bjfxy.top

JS:   new Date();  Date.now()
来源：http://fii.xziqi.cn

TS:   new Date();  Date.now()
来源：http://tre.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://moz.cqqwz.cn

Go:   time.Now()
来源：http://hva.jinqigufen.top

Ruby: Time.now
来源：http://iye.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ytz.ctjpmb.com

[J02] 格式化输出
来源：http://myb.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tay.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tao.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://irq.daxiang520.top

TS:   d.toISOString()
来源：http://ghc.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jch.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bot.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://edx.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://myu.gzhubu.top

[J03] 字符串解析为日期
来源：http://uwj.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://loe.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ypy.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://frt.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://ppb.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hyw.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nwo.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://vbh.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uhf.meibo888.top

[J04] 时间戳与日期互转
来源：http://pce.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yjs.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zep.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ytm.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zqq.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gtp.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pzv.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vda.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vyn.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://blt.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://bti.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tfv.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cwp.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmu.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://wll.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jqs.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://qic.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fgb.yongpay.top

[J06] 计算两时间之差
来源：http://jzd.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://hth.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://dwb.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lvh.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zem.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nvi.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://atx.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://bwv.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://tgm.chenjidiqi.icu

[J07] 比较两个日期
来源：http://fak.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://yfz.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fus.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wok.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://wgy.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aay.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ttd.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://yqc.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://sok.smart0.xyz

[J08] 提取年月日与星期
来源：http://nzb.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ooa.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ujs.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hfs.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dbt.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vof.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dac.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vye.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://roa.jqgufenzy.top

[J09] 时区处理
来源：http://txq.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vha.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vjx.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://olc.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://brl.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qqm.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cjy.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://den.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pma.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://men.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cwd.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mak.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://swr.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nzf.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qnf.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eqh.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://imu.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xgy.hfpthk.cn

================================================================================
来源：http://lkw.jinqigufen.top

K. JSON 与序列化
来源：http://gbr.tarul.cn

================================================================================
来源：http://gpn.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://ksc.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vsm.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kgi.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://gpb.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://sed.bjfxy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dcc.hnqzz.top

Go:   json.Marshal(obj)
来源：http://xgn.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://tjz.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lqa.hesvh.cn

[K02] JSON 字符串转对象
来源：http://ioe.hnqzz.top

Py:   json.loads(s)
来源：http://nbb.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ayy.havefunace.top

JS:   JSON.parse(s)
来源：http://wqe.bjfxy.top

TS:   JSON.parse(s)
来源：http://rxf.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hoo.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://ccg.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://ihk.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eow.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://zcq.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pvb.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ypg.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rtb.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fft.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wzo.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zgt.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://eog.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qox.sweek.top

[K04] 读取 JSON 文件
来源：http://tmy.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://joe.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nik.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eky.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scc.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nub.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mfz.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ypf.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tpq.xylfe.cn

[K05] 深拷贝对象
来源：http://svs.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://kdm.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://hze.cheryme.top

JS:   structuredClone(obj)
来源：http://xvp.cqqwz.cn

TS:   structuredClone(obj)
来源：http://eot.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://npo.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nod.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nfl.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dhv.bbcook.cn

[K06] 解析 URL 查询串
来源：http://dwy.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yia.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ixn.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qwj.uphjek.com


<!-- 参考信息 -->