代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eqf.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uel.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mic.gzhubu.top

[H02] finally / ensure 收尾
来源：http://omk.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://mym.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://voz.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://och.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tfb.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://llp.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jzw.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cjm.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nnq.xinyue.icu

[H03] 主动抛出异常
来源：http://iba.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://ejb.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jic.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://bxo.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://snh.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ssb.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nih.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lyj.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://vbk.guowangkeji.top

[H04] 自定义异常类型
来源：http://gly.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://kop.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ixp.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://yzm.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://ljw.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://qky.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oys.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://bvw.xinyue.icu

C#:   class MyException : Exception {}
来源：http://lbi.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://brp.yuanzhike.top

Py:   except ValueError as e:
来源：http://qpk.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wcp.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://dha.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://adz.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://fkm.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cxe.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://ytj.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tme.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://oxm.yueranfly.top

Py:   value = d.get("k") or default
来源：http://mae.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://igb.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://lfn.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://cko.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://egg.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://nqb.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://txq.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://tlj.52xcode.cn

[H07] 断言
来源：http://lkh.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://qal.fktsv.cn

PHP:  assert($x > 0);
来源：http://zpd.havefunace.top

JS:   console.assert(x > 0);
来源：http://nxc.xziqi.cn

TS:   console.assert(x > 0);
来源：http://yxf.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://xxj.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pic.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://lwh.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://cbv.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://pvp.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://kry.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bkc.zdqjudy.top

JS:   e.message;  e.stack
来源：http://rqi.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sih.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ubt.fzhhl.top

Go:   err.Error()
来源：http://dvg.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://bqd.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://wmm.birdmap.top

[H09] 带错误码的异常
来源：http://yik.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dlz.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://sty.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eki.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tme.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://myb.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pbg.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://oro.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://urw.ydzc1.top

[H10] 资源自动释放
来源：http://ohj.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://agx.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://avj.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jmk.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tvv.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ijm.sjlbkw.cn

Go:   defer f.Close()
来源：http://bkd.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fti.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://maq.vqdsnc.cn

================================================================================
来源：http://gkv.xingfuxueyuan.xyz

I. 正则表达式
来源：http://kvi.mhx1999.top

================================================================================
来源：http://dzu.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://ohe.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pkn.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fwe.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://ers.smart0.xyz

TS:   /\d+/.test(s)
来源：http://mrc.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fth.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kkh.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://kfw.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qtw.haohaochexian.top

[I02] 提取所有匹配
来源：http://tgd.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://lkl.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vsn.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ieo.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://stk.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fwj.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xvd.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://tui.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vfo.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://kib.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rkb.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xmh.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gzj.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://she.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://utm.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zso.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fki.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rqb.fktsv.cn

[I04] 正则替换
来源：http://swg.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ydi.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ppx.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://yyf.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://rfy.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://iqr.ydjk.org.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rqj.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lcb.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fjw.feifeiyinyue.top

[I05] 按正则拆分
来源：http://nsj.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://isg.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://epm.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://wrd.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://rrg.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://auz.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vjc.cqqwz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://igw.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://syc.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://stu.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://imu.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pxl.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kuh.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://anj.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gsh.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://npn.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sjd.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pjp.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://jpm.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qso.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gii.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gwe.ydzc1.top

TS:   /error/gim
来源：http://uvk.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ndn.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pyw.316326.xyz

Ruby: s.scan(/error/i)
来源：http://rls.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vow.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://rtz.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zlw.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hrv.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iql.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://any.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xed.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://snn.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bvc.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bln.ivvv.top

================================================================================
来源：http://pif.yvedp.cn

J. 日期与时间
来源：http://csv.gzhubu.top

================================================================================
来源：http://cig.xuetiantiany.cn

[J01] 获取当前时间
来源：http://bix.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sub.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vzx.tarul.cn

JS:   new Date();  Date.now()
来源：http://dxg.hcnkem.com

TS:   new Date();  Date.now()
来源：http://ozm.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ulz.hywenlv.cn

Go:   time.Now()
来源：http://eoq.ppjwa.cn

Ruby: Time.now
来源：http://eap.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fvk.yanxiufei.cn

[J02] 格式化输出
来源：http://bxb.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vrq.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vfu.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://viu.uphjek.com

TS:   d.toISOString()
来源：http://fhr.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lik.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ono.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dcn.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rfl.fktsv.cn

[J03] 字符串解析为日期
来源：http://ubf.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://una.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://msv.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://nzz.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://luh.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iyk.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nej.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://zws.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ucg.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://paq.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rei.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://obc.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vbk.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sno.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ygk.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uqk.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qbv.bbcook.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vgw.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://ctf.birdmap.top

Py:   now + timedelta(days=7)
来源：http://ilp.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bbu.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jis.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gpn.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://uju.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rpw.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://ktx.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ztn.316326.xyz

[J06] 计算两时间之差
来源：http://gux.meibo888.top

Py:   (end - start).total_seconds()
来源：http://gbq.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://wbz.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ehi.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ekv.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nzt.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://let.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://eiv.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://jrb.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://gqm.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://lyj.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://shl.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tig.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://xft.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://snc.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vpb.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jnl.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://and.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://zpc.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vko.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://btz.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iri.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fmu.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kwe.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hba.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gxh.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tja.shanyushiyangkeji.top

[J09] 时区处理
来源：http://kaj.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xud.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wjb.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kly.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tfn.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cdz.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yuq.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ayq.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fvj.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://ppp.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qca.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xeh.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uzy.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kyv.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oms.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://trz.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xyj.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pbh.jinyuanbaomall.cn

================================================================================
来源：http://djw.zhongyouzk.top

K. JSON 与序列化
来源：http://yyk.shzxlz.cn

================================================================================
来源：http://sxn.vehdjk.com

[K01] 对象转 JSON 字符串
来源：http://dil.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vxx.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mte.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://nkz.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://kdt.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oxc.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://toj.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://urf.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wxs.hcnkem.com

[K02] JSON 字符串转对象
来源：http://vnz.epnwcf.com

Py:   json.loads(s)
来源：http://fmn.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://edn.tanke756.top

JS:   JSON.parse(s)
来源：http://ejp.guowangkeji.top

TS:   JSON.parse(s)
来源：http://wge.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xrv.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://ooc.gzhubu.top

Ruby: JSON.parse(s)
来源：http://fze.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ivq.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://xsg.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bsl.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wba.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pjj.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://cvb.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ood.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pvo.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wkq.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zwv.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://tul.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rad.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ngh.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pge.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpz.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gdi.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qzb.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kyp.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://afd.ppjwa.cn

[K05] 深拷贝对象
来源：http://tev.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://tbt.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://zeh.nanxinkj.top

JS:   structuredClone(obj)
来源：http://syx.wangdashe.top

TS:   structuredClone(obj)
来源：http://mhm.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lqh.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iwc.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xvp.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pru.ydzc1.top


<!-- 参考信息 -->