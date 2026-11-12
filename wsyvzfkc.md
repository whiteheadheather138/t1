代发 wailian999

JS:   class MyError extends Error {}
来源：http://voa.shuidangran.top

TS:   class MyError extends Error {}
来源：http://qhv.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://hxg.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ori.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://ihb.xziqi.cn

C#:   class MyException : Exception {}
来源：http://cfr.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://nqi.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://oea.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pwb.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://lxe.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://kut.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://cqa.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ydm.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://kod.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zkr.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://him.zycfv.cn

Py:   value = d.get("k") or default
来源：http://cru.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zls.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wun.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://inb.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ozs.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sej.yvedp.cn

Ruby: d&.dig(:a, :b)
来源：http://pkn.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://tgy.shanyushiyangtech.top

[H07] 断言
来源：http://xgq.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://gez.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://qad.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://ssx.xylfe.cn

TS:   console.assert(x > 0);
来源：http://btk.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://ase.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nnz.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://vea.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://fdv.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://zpj.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://rqs.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tfz.52xcode.cn

JS:   e.message;  e.stack
来源：http://qzt.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sma.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ona.jqgfzy.top

Go:   err.Error()
来源：http://akm.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://exz.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://vce.zdbjq.cn

[H09] 带错误码的异常
来源：http://pfg.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cql.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xmz.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jag.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zgh.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qle.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wxi.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oge.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://otj.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://xyj.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mcv.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yim.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lhy.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pde.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lps.9152youxi.cn

Go:   defer f.Close()
来源：http://uvf.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ojj.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wct.hammf.cn

================================================================================
来源：http://cvr.zhongyouzk.top

I. 正则表达式
来源：http://opz.cqqwz.cn

================================================================================
来源：http://vww.aibaodan.cn

[I01] 判断是否匹配
来源：http://vuo.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qgw.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://dzj.uphjek.com

JS:   /\d+/.test(s)
来源：http://aga.redwolf501.top

TS:   /\d+/.test(s)
来源：http://wve.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://flg.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vee.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://znx.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wim.jianghu66.top

[I02] 提取所有匹配
来源：http://isq.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://hsq.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rgg.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jmy.cashguo.top

TS:   s.match(/\d+/g)
来源：http://alu.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fdc.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bqj.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://ahu.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xub.vqdsnc.cn

[I03] 提取捕获分组
来源：http://bfe.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wdb.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uot.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ubw.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aex.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zbq.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nkj.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nog.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kkc.yongpay.top

[I04] 正则替换
来源：http://tlc.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://uec.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cdn.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://zvj.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nyw.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://xjd.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://alv.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aee.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ags.cheryme.top

[I05] 按正则拆分
来源：http://yln.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oss.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mdj.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://cfq.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://fhg.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://qqy.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bkj.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://ipr.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ups.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bfw.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ttd.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ybx.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tnl.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tpt.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://czr.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://syg.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tbp.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sjx.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://smy.ybcxt.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mkt.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://krj.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ilc.316326.xyz

TS:   /error/gim
来源：http://kru.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lgi.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mon.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://zyz.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ooy.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://kkg.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gaq.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uvk.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jyi.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rri.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hyl.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tsm.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tti.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nfb.c1oappe.top

================================================================================
来源：http://egn.pengpengdd.cyou

J. 日期与时间
来源：http://uel.zhengqikj.top

================================================================================
来源：http://eoz.shuidangran.top

[J01] 获取当前时间
来源：http://isy.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pzf.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://coi.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://pzc.daxiang520.top

TS:   new Date();  Date.now()
来源：http://wat.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://cru.shanyushiyangkeji.top

Go:   time.Now()
来源：http://zfp.hesvh.cn

Ruby: Time.now
来源：http://txa.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jll.cqqwz.cn

[J02] 格式化输出
来源：http://vcs.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yqu.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rzi.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nkw.tarul.cn

TS:   d.toISOString()
来源：http://are.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yso.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lfs.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://alw.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rkb.jyoumei.cn

[J03] 字符串解析为日期
来源：http://xbm.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fek.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cur.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://fmz.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://bmr.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ggk.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dre.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://uld.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://okh.xylfe.cn

[J04] 时间戳与日期互转
来源：http://jgx.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ivx.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eld.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xco.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bjc.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qme.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ocl.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://omo.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yzn.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://xdn.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://okn.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://kvd.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://toq.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wld.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://bwq.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kki.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://qvs.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://bfx.svipenyu.cn

[J06] 计算两时间之差
来源：http://amj.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://vfw.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://bqj.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nbr.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pqx.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://ubu.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://dhk.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://etv.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://lpw.jqgfzy.top

[J07] 比较两个日期
来源：http://lml.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://aii.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zje.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://let.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jmz.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ttz.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ana.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://kjf.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://rkh.52xcode.cn

[J08] 提取年月日与星期
来源：http://cpj.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cjr.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gwu.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nqk.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kos.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xfx.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bhg.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ogo.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jys.daxiang520.top

[J09] 时区处理
来源：http://cal.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qrp.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://psu.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rlc.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://soh.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ubl.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kkh.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hvw.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uyz.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://zfx.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kmk.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://avu.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ntk.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kyf.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sxt.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wan.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bqh.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xkk.jiagoushi.top

================================================================================
来源：http://glh.gaohongyu789.top

K. JSON 与序列化
来源：http://fzb.aibaodan.cn

================================================================================
来源：http://erk.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://nhz.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qpi.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xxr.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://kvn.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://mnb.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uge.zycfv.cn

Go:   json.Marshal(obj)
来源：http://wxe.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://oib.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vca.fengsongda.top

[K02] JSON 字符串转对象
来源：http://ozk.iojbl.cn

Py:   json.loads(s)
来源：http://gne.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmi.chenzaomai.com

JS:   JSON.parse(s)
来源：http://exv.c1oappe.top

TS:   JSON.parse(s)
来源：http://dvm.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jpq.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://pag.316326.xyz

Ruby: JSON.parse(s)
来源：http://hia.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tlq.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://sqe.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xie.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pys.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gtu.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://dny.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mch.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lfw.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://waq.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://owk.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://vtb.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qft.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lim.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://urn.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jlg.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fhr.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ctu.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xup.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hcg.dashuyun.cn

[K05] 深拷贝对象
来源：http://pua.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://tbx.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://ory.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://gfi.ybcxt.top

TS:   structuredClone(obj)
来源：http://qpx.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://bpj.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gjz.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jln.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://noc.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://gqe.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qhc.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bmv.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dzv.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kcx.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jmq.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xgv.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tcc.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ljp.havefunace.top

[K07] 进制转换
来源：http://qst.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sic.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jlp.daria6918.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gbw.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qzl.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jce.gzhubu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ola.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yuy.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qyu.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://tgi.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://bmr.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gjt.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ucx.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://pzm.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jup.fehbvm.com


<!-- 参考信息 -->