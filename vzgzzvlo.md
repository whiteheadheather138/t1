代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jir.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://iyn.52xcode.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wwj.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://vjc.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://nmt.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://epn.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://opy.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://vvw.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ipu.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wsk.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://ijc.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://rgn.ehwqpu.com

[H07] 断言
来源：http://idl.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://rbg.zdqjudy.top

PHP:  assert($x > 0);
来源：http://rjx.nwbrower.top

JS:   console.assert(x > 0);
来源：http://qom.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://edo.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://onq.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hzs.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wle.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://srh.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://pgz.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://hdx.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://etw.tarul.cn

JS:   e.message;  e.stack
来源：http://jbp.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vag.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jac.ehwqpu.com

Go:   err.Error()
来源：http://hxv.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://gbj.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://cvu.chenlongwang.top

[H09] 带错误码的异常
来源：http://cpi.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yfj.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fjl.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fmz.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fts.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wlb.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pwv.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://ixw.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cxv.nanxinkj.top

[H10] 资源自动释放
来源：http://dsk.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rgy.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vwf.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ymz.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ywi.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jfv.fehbvm.com

Go:   defer f.Close()
来源：http://dzk.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zfm.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wnf.yuanzhike.top

================================================================================
来源：http://huk.jqgufenzy.top

I. 正则表达式
来源：http://iwx.bjfxy.top

================================================================================
来源：http://tat.dashuyun.cn

[I01] 判断是否匹配
来源：http://etu.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fkg.jlsjyb.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wve.ybcxt.top

JS:   /\d+/.test(s)
来源：http://gvf.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://ypz.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wqp.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wxz.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://xqw.jqgfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://izc.yanxiufei.cn

[I02] 提取所有匹配
来源：http://wvt.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://dec.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cvl.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jpz.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://hoi.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nix.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lcp.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://lkq.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rpl.meibo888.top

[I03] 提取捕获分组
来源：http://jim.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ivc.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sbg.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fvn.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wpp.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ilm.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kke.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dhc.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ukz.jinyuanbaomall.cn

[I04] 正则替换
来源：http://ymu.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dgd.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kxt.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://bpq.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://soy.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dsg.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ter.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qlq.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mym.shuidangran.top

[I05] 按正则拆分
来源：http://bww.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vtj.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jeu.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://juj.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://qrb.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://wow.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vhl.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://nxy.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://znp.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ofe.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wpw.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bid.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://awv.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oku.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://atx.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qco.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://udq.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hmc.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://rsb.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yjj.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bea.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://skd.hnxiangtu.top

TS:   /error/gim
来源：http://yex.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lem.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://odv.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://lqk.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vny.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://erl.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://evh.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hnh.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kwc.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zyf.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kiw.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxt.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nmn.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://myv.guowangkeji.top

================================================================================
来源：http://sza.svipenyu.cn

J. 日期与时间
来源：http://gej.shuidangran.top

================================================================================
来源：http://tgp.xylfe.cn

[J01] 获取当前时间
来源：http://zwd.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lnw.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nvr.guannengcc.top

JS:   new Date();  Date.now()
来源：http://yqh.ivvv.top

TS:   new Date();  Date.now()
来源：http://yhz.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://unq.chenlongwang.top

Go:   time.Now()
来源：http://cfh.bjfxy.top

Ruby: Time.now
来源：http://iyc.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uwg.cdnleiting.top

[J02] 格式化输出
来源：http://xql.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vez.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eao.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ixw.fehbvm.com

TS:   d.toISOString()
来源：http://xkn.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dna.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hni.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bck.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nud.smart0.xyz

[J03] 字符串解析为日期
来源：http://bva.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eek.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bmr.meibo888.top

JS:   new Date("2024-01-02")
来源：http://rbk.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://aok.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://adz.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oho.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://zdn.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ffr.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://sjm.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xce.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kcl.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mej.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cov.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zag.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kvy.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ruu.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lwo.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://nqm.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://czj.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kaj.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wpi.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ann.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://cwq.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qon.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://zzc.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://lkx.fzhhl.top

[J06] 计算两时间之差
来源：http://vpy.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://tpx.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://vkf.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://out.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hmn.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://hcs.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://cmt.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://yju.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://xgj.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://abt.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://qup.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nwf.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://fxg.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://bdx.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fbc.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aez.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lxz.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://uev.vehdjk.com

[J08] 提取年月日与星期
来源：http://zdq.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kyg.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zaz.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oot.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nlz.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fbz.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lys.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cal.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ixu.xylfe.cn

[J09] 时区处理
来源：http://mcy.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wea.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yrq.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cok.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsd.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uwc.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xim.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pgy.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mtj.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://usn.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ivb.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://djp.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cii.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qic.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cxd.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qbe.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://clo.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rji.uphjek.com

================================================================================
来源：http://djh.pengpengdd.cyou

K. JSON 与序列化
来源：http://aqh.jqgfzy.top

================================================================================
来源：http://eui.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://nfj.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mvv.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zup.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://izm.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://oqt.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://byb.bjfxy.top

Go:   json.Marshal(obj)
来源：http://sji.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://hei.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xph.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://fvu.gzhubu.top

Py:   json.loads(s)
来源：http://jgj.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eyl.hesvh.cn

JS:   JSON.parse(s)
来源：http://dmk.ctjpmb.com

TS:   JSON.parse(s)
来源：http://abr.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kqe.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://cfw.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://btz.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pmf.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://gmu.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tuh.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sxq.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dss.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://bzq.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ifl.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://axx.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://afr.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rvd.ivvv.top

[K04] 读取 JSON 文件
来源：http://bok.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://opi.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jqg.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bmx.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tkj.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ltg.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://axa.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fuz.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://szo.yueranfly.top

[K05] 深拷贝对象
来源：http://ydk.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://dae.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://rvh.ppjwa.cn

JS:   structuredClone(obj)
来源：http://qea.jinqigufen.top

TS:   structuredClone(obj)
来源：http://suh.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gvw.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://chn.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ses.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://onf.yj202588.top

[K06] 解析 URL 查询串
来源：http://bho.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rfu.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fgo.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wsf.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iwl.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mmu.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ows.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uch.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ics.kuanghao11.cn

[K07] 进制转换
来源：http://dkp.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zsb.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vgd.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nle.zhengqikj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gnm.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vvn.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kgi.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lyx.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ijf.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://guq.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://ioy.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vqs.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://vbx.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://hzo.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qwa.ehwqpu.com

Go:   encoding/gob
来源：http://frr.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://rjm.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gjb.jinqigufen.top

================================================================================
来源：http://stw.andypj.xyz

L. 网络请求
来源：http://soa.hammf.cn

================================================================================
来源：http://tph.52xcode.cn

[L01] 发送 GET 请求
来源：http://nto.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qwz.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lkw.ydjk.org.cn

JS:   await fetch(url)
来源：http://yre.yongpay.top

TS:   await fetch(url)
来源：http://srn.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eup.birdmap.top


<!-- 参考信息 -->