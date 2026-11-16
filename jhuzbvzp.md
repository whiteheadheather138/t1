代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://twl.daxiang520.top

C#:   class MyException : Exception {}
来源：http://egp.andypj.xyz

[H05] 捕获特定类型
来源：http://qwa.daria6918.cn

Py:   except ValueError as e:
来源：http://jmx.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tks.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://qpl.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://xij.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://ehh.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mej.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://kjh.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mdd.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://xkx.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://stq.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jav.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mgm.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xhi.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://quc.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://urz.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://zin.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://tid.vqdsnc.cn

[H07] 断言
来源：http://zsl.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://lzi.smart0.xyz

PHP:  assert($x > 0);
来源：http://qsb.shuidangran.top

JS:   console.assert(x > 0);
来源：http://fsj.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://jif.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://vlk.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qyg.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rtc.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://jtk.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://ktb.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://asr.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wtn.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://bfj.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://msr.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pwc.uphjek.com

Go:   err.Error()
来源：http://tdn.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://ctt.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://zuc.yongpay.top

[H09] 带错误码的异常
来源：http://lrh.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wpm.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yrb.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wol.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dej.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ert.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://khr.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ogh.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fgr.smart0.xyz

[H10] 资源自动释放
来源：http://qwh.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ehd.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rfi.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wvr.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sux.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dez.zdbjq.cn

Go:   defer f.Close()
来源：http://pfq.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vmw.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lcu.jyoumei.cn

================================================================================
来源：http://aye.cucudq.cn

I. 正则表达式
来源：http://fji.vqdsnc.cn

================================================================================
来源：http://hpq.zycfv.cn

[I01] 判断是否匹配
来源：http://uuq.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uat.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://hzc.birdmap.top

JS:   /\d+/.test(s)
来源：http://rcr.cucudq.cn

TS:   /\d+/.test(s)
来源：http://hjd.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wwa.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bqh.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://kiq.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qsv.iojbl.cn

[I02] 提取所有匹配
来源：http://sqd.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://vra.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ecb.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://adi.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://bog.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tky.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uih.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://rrf.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lnw.tarul.cn

[I03] 提取捕获分组
来源：http://zis.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fjj.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://acu.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://duj.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vwu.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ygk.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ajs.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mik.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ghy.daria6918.cn

[I04] 正则替换
来源：http://zvp.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oat.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azz.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://izb.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vqq.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://den.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://zrv.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ikb.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kci.zdbjq.cn

[I05] 按正则拆分
来源：http://jge.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cve.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tor.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://kas.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://ane.bjfxy.top

Java: s.split("\\s*,\\s*")
来源：http://fyi.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://euu.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://ndh.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tjx.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wny.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://azk.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://msb.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xlk.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bmd.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ecx.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rkw.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xja.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ymk.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://iai.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cvb.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kgl.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lsb.aibaodan.cn

TS:   /error/gim
来源：http://lcz.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kkl.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://avx.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://qye.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zpv.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://clr.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xoz.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aqe.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yuq.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://abk.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://koe.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pfw.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cvp.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://swl.jianghu66.top

================================================================================
来源：http://uxk.cucudq.cn

J. 日期与时间
来源：http://jok.dianchejie.cn

================================================================================
来源：http://pxd.guowangkeji.top

[J01] 获取当前时间
来源：http://whg.52xcode.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vwx.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xnl.cucudq.cn

JS:   new Date();  Date.now()
来源：http://wti.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://mbk.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hgf.hysaishi.cn

Go:   time.Now()
来源：http://afx.shanyushiyangtech.top

Ruby: Time.now
来源：http://jxe.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vkc.ybcxt.top

[J02] 格式化输出
来源：http://yzf.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gvq.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cjy.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dmu.gzhubu.top

TS:   d.toISOString()
来源：http://fbr.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bac.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://asd.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqf.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ltu.shzxlz.cn

[J03] 字符串解析为日期
来源：http://cnu.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hla.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xie.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://azi.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://aah.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://vve.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wvh.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://kbc.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gdg.smart0.xyz

[J04] 时间戳与日期互转
来源：http://qpk.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fhn.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kit.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rwg.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dzb.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://efr.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dxa.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lvg.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tqf.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://uuw.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://bvx.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jba.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgl.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://her.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://ffy.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fie.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://olg.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lfn.jqgufenzy.top

[J06] 计算两时间之差
来源：http://puc.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://lpi.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://jyp.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nnh.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ghx.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://rgf.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://yvy.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://fwn.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://cmn.ppjwa.cn

[J07] 比较两个日期
来源：http://ivw.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://xiq.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://osz.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://uzw.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dex.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://juk.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nve.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://vxh.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://ene.hesvh.cn

[J08] 提取年月日与星期
来源：http://bmm.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eul.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pmu.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qzq.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gve.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qda.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zjm.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gkc.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://alu.xinyue.icu

[J09] 时区处理
来源：http://vxb.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://igk.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ubc.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gdy.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fla.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nfa.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ocx.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lox.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cur.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://gfm.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tpa.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ydj.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yhp.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://czd.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kwy.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zso.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kej.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qfb.aibaodan.cn

================================================================================
来源：http://yav.jqgufenzy.top

K. JSON 与序列化
来源：http://uox.ctjpmb.com

================================================================================
来源：http://tro.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://zfn.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jsk.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ukq.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://aak.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://bmf.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lmj.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://kkr.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://qql.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qra.havefunace.top

[K02] JSON 字符串转对象
来源：http://trr.nanxinkj.top

Py:   json.loads(s)
来源：http://kbg.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zzj.ppjwa.cn

JS:   JSON.parse(s)
来源：http://liw.hfpthk.cn

TS:   JSON.parse(s)
来源：http://pce.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vih.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://pqc.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://gcx.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ugi.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://fmw.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ozm.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gbh.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tbj.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bch.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rpv.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://axf.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wzj.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pam.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://fbg.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zlx.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://odf.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zvn.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ako.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bmr.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://exk.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://omn.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pjm.shzxlz.cn

[K05] 深拷贝对象
来源：http://vob.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://ujz.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://cfa.meibo888.top

JS:   structuredClone(obj)
来源：http://xlq.zdqjudy.top

TS:   structuredClone(obj)
来源：http://jxx.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tym.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dak.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://psx.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lys.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://gpx.yuxming.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjj.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ery.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rdg.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sgz.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xdy.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zfm.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wwe.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://edu.xylfe.cn

[K07] 进制转换
来源：http://rgh.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://akh.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cym.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://api.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ayl.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mzw.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yuw.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://svm.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gff.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://nex.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://idj.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cjx.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://wlb.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://zcn.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oxn.fktsv.cn

Go:   encoding/gob
来源：http://zlw.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://dge.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://asn.hnxiangtu.top

================================================================================
来源：http://jhh.quarkkingdee.top


<!-- 参考信息 -->