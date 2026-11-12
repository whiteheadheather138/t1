代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://etl.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tnq.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eyt.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zcp.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mgs.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sro.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://fdx.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://joh.guannengcc.top

[H03] 主动抛出异常
来源：http://cfc.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://zht.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vwr.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://sev.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://qmp.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fje.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nua.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mgb.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fbl.zhongyouzk.top

[H04] 自定义异常类型
来源：http://jql.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://lyf.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://dyu.xziqi.cn

JS:   class MyError extends Error {}
来源：http://jgp.xziqi.cn

TS:   class MyError extends Error {}
来源：http://lna.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://knh.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yot.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://tvc.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://ndc.tianlin.xyz

[H05] 捕获特定类型
来源：http://hkv.pycfn.com

Py:   except ValueError as e:
来源：http://dvg.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fez.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://dzf.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://gop.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://kft.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kox.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://kqm.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sgi.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://azj.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://lla.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uin.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://qix.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://icv.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cuk.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://pzm.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://oon.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://nnf.andypj.xyz

[H07] 断言
来源：http://jla.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://bdh.jiagoushi.top

PHP:  assert($x > 0);
来源：http://wag.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://avd.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://yny.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://kfi.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mdb.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://pnx.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://izi.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://wgq.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://lll.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ysw.yonumen.top

JS:   e.message;  e.stack
来源：http://wmm.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lxe.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lrx.cashguo.top

Go:   err.Error()
来源：http://ipe.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://qbr.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://pzz.redwolf501.top

[H09] 带错误码的异常
来源：http://gfr.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jgi.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://trl.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uhb.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://utf.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rll.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cpy.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://vab.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ubq.daria6918.cn

[H10] 资源自动释放
来源：http://yof.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://dtp.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://agl.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pei.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bgu.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xtq.tarul.cn

Go:   defer f.Close()
来源：http://tyv.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xmy.zhiwuduotai.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kzx.0kj1m.cn

================================================================================
来源：http://krj.snrcjt.cn

I. 正则表达式
来源：http://wpk.tian-w.cn

================================================================================
来源：http://jwo.hnqzz.top

[I01] 判断是否匹配
来源：http://mab.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cub.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://pmp.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://ici.guannengcc.top

TS:   /\d+/.test(s)
来源：http://gnt.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sig.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ust.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://wbg.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sfv.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://cnf.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://oah.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uen.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lry.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://wof.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mit.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://try.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://boh.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dje.wangdashe.top

[I03] 提取捕获分组
来源：http://lhp.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ksi.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://snw.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://laa.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://izi.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wru.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gtl.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kra.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://thu.wangdashe.top

[I04] 正则替换
来源：http://wmy.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://zkd.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kvf.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://rlr.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://vqf.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://tuq.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wat.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://hxb.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nuy.havefunace.top

[I05] 按正则拆分
来源：http://teo.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oeu.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lxe.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://tzn.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://hoo.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://ndd.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://efd.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://six.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lfi.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wid.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bhs.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ivc.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qsd.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tlj.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://drm.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mqk.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://icj.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://box.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://aji.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bqq.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://izl.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rqp.zhixingplan.top

TS:   /error/gim
来源：http://viy.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sve.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tnq.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://fjv.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rkn.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://map.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vis.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://czq.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cad.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ncv.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://iuh.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tnh.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://duw.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qxh.wangdashe.top

================================================================================
来源：http://waz.kuanghao11.cn

J. 日期与时间
来源：http://pfd.meibo888.top

================================================================================
来源：http://zsy.tanke756.top

[J01] 获取当前时间
来源：http://kwx.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bhl.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://idc.andypj.xyz

JS:   new Date();  Date.now()
来源：http://hqs.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://ctc.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://opn.daxiang520.top

Go:   time.Now()
来源：http://fhr.meibo888.top

Ruby: Time.now
来源：http://myy.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://egk.hesvh.cn

[J02] 格式化输出
来源：http://lex.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bsd.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zhq.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wmc.tianlin.xyz

TS:   d.toISOString()
来源：http://bms.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rox.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xul.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gjg.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cnn.ehwqpu.com

[J03] 字符串解析为日期
来源：http://rmi.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vrg.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lnj.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://vfo.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://tga.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kvl.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eim.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://yvb.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxz.shuidangran.top

[J04] 时间戳与日期互转
来源：http://ckf.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bfp.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lqu.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://myp.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://eva.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cyj.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://icj.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bij.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zrs.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://mky.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://vsk.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://ejr.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iwe.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zyi.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://kaj.ehwqpu.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://min.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://que.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ufh.sxryk.cn

[J06] 计算两时间之差
来源：http://txr.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://dvs.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://xnv.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mgo.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://clo.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dty.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://zzf.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://pbj.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://gey.iojbl.cn

[J07] 比较两个日期
来源：http://iff.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://bwm.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gdg.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xcz.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bvg.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wkj.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://snk.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://edy.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://iiu.gotoacloud.top

[J08] 提取年月日与星期
来源：http://ecn.hnxiangtu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ghi.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bor.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wym.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dqd.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fwy.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qqj.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zqw.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xig.jinghuilouyu.cn

[J09] 时区处理
来源：http://jsi.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dcc.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mos.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mxn.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chv.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fpy.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zdt.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://thl.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kgz.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://zls.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eox.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://afe.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gcf.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://stl.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vvi.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qbj.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jmv.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xsg.chenlongwang.top

================================================================================
来源：http://goh.nanxinkj.top

K. JSON 与序列化
来源：http://dzy.zdqjudy.top

================================================================================
来源：http://brm.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://gsc.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aym.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gde.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://wuv.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://mht.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ihd.ydzc1.top

Go:   json.Marshal(obj)
来源：http://ujx.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://lep.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yza.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://lnb.zhixingplan.top

Py:   json.loads(s)
来源：http://nsw.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rtq.hammf.cn

JS:   JSON.parse(s)
来源：http://tzk.hnqzz.top

TS:   JSON.parse(s)
来源：http://ndw.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kau.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://lbw.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://gxi.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tit.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://klz.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uuz.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rnq.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zfe.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wqz.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hug.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aan.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://grt.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tqe.xinyue.icu

[K04] 读取 JSON 文件
来源：http://qmq.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rup.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sfz.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://taa.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://thm.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uaj.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qrm.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://trq.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yuz.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://xch.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://ikv.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://ved.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://gas.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://uqt.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wii.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://htm.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sic.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rqc.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://ndk.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mtr.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ceo.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xiy.gaohongyu789.top


<!-- 参考信息 -->