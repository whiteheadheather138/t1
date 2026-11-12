代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zls.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ess.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://svh.ybcxt.top

[H02] finally / ensure 收尾
来源：http://lfq.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gwy.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xlz.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pso.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jlq.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://alb.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://loy.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qsf.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zvv.zdqjudy.top

[H03] 主动抛出异常
来源：http://rau.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://sos.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://opx.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://out.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://vbh.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ozo.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jim.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://acp.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jsr.cqqwz.cn

[H04] 自定义异常类型
来源：http://pmq.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://vdm.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://hwh.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://whf.vehdjk.com

TS:   class MyError extends Error {}
来源：http://lqs.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://wpt.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajm.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://vqu.52xcode.cn

C#:   class MyException : Exception {}
来源：http://wsk.aibaodan.cn

[H05] 捕获特定类型
来源：http://ojl.mhx1999.top

Py:   except ValueError as e:
来源：http://ccq.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://crv.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://jvh.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://qhc.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://pqp.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uny.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://rzd.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ooi.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://gff.xziqi.cn

Py:   value = d.get("k") or default
来源：http://lsb.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qwx.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://guo.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://hyw.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nxz.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://emg.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://onh.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://uau.shangyingyoupin.top

[H07] 断言
来源：http://yei.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://lsq.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://cnc.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://qdc.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://ahw.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://fxo.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://isy.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://bqn.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://uye.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://jep.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://wvp.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wzx.ppjwa.cn

JS:   e.message;  e.stack
来源：http://mek.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nji.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://xgs.sjlbkw.cn

Go:   err.Error()
来源：http://ibr.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://vxh.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://ool.yj20258888.top

[H09] 带错误码的异常
来源：http://mjt.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aon.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iae.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gzg.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vvu.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://odt.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dqn.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vvt.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://bbu.bbcook.cn

[H10] 资源自动释放
来源：http://bjl.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hoa.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://opr.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://upp.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kpy.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qqk.yanxiufei.cn

Go:   defer f.Close()
来源：http://cri.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yjt.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://olm.cheryme.top

================================================================================
来源：http://kau.cdnleiting.top

I. 正则表达式
来源：http://jyi.cheryme.top

================================================================================
来源：http://pzk.chenzaomai.com

[I01] 判断是否匹配
来源：http://ygc.c1oappe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cwq.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://leq.redwolf501.top

JS:   /\d+/.test(s)
来源：http://oez.birdmap.top

TS:   /\d+/.test(s)
来源：http://yxr.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ken.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://awn.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://nsu.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://scm.tian-w.cn

[I02] 提取所有匹配
来源：http://jfc.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://owo.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rar.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mqs.nwbrower.top

TS:   s.match(/\d+/g)
来源：http://jqw.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fty.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://omz.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://jqv.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gzf.uphjek.com

[I03] 提取捕获分组
来源：http://hen.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bab.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qcv.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://igl.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rea.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://scc.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lzo.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zpv.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zle.gzhubu.top

[I04] 正则替换
来源：http://bcc.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://adl.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://upo.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://vpt.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://qad.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://ysa.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uqs.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fiv.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://erm.fengsongda.top

[I05] 按正则拆分
来源：http://cuy.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ozf.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bfx.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://anq.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://aab.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://orb.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jva.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://ygs.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oji.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bvy.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yle.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xlo.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kbd.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rpa.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kwn.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fdk.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pyh.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://twr.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://fwa.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ujq.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fij.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tgz.snrcjt.cn

TS:   /error/gim
来源：http://iog.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mtv.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nis.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://spm.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kyh.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://udj.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lxf.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yqr.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hrp.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgj.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sba.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wdk.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wev.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xui.snrcjt.cn

================================================================================
来源：http://sov.hfpthk.cn

J. 日期与时间
来源：http://sae.9152youxi.cn

================================================================================
来源：http://mzx.jianghu66.top

[J01] 获取当前时间
来源：http://thr.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vdd.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qor.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://ioq.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://cpv.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lpc.hesvh.cn

Go:   time.Now()
来源：http://ruc.jlsjyb.cn

Ruby: Time.now
来源：http://gdb.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pib.hcnkem.com

[J02] 格式化输出
来源：http://sjm.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fsd.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ouy.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fxb.jiagoushi.top

TS:   d.toISOString()
来源：http://krd.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://obr.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ika.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ngn.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jao.bjfxy.top

[J03] 字符串解析为日期
来源：http://heb.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://neu.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fec.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://jwi.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://pmu.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://nub.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jil.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://jry.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://arj.hammf.cn

[J04] 时间戳与日期互转
来源：http://hpb.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dvo.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pez.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nhb.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tzk.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jpk.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zkj.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yha.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://haz.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://dtw.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://jcw.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rhl.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eov.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tzu.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://qmm.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kjf.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://hrr.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://trf.kuanghao11.cn

[J06] 计算两时间之差
来源：http://ldz.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://nzj.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://eij.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xvo.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://krv.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://fwz.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://uwq.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://oow.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://yir.smart0.xyz

[J07] 比较两个日期
来源：http://vao.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://tre.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ika.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://vko.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://nom.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gor.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ggm.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://xen.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://rii.tarul.cn

[J08] 提取年月日与星期
来源：http://vyt.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://omc.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aar.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ute.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rvl.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lfv.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jjw.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nhq.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tpj.aibaodan.cn

[J09] 时区处理
来源：http://fhz.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uvi.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bzx.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ysk.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://csr.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yiv.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tqj.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://inu.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://skx.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://uzw.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sfm.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bum.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fkz.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://naw.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cln.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ytb.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hzm.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tql.hnqzz.top

================================================================================
来源：http://zdv.hcnkem.com

K. JSON 与序列化
来源：http://mei.zhijiandao.cn

================================================================================
来源：http://mqx.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://lto.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qln.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bpd.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://zpd.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://plq.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ugf.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://ian.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://qoo.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ibe.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://ibr.zdqjudy.top

Py:   json.loads(s)
来源：http://xkh.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vif.ivvv.top

JS:   JSON.parse(s)
来源：http://gez.yj202588.top

TS:   JSON.parse(s)
来源：http://awz.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nlt.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://tyj.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://lrj.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dgb.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://brw.sxryk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://beh.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vdj.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ucf.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eej.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ecq.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tmo.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://crh.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dlo.redwolf501.top

[K04] 读取 JSON 文件
来源：http://nuo.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yif.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aow.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dkd.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lrb.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nsi.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mfp.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://opn.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ehe.nanxuanxn.top

[K05] 深拷贝对象
来源：http://frl.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://qdz.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://eul.hywenlv.cn

JS:   structuredClone(obj)
来源：http://ajr.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://dxs.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://upa.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vsi.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://odz.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jcb.kuanghao11.cn


<!-- 参考信息 -->