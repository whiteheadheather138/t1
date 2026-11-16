代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://izv.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ajs.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://kyw.dianchejie.cn

C#:   obj?.A?.B ?? default
来源：http://zan.c1oappe.top

[H07] 断言
来源：http://ghw.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://iwv.chenlongwang.top

PHP:  assert($x > 0);
来源：http://usk.316326.xyz

JS:   console.assert(x > 0);
来源：http://pgv.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://ope.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://pvj.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ejm.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hre.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://kjj.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://dss.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://odx.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cco.tarul.cn

JS:   e.message;  e.stack
来源：http://pge.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ykv.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://aae.jyoumei.cn

Go:   err.Error()
来源：http://wxe.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://cof.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://htm.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://gmy.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ogb.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ihb.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://itu.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ffn.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffq.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://elf.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://izt.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://foc.hcnkem.com

[H10] 资源自动释放
来源：http://zhn.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://btd.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vmc.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lzj.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pke.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bxh.yanxiufei.cn

Go:   defer f.Close()
来源：http://gda.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://phd.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xwk.c1oappe.top

================================================================================
来源：http://gnx.quarkkingdee.top

I. 正则表达式
来源：http://xlx.hfpthk.cn

================================================================================
来源：http://lzm.sufxvd.cn

[I01] 判断是否匹配
来源：http://nba.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://svb.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sdp.316326.xyz

JS:   /\d+/.test(s)
来源：http://jgi.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://xtt.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ljd.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dhl.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://phg.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gfg.hnqzz.top

[I02] 提取所有匹配
来源：http://bqi.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://acj.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://laz.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hvp.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://peh.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ojf.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gxb.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://zhb.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ymk.sysykeji.top

[I03] 提取捕获分组
来源：http://itc.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rig.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pmy.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kpe.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vwp.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tjc.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zyp.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pvv.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ysn.zhaomingkeji.xyz

[I04] 正则替换
来源：http://fsz.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jwr.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gmf.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://wiq.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://hqc.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://bdo.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ecy.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mra.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cdc.yuanzhike.top

[I05] 按正则拆分
来源：http://wxk.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hqj.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pev.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://csv.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://gvq.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://eby.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wds.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://dkv.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jma.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hjp.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oby.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rvz.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdd.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nvn.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ozu.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://exz.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uxb.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jlr.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://esn.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nbr.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tlr.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rcv.ybcxt.top

TS:   /error/gim
来源：http://iho.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iia.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jjn.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://lxu.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ahb.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://pin.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rci.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yig.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwl.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hqm.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://kuz.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://acf.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nzs.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rqn.jqgfzy.top

================================================================================
来源：http://sum.xylfe.cn

J. 日期与时间
来源：http://vrh.ctjpmb.com

================================================================================
来源：http://jtx.dashuyun.cn

[J01] 获取当前时间
来源：http://ans.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oez.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://onh.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://wyw.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://yog.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yjz.jinqigfzy.top

Go:   time.Now()
来源：http://yyw.jqgufenzy.top

Ruby: Time.now
来源：http://jru.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://exe.jlsjyb.cn

[J02] 格式化输出
来源：http://exk.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hze.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://avi.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lrb.wangshuangyany.cn

TS:   d.toISOString()
来源：http://yig.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kxr.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ypa.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iaz.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zqy.316326.xyz

[J03] 字符串解析为日期
来源：http://xka.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tqm.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://clq.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://vhm.uphjek.com

TS:   new Date("2024-01-02")
来源：http://yjb.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://pud.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://syl.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://adk.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ujr.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://mxr.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ywu.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wbi.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lak.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qci.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xpp.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hty.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wdd.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rej.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://ujl.meibo888.top

Py:   now + timedelta(days=7)
来源：http://vqi.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dme.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://idz.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tfn.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://byx.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://air.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://wef.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ymk.52xcode.cn

[J06] 计算两时间之差
来源：http://gkz.yj202588.top

Py:   (end - start).total_seconds()
来源：http://jyi.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://umt.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://enx.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cgy.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://kyl.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://uns.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://djl.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://tpk.tian-w.cn

[J07] 比较两个日期
来源：http://vtx.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://kqy.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hvs.yj202588.top

JS:   d1.getTime() < d2.getTime()
来源：http://xof.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://vpr.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sil.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yji.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://byd.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://pag.nanxinkj.top

[J08] 提取年月日与星期
来源：http://ydz.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uml.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xce.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lrl.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vzu.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yja.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hih.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qso.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idt.ywan-chungtsiang.top

[J09] 时区处理
来源：http://sjq.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cxs.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ypq.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oqd.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://swa.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vdc.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cpj.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hmu.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ugq.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://zpc.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vcq.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bfz.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wdp.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wdt.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nxf.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pca.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jct.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mlg.chenlongwang.top

================================================================================
来源：http://vxa.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://nwm.gogol.net.cn

================================================================================
来源：http://kat.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://tvu.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jts.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rue.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://idx.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://amd.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ltn.jianghu66.top

Go:   json.Marshal(obj)
来源：http://jju.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://gpz.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bqo.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://iew.yj20258888.top

Py:   json.loads(s)
来源：http://xpc.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ing.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://nqe.yj20258888.top

TS:   JSON.parse(s)
来源：http://qgp.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lqg.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://ibd.pycfn.com

Ruby: JSON.parse(s)
来源：http://qqk.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yup.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://zje.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jir.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://njh.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cyi.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wve.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mic.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fgs.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://evc.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wib.c1oappe.top

[K04] 读取 JSON 文件
来源：http://fwv.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eiw.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tec.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wpe.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fse.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qip.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://naq.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qpz.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rmx.zhoulong.xyz

[K05] 深拷贝对象
来源：http://tln.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://kja.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://skc.andypj.xyz

JS:   structuredClone(obj)
来源：http://ruh.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://wpd.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://rsh.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nni.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hgd.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://gqy.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://fmd.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mht.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tqm.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qfs.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lup.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yko.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bzk.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oaf.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bxy.cashguo.top

[K07] 进制转换
来源：http://wsy.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mss.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cbx.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hom.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xfz.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qku.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wwj.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fsc.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cva.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://sid.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://azn.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eqe.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://fgt.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://zto.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wvh.chenlongwang.top

Go:   encoding/gob
来源：http://mir.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://mjk.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mkr.zdbjq.cn

================================================================================
来源：http://nyj.0kj1m.cn

L. 网络请求
来源：http://saf.ywan-chungtsiang.top

================================================================================
来源：http://sfr.ctjpmb.com

[L01] 发送 GET 请求
来源：http://wbt.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cuo.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pes.ybcxt.top

JS:   await fetch(url)
来源：http://vex.pycfn.com

TS:   await fetch(url)
来源：http://rwq.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oso.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://kdr.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jla.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rwr.hnqzz.top

[L02] 发送 POST JSON
来源：http://mtf.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://awo.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jub.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cpw.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bog.zhaomingkeji.xyz


<!-- 参考信息 -->