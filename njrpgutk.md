代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://yot.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jgc.jqgfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hly.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gaj.nwbrower.top

[H03] 主动抛出异常
来源：http://xuo.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://pnx.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ead.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://fqg.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://zaq.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gyn.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ltp.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://pkj.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cxy.zhengqikj.top

[H04] 自定义异常类型
来源：http://udz.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://mae.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://mtc.meibo888.top

JS:   class MyError extends Error {}
来源：http://zkb.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://ucs.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://xjc.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://biv.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://pol.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://qry.zhongyouzk.top

[H05] 捕获特定类型
来源：http://eln.sjlbkw.cn

Py:   except ValueError as e:
来源：http://aqq.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kmr.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://yea.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://zmq.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://bjz.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xka.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://oxk.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qgr.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://ntq.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://dms.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://otq.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://qhj.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://zwb.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yme.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://guk.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://lpz.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://qdw.c1oappe.top

[H07] 断言
来源：http://ape.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://iwm.yj20258.top

PHP:  assert($x > 0);
来源：http://keo.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://rtf.ybcxt.top

TS:   console.assert(x > 0);
来源：http://bib.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://zdr.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nbt.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mxr.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://ohs.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://ngv.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ihc.nanxuanxn.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://anq.9152youxi.cn

JS:   e.message;  e.stack
来源：http://mrw.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qdu.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uhe.cqqwz.cn

Go:   err.Error()
来源：http://lnj.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://ers.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://rvk.yangfankeji.com

[H09] 带错误码的异常
来源：http://fmt.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jyq.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pjz.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nil.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://edt.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zll.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://udm.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vwz.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://jzb.nanxinkj.top

[H10] 资源自动释放
来源：http://hyf.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aja.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uxw.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yal.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dzl.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lwy.feifeiyinyue.top

Go:   defer f.Close()
来源：http://zsh.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xpf.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sfu.feifeiyinyue.top

================================================================================
来源：http://pay.vqdsnc.cn

I. 正则表达式
来源：http://vvc.hnxiangtu.top

================================================================================
来源：http://dsc.aibaodan.cn

[I01] 判断是否匹配
来源：http://whv.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fic.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://shy.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://pwm.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://oba.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nck.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fqx.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://tcr.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lzl.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://xfg.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://ela.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ivd.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nqx.ivvv.top

TS:   s.match(/\d+/g)
来源：http://rxw.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cbk.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wre.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://imr.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cni.yvedp.cn

[I03] 提取捕获分组
来源：http://jar.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xur.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://trc.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ctx.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kbi.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pdx.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://snz.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kzb.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dof.yj20258888.top

[I04] 正则替换
来源：http://vam.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://djp.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ndm.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://kne.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://pxl.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pjr.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ybo.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://reu.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wkr.fktsv.cn

[I05] 按正则拆分
来源：http://emk.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://zdh.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nsg.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://ehm.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://ftc.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://dmx.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vgm.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wyb.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nmp.pengpengdd.cyou

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xlh.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://liq.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oxh.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpg.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uvl.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kjh.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ltx.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tdr.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wcg.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://cke.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://krh.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ixi.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vdr.smart0.xyz

TS:   /error/gim
来源：http://zcp.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jzx.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qqw.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://aah.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bga.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://pnz.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qcp.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://waa.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uip.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wdn.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qvt.ybcxt.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bim.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gga.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mvw.kuanghao11.cn

================================================================================
来源：http://twk.ywan-chungtsiang.top

J. 日期与时间
来源：http://ezu.jqgfzy.top

================================================================================
来源：http://eod.hnqzz.top

[J01] 获取当前时间
来源：http://tsx.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uej.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cik.ybcxt.top

JS:   new Date();  Date.now()
来源：http://hbo.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://afu.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tfk.xinyue.icu

Go:   time.Now()
来源：http://ndj.dianchejie.cn

Ruby: Time.now
来源：http://rrn.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ymw.tarul.cn

[J02] 格式化输出
来源：http://aib.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dtd.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aic.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fvr.cucudq.cn

TS:   d.toISOString()
来源：http://ojl.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rdr.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hxm.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://whq.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://omm.sxryk.cn

[J03] 字符串解析为日期
来源：http://ixv.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lmp.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pyo.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://ivb.uphjek.com

TS:   new Date("2024-01-02")
来源：http://pgk.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://puu.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iyg.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://yrr.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jbu.tanke756.top

[J04] 时间戳与日期互转
来源：http://zbu.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://slq.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://meb.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xox.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mob.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zzv.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lwd.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://str.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://djn.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://rzt.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://zoj.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://szm.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gwm.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bep.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://aht.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cxk.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://fwr.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dzj.meibo888.top

[J06] 计算两时间之差
来源：http://who.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://sdf.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://gfz.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oiw.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fiu.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://tpc.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://oln.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://yai.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://nfh.ivvv.top

[J07] 比较两个日期
来源：http://cfh.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://foh.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vml.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cwf.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://scc.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aot.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bqx.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://rzf.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://ubb.yvedp.cn

[J08] 提取年月日与星期
来源：http://cst.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kjw.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ssy.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sqz.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://suj.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://upk.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kkk.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bno.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cyo.fzhhl.top

[J09] 时区处理
来源：http://yhx.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cum.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dqg.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lxp.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gvn.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mwk.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://red.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nno.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zkn.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://fwh.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cyc.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pya.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nfi.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zjn.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zrc.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lqo.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bki.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vjz.gogol.net.cn

================================================================================
来源：http://zex.yj20258888.top

K. JSON 与序列化
来源：http://loz.uphjek.com

================================================================================
来源：http://qqm.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://dze.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qkb.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zay.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://cvr.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://wrd.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://njp.yvedp.cn

Go:   json.Marshal(obj)
来源：http://iyr.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://isp.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gby.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://kni.yanxiufei.cn

Py:   json.loads(s)
来源：http://pbz.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wsz.yonumen.top

JS:   JSON.parse(s)
来源：http://rcz.yonumen.top

TS:   JSON.parse(s)
来源：http://hti.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jau.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://hrw.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://dzz.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pro.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://kuh.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rgt.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xrm.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kea.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mwh.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ycw.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hip.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ekg.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hkw.jianghu66.top

[K04] 读取 JSON 文件
来源：http://ici.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yzp.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nzn.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ztt.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwy.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eun.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yqx.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://xwm.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pvs.bjfxy.top

[K05] 深拷贝对象
来源：http://amt.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://wvf.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://qeq.hammf.cn

JS:   structuredClone(obj)
来源：http://tkn.gogol.net.cn

TS:   structuredClone(obj)
来源：http://ppk.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kfp.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://igu.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qyg.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://wen.hcnkem.com

[K06] 解析 URL 查询串
来源：http://jfx.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lnm.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://crn.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hcn.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sod.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fol.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wec.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oet.jinqigfzy.top


<!-- 参考信息 -->