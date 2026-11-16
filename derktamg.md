代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qep.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://zmw.jqgfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nnz.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://ioe.epnwcf.com

Py:   value = d.get("k") or default
来源：http://jdr.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cez.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://dzl.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://opf.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wzv.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://asm.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://jto.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://qgs.jinghuilouyu.cn

[H07] 断言
来源：http://tkm.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://rje.zycfv.cn

PHP:  assert($x > 0);
来源：http://yqu.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://hna.fehbvm.com

TS:   console.assert(x > 0);
来源：http://nwm.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://xhh.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cet.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sdj.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://pym.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://tjg.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://wbm.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ffv.fehbvm.com

JS:   e.message;  e.stack
来源：http://uuw.guannengcc.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tpi.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jxf.gogol.net.cn

Go:   err.Error()
来源：http://dhk.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://xvw.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://sei.0kj1m.cn

[H09] 带错误码的异常
来源：http://mmn.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://erw.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kch.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ami.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rha.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sob.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dil.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xri.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vmb.epnwcf.com

[H10] 资源自动释放
来源：http://jrg.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nfq.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ncc.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://syv.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sfh.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qjp.cheryme.top

Go:   defer f.Close()
来源：http://ccb.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xei.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hrg.jianghu66.top

================================================================================
来源：http://pew.cheryme.top

I. 正则表达式
来源：http://tko.jinghuilouyu.cn

================================================================================
来源：http://mpw.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://voc.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jzq.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://drd.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://xmv.fktsv.cn

TS:   /\d+/.test(s)
来源：http://iky.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://raq.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wnr.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://vrx.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fvl.chenzaomai.com

[I02] 提取所有匹配
来源：http://cgh.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://iae.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qgc.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wdr.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://hlu.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sdc.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rkj.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://lcb.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://znx.meibo888.top

[I03] 提取捕获分组
来源：http://wwn.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ltm.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xec.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hiy.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ofr.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hjo.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gex.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nev.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bsm.aibaodan.cn

[I04] 正则替换
来源：http://ybw.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wzq.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fgf.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pnj.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qwn.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://mky.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qwx.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ixb.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ebe.vehdjk.com

[I05] 按正则拆分
来源：http://jba.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hlt.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nua.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://tvg.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://hty.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://ero.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://osa.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://hky.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vge.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tzl.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://weo.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kpy.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yzo.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wwg.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lpc.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lgu.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ode.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://urq.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://tir.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gtz.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dch.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gtt.wangshuangyany.cn

TS:   /error/gim
来源：http://twg.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ahd.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yht.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://zht.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oxn.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://aox.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dcz.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lmp.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xly.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://skl.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mgz.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mkm.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kgr.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fwg.cucudq.cn

================================================================================
来源：http://ktj.nwbrower.top

J. 日期与时间
来源：http://orm.aizwys.cn

================================================================================
来源：http://syo.shuidangran.top

[J01] 获取当前时间
来源：http://wqu.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iui.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rhf.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://lhc.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://gyi.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lkp.c1oappe.top

Go:   time.Now()
来源：http://sxk.bjfxy.top

Ruby: Time.now
来源：http://kfg.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pyq.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://xxb.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hen.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rqx.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://egs.yongpay.top

TS:   d.toISOString()
来源：http://uvc.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rdv.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ocx.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gkb.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vnp.316326.xyz

[J03] 字符串解析为日期
来源：http://wch.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://igi.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hra.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://mpb.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://qqd.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://bhn.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jcm.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://pvp.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ntj.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://pzw.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yui.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wil.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uzm.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dxf.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pxf.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://npg.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sfm.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gbz.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://xcj.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://bjn.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hik.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bnr.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uew.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://dhg.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lbb.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://nxx.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://pxx.nanxuanxn.top

[J06] 计算两时间之差
来源：http://bsn.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://knz.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://aju.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cya.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ibk.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://irx.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://dtb.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://qfe.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://gdd.ppjwa.cn

[J07] 比较两个日期
来源：http://hpn.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://twl.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pee.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://asp.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hnx.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hjh.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jua.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://wxt.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://udn.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://wdr.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cir.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vhw.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://atf.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cyk.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://efl.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rjh.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nge.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zua.ydjk.org.cn

[J09] 时区处理
来源：http://ita.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jei.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agy.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://amz.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://huu.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uhh.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oad.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hhq.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jnj.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://lbd.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wxc.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jhe.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://csl.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eis.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vul.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rpv.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hkd.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mau.ydjk.org.cn

================================================================================
来源：http://ujr.shanyushiyangtech.top

K. JSON 与序列化
来源：http://uxe.cqqwz.cn

================================================================================
来源：http://cpf.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://wba.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lpw.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lfw.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://wzb.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://jga.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://thn.gzhubu.top

Go:   json.Marshal(obj)
来源：http://mod.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://njm.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gps.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://atc.tianlin.xyz

Py:   json.loads(s)
来源：http://adg.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jfa.smart0.xyz

JS:   JSON.parse(s)
来源：http://esp.xuanzx.com

TS:   JSON.parse(s)
来源：http://zxk.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vlc.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://axi.hammf.cn

Ruby: JSON.parse(s)
来源：http://vou.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ulm.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ici.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bvp.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://exb.iojbl.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://opk.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://cqs.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ahf.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ajp.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://zgo.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zyq.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://gqr.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kyu.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://abh.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drp.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://log.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pwj.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://efx.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ckx.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yfu.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://msq.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://pvf.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://bnd.xziqi.cn

JS:   structuredClone(obj)
来源：http://coq.dashuyun.cn

TS:   structuredClone(obj)
来源：http://jza.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://crk.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyr.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eta.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hrv.yfazqb.com

[K06] 解析 URL 查询串
来源：http://yas.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wgj.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iuu.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wra.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dkd.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jar.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://smq.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fbk.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ugz.chenzaomai.com

[K07] 进制转换
来源：http://bkw.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pnk.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ocx.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jdq.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dhx.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rmw.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uqy.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vuz.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://exd.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://ojw.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://lxa.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nom.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://lvn.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://huz.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wyy.jyoumei.cn

Go:   encoding/gob
来源：http://lqz.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://eep.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://inu.smart0.xyz

================================================================================
来源：http://uha.sxryk.cn

L. 网络请求
来源：http://wam.sweek.top

================================================================================
来源：http://jaz.9152youxi.cn

[L01] 发送 GET 请求
来源：http://qby.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://drl.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gzt.yongpay.top

JS:   await fetch(url)
来源：http://qul.xylfe.cn

TS:   await fetch(url)
来源：http://sxd.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vgk.xuanzx.com


<!-- 参考信息 -->