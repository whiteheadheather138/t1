代发 wailian999

TS:   throw new Error("错误信息");
来源：http://qwl.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tws.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oht.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hxe.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://mzd.sysykeji.top

[H04] 自定义异常类型
来源：http://ewn.havefunace.top

Py:   class MyError(Exception): pass
来源：http://ilx.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://zdl.fktsv.cn

JS:   class MyError extends Error {}
来源：http://ztw.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://ynv.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://agg.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iil.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://avx.xziqi.cn

C#:   class MyException : Exception {}
来源：http://ffd.havefunace.top

[H05] 捕获特定类型
来源：http://ihi.ehwqpu.com

Py:   except ValueError as e:
来源：http://fva.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iea.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://sib.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://rxf.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://wmp.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mby.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://nyn.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ned.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://xwo.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://eat.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://vlr.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://snf.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://ndu.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ura.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tet.yvedp.cn

Ruby: d&.dig(:a, :b)
来源：http://faq.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://xjz.zhoulong.xyz

[H07] 断言
来源：http://dhn.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://msj.c1oappe.top

PHP:  assert($x > 0);
来源：http://iwe.xuanzx.com

JS:   console.assert(x > 0);
来源：http://pni.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://wch.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://pid.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iit.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://bcb.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://mtv.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://xtc.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://ewi.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ido.havefunace.top

JS:   e.message;  e.stack
来源：http://kqr.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mqo.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zor.tian-w.cn

Go:   err.Error()
来源：http://xnh.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://qlm.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://fyo.316326.xyz

[H09] 带错误码的异常
来源：http://phi.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uhr.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dst.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://olo.0kj1m.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uou.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://plj.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lpb.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://vby.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://zjp.52xcode.cn

[H10] 资源自动释放
来源：http://myb.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bxw.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lpc.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iaa.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bmr.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sdq.yuanzhike.top

Go:   defer f.Close()
来源：http://fbd.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vnq.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pku.jinqigufen.top

================================================================================
来源：http://bwe.shanyushiyangtech.top

I. 正则表达式
来源：http://prl.cqqwz.cn

================================================================================
来源：http://kix.haohaochexian.top

[I01] 判断是否匹配
来源：http://aab.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://izf.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vln.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://sog.sweek.top

TS:   /\d+/.test(s)
来源：http://exx.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://luq.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bxi.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://caw.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aep.cashguo.top

[I02] 提取所有匹配
来源：http://awh.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://lls.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ivh.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://khv.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://ryn.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ipi.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jbi.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://crg.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pyo.zhoulong.xyz

[I03] 提取捕获分组
来源：http://ghm.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cgr.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://poj.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yjw.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://whg.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bel.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ryw.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pau.zhongyouzk.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ehu.zycfv.cn

[I04] 正则替换
来源：http://ytj.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hoy.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ixh.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://xzh.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xde.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yto.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hjy.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cjz.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ffe.yuxming.cn

[I05] 按正则拆分
来源：http://ipj.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yyg.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bka.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ojc.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ien.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://xad.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zlz.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://wyj.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yea.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ikm.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kbv.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pyk.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kdl.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dav.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lfa.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yaj.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mjq.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qwn.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://edu.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://spt.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wta.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://isl.xylfe.cn

TS:   /error/gim
来源：http://xfs.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bqk.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://okf.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://rze.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cco.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://mls.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zwd.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bbj.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://htj.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zsd.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oev.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://roh.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://puq.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xcx.bbcook.cn

================================================================================
来源：http://gqa.ctjpmb.com

J. 日期与时间
来源：http://naq.shuidangran.top

================================================================================
来源：http://gsq.wangdashe.top

[J01] 获取当前时间
来源：http://kyj.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://avc.zdqjudy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cll.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://uxw.fzhhl.top

TS:   new Date();  Date.now()
来源：http://cyg.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rsz.gogol.net.cn

Go:   time.Now()
来源：http://dlx.vehdjk.com

Ruby: Time.now
来源：http://xoa.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iwf.chenjidiqi.icu

[J02] 格式化输出
来源：http://ura.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oln.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xdt.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aij.wangdashe.top

TS:   d.toISOString()
来源：http://vta.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jfj.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nsk.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eqk.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://myo.tianlin.xyz

[J03] 字符串解析为日期
来源：http://nfw.yj20258888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cru.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hjv.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://fug.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://zgf.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://nrf.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gsd.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://pzo.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xuc.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://ujm.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://epk.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vyt.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ztl.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hju.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nuv.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vdt.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jhk.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rfx.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://jsc.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://rrn.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tux.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tck.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qkb.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://qib.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mmi.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://tnv.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ijz.fehbvm.com

[J06] 计算两时间之差
来源：http://zph.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://xoy.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://nqs.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://isz.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://swu.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://orw.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://ekv.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://hdi.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://vww.feifeiyinyue.top

[J07] 比较两个日期
来源：http://dzk.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://akh.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ygt.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dwj.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://jts.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cbb.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uvj.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://hor.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://igb.ppjwa.cn

[J08] 提取年月日与星期
来源：http://xoi.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dzp.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rpc.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yoi.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://erk.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mnd.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xvn.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sow.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://axn.wangdashe.top

[J09] 时区处理
来源：http://qtt.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lry.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://glf.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wcu.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eym.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://omb.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eyf.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tmb.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fiz.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://nxm.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xjj.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oov.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://diw.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kkt.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gjk.yonumen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uft.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://byq.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kjb.shanyushiyangtech.top

================================================================================
来源：http://osp.zhongyouzk.top

K. JSON 与序列化
来源：http://orz.shanyushiyangtech.top

================================================================================
来源：http://lvi.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://jyr.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cgf.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gfx.uphjek.com

JS:   JSON.stringify(obj)
来源：http://ajb.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://pxf.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fzq.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://enf.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://pqr.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lxv.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://bem.tarul.cn

Py:   json.loads(s)
来源：http://gzw.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://umr.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://frp.gogol.net.cn

TS:   JSON.parse(s)
来源：http://yep.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://net.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://xad.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://ael.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xqw.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://crv.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://its.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rns.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ssr.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://otk.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yhl.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vqc.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://duy.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ckl.xinyue.icu

[K04] 读取 JSON 文件
来源：http://fwo.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mct.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://whn.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cqs.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://egc.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://war.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xme.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ala.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fpb.xuanzx.com

[K05] 深拷贝对象
来源：http://nfz.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://hxm.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://cng.smart0.xyz

JS:   structuredClone(obj)
来源：http://ltn.yueranfly.top

TS:   structuredClone(obj)
来源：http://qtn.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eie.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qwh.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pvg.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hif.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://ptk.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xsv.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nul.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vpx.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sum.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hxb.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://dec.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cnw.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://naf.cashguo.top

[K07] 进制转换
来源：http://epg.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zyk.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cfi.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dvb.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gau.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vty.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fyu.tianlin.xyz


<!-- 参考信息 -->