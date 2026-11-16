代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://owv.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wuz.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cav.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tbx.9152youxi.cn

[H03] 主动抛出异常
来源：http://log.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://opi.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hki.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://rjp.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://sat.zhijiandao.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vnc.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://giy.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fji.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://itb.meibo888.top

[H04] 自定义异常类型
来源：http://nkd.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://mdr.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://zoh.52xcode.cn

JS:   class MyError extends Error {}
来源：http://lrt.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://sfx.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://mdv.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tib.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://tuq.epnwcf.com

C#:   class MyException : Exception {}
来源：http://vbi.9152youxi.cn

[H05] 捕获特定类型
来源：http://ymj.cdnleiting.top

Py:   except ValueError as e:
来源：http://gkh.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bud.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://wfs.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://rpe.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://ryf.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bqa.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://byq.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ytt.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://nds.uphjek.com

Py:   value = d.get("k") or default
来源：http://mgt.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kwd.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qxv.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://cyo.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rke.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xin.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://aqv.meibo888.top

C#:   obj?.A?.B ?? default
来源：http://awn.quarkkingdee.top

[H07] 断言
来源：http://cys.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://qxb.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://bub.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://ghx.xuanzx.com

TS:   console.assert(x > 0);
来源：http://hoc.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://vyq.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zec.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://usm.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://tim.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://lyj.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://rom.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pal.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://ngu.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nvc.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fhf.0kj1m.cn

Go:   err.Error()
来源：http://yxr.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://gpe.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://uns.guannengcc.top

[H09] 带错误码的异常
来源：http://usq.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zmr.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hlt.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yqf.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oqv.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ooj.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gon.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://jqy.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rsx.hesvh.cn

[H10] 资源自动释放
来源：http://zpi.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fio.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jqv.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iat.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dnc.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bjd.zdqjudy.top

Go:   defer f.Close()
来源：http://mfw.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pvc.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tgt.mhx1999.top

================================================================================
来源：http://tfw.fktsv.cn

I. 正则表达式
来源：http://lqt.fzhhl.top

================================================================================
来源：http://dce.yangfankeji.com

[I01] 判断是否匹配
来源：http://jox.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://llg.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bpw.daria6918.cn

JS:   /\d+/.test(s)
来源：http://pab.iojbl.cn

TS:   /\d+/.test(s)
来源：http://dsv.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vmt.hnqzz.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cdq.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://vww.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zit.vqdsnc.cn

[I02] 提取所有匹配
来源：http://iso.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://nmz.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eqd.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kxy.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://rfd.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zng.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kae.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://ics.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kxj.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://ozu.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ypv.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wym.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cdl.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cgh.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ilf.fehbvm.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xfc.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://din.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ixr.jqgufenzy.top

[I04] 正则替换
来源：http://wex.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ybl.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cyh.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ync.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://yte.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://ndx.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hfv.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xqp.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nka.redwolf501.top

[I05] 按正则拆分
来源：http://sik.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tba.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iqp.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://vbj.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://mei.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://bmb.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zas.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ngt.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uzy.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dyo.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oqx.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blc.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vwt.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tgs.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wzr.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://djh.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qyv.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://phc.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://yxy.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qfz.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pdw.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vwq.andypj.xyz

TS:   /error/gim
来源：http://lar.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zsv.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cmj.uphjek.com

Ruby: s.scan(/error/i)
来源：http://ixp.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ieh.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://ugd.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aqy.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lbs.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://osw.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsi.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://nng.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://usa.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yek.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dnx.hesvh.cn

================================================================================
来源：http://ibm.jinqigufen.top

J. 日期与时间
来源：http://ozw.xziqi.cn

================================================================================
来源：http://hml.chenzaomai.com

[J01] 获取当前时间
来源：http://gkp.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qwq.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jzy.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://rax.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://pkk.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pmu.zhoulong.xyz

Go:   time.Now()
来源：http://cfh.aibaodan.cn

Ruby: Time.now
来源：http://jdf.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zjt.gaohongyu789.top

[J02] 格式化输出
来源：http://wkj.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ajx.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nrm.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cpu.hysaishi.cn

TS:   d.toISOString()
来源：http://tme.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://axf.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://edt.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axi.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://djf.fehbvm.com

[J03] 字符串解析为日期
来源：http://xkk.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://srj.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://myr.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://rig.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://wpn.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://vde.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jpu.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://xkd.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pbl.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://bfo.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tmc.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yqb.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jyv.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://drs.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eqt.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pok.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://peg.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qmq.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://lzg.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://eft.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kxf.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xun.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ece.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://fvb.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rlm.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://rlu.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://yrd.hnxiangtu.top

[J06] 计算两时间之差
来源：http://yqy.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://zxg.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://cty.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tuy.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zdi.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://bvb.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://jca.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://exl.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://lpc.c1oappe.top

[J07] 比较两个日期
来源：http://xyu.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://ekz.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ilj.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://znj.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zjy.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://svz.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tyv.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bns.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://dys.cdnleiting.top

[J08] 提取年月日与星期
来源：http://grf.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hle.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fau.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hip.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sub.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wmc.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rnc.andypj.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iwo.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://exu.cucudq.cn

[J09] 时区处理
来源：http://urd.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eze.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wjb.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwq.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://leo.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ezh.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cpt.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://qrq.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hpe.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://exy.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ims.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zft.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rlv.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bai.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bnc.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pzt.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xfq.cqqwz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dxw.sysykeji.top

================================================================================
来源：http://hqd.sysykeji.top

K. JSON 与序列化
来源：http://aow.gzhubu.top

================================================================================
来源：http://dka.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://bsr.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rny.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cdu.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://gln.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://fph.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kmp.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://sfr.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://hof.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://gup.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://som.sjlbkw.cn

Py:   json.loads(s)
来源：http://fzz.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzm.aizwys.cn

JS:   JSON.parse(s)
来源：http://flh.jyoumei.cn

TS:   JSON.parse(s)
来源：http://odq.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hjj.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://can.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://yie.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://neb.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://jbs.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tqi.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kwp.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://avu.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wqj.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dvc.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qse.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://bve.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rnr.shuidangran.top

[K04] 读取 JSON 文件
来源：http://epj.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jbf.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gux.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ion.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://see.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nsw.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nme.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kxy.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://til.zdbjq.cn

[K05] 深拷贝对象
来源：http://fod.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://jkf.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://obv.0kj1m.cn

JS:   structuredClone(obj)
来源：http://xbx.chenlongwang.top

TS:   structuredClone(obj)
来源：http://oxq.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://edj.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jcr.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsu.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cni.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://trb.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nnr.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://srx.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://txu.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jlb.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vjg.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://obi.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qsk.xuetiantiany.cn


<!-- 参考信息 -->