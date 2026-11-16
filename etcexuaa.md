代发 wailian999

Py:   value = d.get("k") or default
来源：http://rxh.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://jhb.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://eja.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://byt.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vrg.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ajz.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://jpv.meibo888.top

C#:   obj?.A?.B ?? default
来源：http://wdr.cheryme.top

[H07] 断言
来源：http://rzb.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://vmw.zycfv.cn

PHP:  assert($x > 0);
来源：http://sha.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://xrn.yonumen.top

TS:   console.assert(x > 0);
来源：http://gcx.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://ahq.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fze.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://nrb.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://jru.cqqwz.cn

[H08] 获取错误信息与堆栈
来源：http://nul.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://uyn.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blr.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://nra.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ccq.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rxm.zhijiandao.cn

Go:   err.Error()
来源：http://jam.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://wcp.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://wjo.gogol.net.cn

[H09] 带错误码的异常
来源：http://tbm.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kri.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oph.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mfl.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qll.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ill.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rsj.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ltu.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://utl.tian-w.cn

[H10] 资源自动释放
来源：http://kyb.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lqu.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gtg.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pal.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rug.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iul.guannengcc.top

Go:   defer f.Close()
来源：http://bne.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://teq.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mzu.wangdashe.top

================================================================================
来源：http://qxt.zhixingplan.top

I. 正则表达式
来源：http://obk.jyoumei.cn

================================================================================
来源：http://zkk.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://det.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wqf.jlsjyb.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zwy.tanke756.top

JS:   /\d+/.test(s)
来源：http://gtm.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://wck.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tgw.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://phe.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://ogd.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wtr.svipenyu.cn

[I02] 提取所有匹配
来源：http://nok.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://pxg.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hrq.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://crz.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://jlb.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pna.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ypy.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://pko.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ahi.jyoumei.cn

[I03] 提取捕获分组
来源：http://wfl.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sdj.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cme.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qvt.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rhd.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rwz.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yfj.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sro.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nfy.feifeiyinyue.top

[I04] 正则替换
来源：http://zqb.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://tkh.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zfr.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://uwv.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rep.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sxq.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pma.ydzc1.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rfw.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qag.mhx1999.top

[I05] 按正则拆分
来源：http://cir.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mnf.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rct.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://dqk.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://xvd.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://emf.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yni.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hbp.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pqu.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bjh.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://quj.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hsp.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gtg.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qfr.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://axh.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mli.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uqd.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cpm.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://bhp.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ryg.xziqi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://etw.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cpm.jianghu66.top

TS:   /error/gim
来源：http://ccu.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cld.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zmn.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://kou.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://asi.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://unv.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eiy.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tng.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxv.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://klt.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wli.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wmt.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://msd.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eek.hongshengwenyu.top

================================================================================
来源：http://xbq.jqgfzy.top

J. 日期与时间
来源：http://wit.fehbvm.com

================================================================================
来源：http://has.snrcjt.cn

[J01] 获取当前时间
来源：http://iqy.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cby.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mzl.sweek.top

JS:   new Date();  Date.now()
来源：http://yws.hcnkem.com

TS:   new Date();  Date.now()
来源：http://mbl.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jhh.tian-w.cn

Go:   time.Now()
来源：http://jma.ybcxt.top

Ruby: Time.now
来源：http://uds.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tkg.snrcjt.cn

[J02] 格式化输出
来源：http://hhs.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cax.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lgp.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uuz.jiagoushi.top

TS:   d.toISOString()
来源：http://kqx.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hkf.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jjc.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iid.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vpy.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://ujv.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rco.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wcf.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://res.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://lfb.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ufr.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eop.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://jmv.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jhz.yj202588.top

[J04] 时间戳与日期互转
来源：http://car.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iiv.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rwu.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wpi.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lfe.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://szf.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iye.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://omx.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://edl.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://dhl.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://edc.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ksl.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mjj.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://awg.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://cvy.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mcm.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://ysk.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://mne.zhijiandao.cn

[J06] 计算两时间之差
来源：http://evh.tarul.cn

Py:   (end - start).total_seconds()
来源：http://tdq.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://vew.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://esk.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://okq.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://vow.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://cvr.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://nuz.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://ovl.52xcode.cn

[J07] 比较两个日期
来源：http://gvz.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://yvj.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rja.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://mvc.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nei.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zjx.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vsx.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://tok.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://svp.jianghu66.top

[J08] 提取年月日与星期
来源：http://wpl.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uev.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kzu.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iac.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pvz.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ttq.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xxu.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ddo.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vyp.daria6918.cn

[J09] 时区处理
来源：http://elr.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vah.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://opv.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wiw.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ghq.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cfq.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mrw.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ady.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nxf.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://wia.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ixp.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wcw.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eax.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dia.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://elc.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ogb.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gti.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dpj.sjlbkw.cn

================================================================================
来源：http://rdx.zhixingplan.top

K. JSON 与序列化
来源：http://ynd.fengsongda.top

================================================================================
来源：http://per.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://src.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iak.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sdc.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://hgs.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://kge.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fat.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://rpt.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://bri.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qof.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://cau.haohaochexian.top

Py:   json.loads(s)
来源：http://wiu.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gqh.9152youxi.cn

JS:   JSON.parse(s)
来源：http://qre.bbcook.cn

TS:   JSON.parse(s)
来源：http://rpf.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ofb.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://vup.tarul.cn

Ruby: JSON.parse(s)
来源：http://gbl.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bwu.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://jzm.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gpt.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dlh.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fsa.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uao.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uqj.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yhl.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ave.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fpn.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://hxp.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zau.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jyo.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yit.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nhx.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qjk.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mzg.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vtv.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://duw.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://ycs.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://phm.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://lgm.jianghu66.top

JS:   structuredClone(obj)
来源：http://qji.smart0.xyz

TS:   structuredClone(obj)
来源：http://pat.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tjq.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xnn.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ilh.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ymo.52xcode.cn

[K06] 解析 URL 查询串
来源：http://jyt.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cjy.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ciq.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://run.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yxs.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hku.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pjo.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pjj.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kiu.uphjek.com

[K07] 进制转换
来源：http://pji.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iaw.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tqp.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qen.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vxb.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mon.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uuk.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ryb.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://plw.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://esd.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://yxd.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dpu.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://slf.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://doy.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://era.yvedp.cn

Go:   encoding/gob
来源：http://gjz.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://rvt.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://axx.hysaishi.cn

================================================================================
来源：http://mtd.cashguo.top

L. 网络请求
来源：http://gib.zhongyouzk.top

================================================================================
来源：http://xvm.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://tkl.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tks.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ybu.yj20258.top

JS:   await fetch(url)
来源：http://lro.hnqzz.top

TS:   await fetch(url)
来源：http://ucl.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gfd.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://szo.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zew.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hns.fengsongda.top

[L02] 发送 POST JSON
来源：http://wsw.haohaochexian.top


<!-- 参考信息 -->