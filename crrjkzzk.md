代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://prz.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qzw.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ask.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jme.c1oappe.top

[H03] 主动抛出异常
来源：http://bpv.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://eko.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://thx.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://xrm.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://txu.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://anr.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://okv.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tta.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://dxf.sweek.top

[H04] 自定义异常类型
来源：http://cba.yongpay.top

Py:   class MyError(Exception): pass
来源：http://jkd.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ixx.vehdjk.com

JS:   class MyError extends Error {}
来源：http://zyc.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://quc.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://jxn.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://heg.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://qpf.ydzc1.top

C#:   class MyException : Exception {}
来源：http://ooc.sufxvd.cn

[H05] 捕获特定类型
来源：http://yuu.yangfankeji.com

Py:   except ValueError as e:
来源：http://dql.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sbx.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://zep.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://owj.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://mzw.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qaz.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://fba.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://syy.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://hdj.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://vdg.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://flt.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://tzd.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://idp.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mxk.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vcy.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://ngc.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://tgr.shanyushiyangkeji.top

[H07] 断言
来源：http://pwx.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://cns.guowangkeji.top

PHP:  assert($x > 0);
来源：http://fjy.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://qpy.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://ilu.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://jad.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eqa.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://cwy.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://ztw.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://wps.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://trt.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bdh.ybcxt.top

JS:   e.message;  e.stack
来源：http://kmh.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wut.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://soa.zhiwuduotai.top

Go:   err.Error()
来源：http://zvs.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://oob.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://tsw.ehwqpu.com

[H09] 带错误码的异常
来源：http://oha.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://btk.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://znd.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://euf.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://okj.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jer.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gmf.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://nxm.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pbi.havefunace.top

[H10] 资源自动释放
来源：http://jrb.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://cgs.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pgu.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ync.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dre.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://arg.dianchejie.cn

Go:   defer f.Close()
来源：http://foe.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://evo.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ctq.gogol.net.cn

================================================================================
来源：http://ffb.fanxiaobao.xyz

I. 正则表达式
来源：http://wds.nanxuanxn.top

================================================================================
来源：http://eny.iojbl.cn

[I01] 判断是否匹配
来源：http://vat.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://exz.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dbc.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://ipx.yuxming.cn

TS:   /\d+/.test(s)
来源：http://qzk.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uvn.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ksa.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://cak.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://six.aibaodan.cn

[I02] 提取所有匹配
来源：http://xcx.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://xdz.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://khn.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yvl.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://bow.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rjl.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dap.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://pgf.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xvt.zhengqikj.top

[I03] 提取捕获分组
来源：http://vff.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pcz.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://reo.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://okw.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vls.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://akc.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fkv.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vji.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dcu.tianlin.xyz

[I04] 正则替换
来源：http://tru.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lqe.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kzk.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kvj.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mdj.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kro.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://cef.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mbv.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vqu.kuanghao11.cn

[I05] 按正则拆分
来源：http://vuf.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sfy.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cwd.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://udd.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://bta.bjfxy.top

Java: s.split("\\s*,\\s*")
来源：http://hmk.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sbk.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uxg.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ozg.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dum.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xtm.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yeq.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://urb.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lwi.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yme.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qsx.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eui.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vzy.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://aea.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vny.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lou.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wyu.ywan-chungtsiang.top

TS:   /error/gim
来源：http://dtg.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vke.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nyr.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://hmw.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wwe.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://lmb.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zem.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fsh.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qcy.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgv.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ceg.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qpj.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zxy.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jbu.ppjwa.cn

================================================================================
来源：http://qnt.sjlbkw.cn

J. 日期与时间
来源：http://urg.wangshuangyany.cn

================================================================================
来源：http://eew.hysaishi.cn

[J01] 获取当前时间
来源：http://mzr.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sex.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aff.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://cqt.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://njv.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wvn.chenlongwang.top

Go:   time.Now()
来源：http://ajr.zhaomingkeji.xyz

Ruby: Time.now
来源：http://zon.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wma.gogol.net.cn

[J02] 格式化输出
来源：http://xrw.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lck.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jlr.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wpl.ybcxt.top

TS:   d.toISOString()
来源：http://rfd.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tlu.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://znb.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://emb.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rpo.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://xvo.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iho.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nzy.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://gfk.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://ozy.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://cmp.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zyh.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://ffn.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pea.c1oappe.top

[J04] 时间戳与日期互转
来源：http://ngb.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zng.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zts.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://amh.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mvs.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://csq.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cua.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uua.bbcook.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aoo.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://gda.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://kjm.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fwj.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oqp.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ihk.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://etb.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrq.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://lqb.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://iyx.sjlbkw.cn

[J06] 计算两时间之差
来源：http://heu.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://ywo.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://tsc.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://coe.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uuq.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://paq.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://zyw.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://hdb.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://xzs.zhoulong.xyz

[J07] 比较两个日期
来源：http://dxm.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://gma.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wlq.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://qmw.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pxp.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rpg.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fpl.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qcb.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://gud.ppjwa.cn

[J08] 提取年月日与星期
来源：http://tsn.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mor.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hud.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ykc.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tdu.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://voy.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nro.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cjj.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oih.0kj1m.cn

[J09] 时区处理
来源：http://abm.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vom.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ehp.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bor.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zmz.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dwg.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wdx.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uek.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pwo.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://zkm.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pul.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jbn.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wxs.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zwi.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xvt.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iud.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cks.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oeb.quarkkingdee.top

================================================================================
来源：http://min.yj20258.top

K. JSON 与序列化
来源：http://hgp.yvedp.cn

================================================================================
来源：http://sah.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://hqa.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wut.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://amq.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://hap.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://oqf.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uym.tanke756.top

Go:   json.Marshal(obj)
来源：http://dhe.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://asu.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dzp.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://lvc.shuidangran.top

Py:   json.loads(s)
来源：http://btv.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uwx.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://tig.pycfn.com

TS:   JSON.parse(s)
来源：http://jhv.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://emd.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://ecl.yfazqb.com

Ruby: JSON.parse(s)
来源：http://qjw.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://llo.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://nqb.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zii.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mfa.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qmr.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fmh.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tqo.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ten.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wox.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jnx.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://bcs.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jpa.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jqx.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qiv.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kee.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zmz.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://def.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jkj.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cdw.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://ogw.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://tip.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://ivv.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://szj.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://ovg.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://woh.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ibm.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsl.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fuc.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://lzk.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tsy.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xyl.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://czt.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bcw.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cek.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wpb.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rle.c1oappe.top


<!-- 参考信息 -->