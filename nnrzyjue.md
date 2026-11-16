代发 wailian999

[H07] 断言
来源：http://wfy.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://dhg.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://hhm.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://imk.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://xoz.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://hol.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vae.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://mib.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://rhz.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://lnz.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://dgg.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ued.yuxming.cn

JS:   e.message;  e.stack
来源：http://dkq.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://atu.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://lpd.chenjidiqi.icu

Go:   err.Error()
来源：http://adm.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://shv.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://upj.shzxlz.cn

[H09] 带错误码的异常
来源：http://ihy.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nui.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mvt.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rwk.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://str.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jsk.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bho.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uyv.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ukw.gotoacloud.top

[H10] 资源自动释放
来源：http://yub.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uhq.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://drx.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xyu.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vrd.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oaz.hesvh.cn

Go:   defer f.Close()
来源：http://kig.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nzr.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rvx.epnwcf.com

================================================================================
来源：http://lgp.gzhubu.top

I. 正则表达式
来源：http://jhh.yongpay.top

================================================================================
来源：http://obk.fktsv.cn

[I01] 判断是否匹配
来源：http://swv.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vtg.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://pcr.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://dll.316326.xyz

TS:   /\d+/.test(s)
来源：http://ttk.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iak.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://trq.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://qbp.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ciy.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://rnf.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://nkb.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oef.shzxlz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dic.yj202588.top

TS:   s.match(/\d+/g)
来源：http://glv.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ogg.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ejs.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://rds.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://onf.hcnkem.com

[I03] 提取捕获分组
来源：http://lbr.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qrk.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fgu.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://efu.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fsv.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cir.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iab.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rvi.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ohp.hysaishi.cn

[I04] 正则替换
来源：http://qrs.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://amt.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lhx.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://tkr.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://pwl.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://nxx.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://nrl.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://scx.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yys.meibo888.top

[I05] 按正则拆分
来源：http://mrr.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://scp.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://box.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://ccq.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://ept.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://ihe.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bir.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://npq.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zbd.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xcc.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://esk.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mik.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gue.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yvv.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ihf.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fih.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://byw.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yps.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://nef.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kth.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ilc.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sdm.dianchejie.cn

TS:   /error/gim
来源：http://glb.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kaz.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pnf.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://kea.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vke.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://cyl.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vvp.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bxv.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bxi.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dbi.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wif.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yca.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://muv.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uqf.xinyue.icu

================================================================================
来源：http://afi.quarkkingdee.top

J. 日期与时间
来源：http://pjd.pengpengdd.cyou

================================================================================
来源：http://mxe.yj20258.top

[J01] 获取当前时间
来源：http://eee.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://nev.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ytt.hammf.cn

JS:   new Date();  Date.now()
来源：http://hfu.mhx1999.top

TS:   new Date();  Date.now()
来源：http://lvy.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ajt.tian-w.cn

Go:   time.Now()
来源：http://roq.nanxuanxn.top

Ruby: Time.now
来源：http://wum.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tds.tian-w.cn

[J02] 格式化输出
来源：http://cho.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nqz.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nbq.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://akk.cashguo.top

TS:   d.toISOString()
来源：http://byc.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ujo.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gtu.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sgt.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fae.hnqzz.top

[J03] 字符串解析为日期
来源：http://anl.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vfj.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://umt.yonumen.top

JS:   new Date("2024-01-02")
来源：http://tuw.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://mrs.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://awa.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://evf.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://syt.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bow.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://axd.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jzz.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fkq.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qbo.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://usn.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wrh.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rih.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nfx.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xxy.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://tpq.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://fuu.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nzx.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://esa.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fag.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://zab.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://thn.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://qhr.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wjw.hfpthk.cn

[J06] 计算两时间之差
来源：http://vhe.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://slf.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://ilu.cucudq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lqn.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aep.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://glz.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://rnb.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://rte.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://ktn.yj20258.top

[J07] 比较两个日期
来源：http://elu.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://kve.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wsl.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ugi.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://rwc.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lii.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gkt.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://wdx.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://bne.epnwcf.com

[J08] 提取年月日与星期
来源：http://ych.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aux.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://btc.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://frm.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bjo.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zsb.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pdx.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zpz.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bfb.guannengcc.top

[J09] 时区处理
来源：http://ryn.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kki.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xyb.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxq.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://flr.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tnq.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qas.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ipk.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qwk.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://vtv.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://trd.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://csp.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uun.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://doi.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ajo.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tlc.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xbq.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wwx.sysykeji.top

================================================================================
来源：http://sog.cqqwz.cn

K. JSON 与序列化
来源：http://fqx.yanxiufei.cn

================================================================================
来源：http://hol.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://lxp.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vfs.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eiu.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://evz.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://pbt.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qhp.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://gkr.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://jni.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ucp.daxiang520.top

[K02] JSON 字符串转对象
来源：http://kwh.uphjek.com

Py:   json.loads(s)
来源：http://wip.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cdx.chenlongwang.top

JS:   JSON.parse(s)
来源：http://yro.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://yve.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nio.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://xtm.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://igg.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tgz.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://bou.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hvz.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rwx.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fcp.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://xlm.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ywl.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wbx.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://dov.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vwb.52xcode.cn

[K04] 读取 JSON 文件
来源：http://qqw.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wor.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mze.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tfa.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwa.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jnb.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://efk.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ilh.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://chl.hnxiangtu.top

[K05] 深拷贝对象
来源：http://vaq.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://ozy.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://lgq.cheryme.top

JS:   structuredClone(obj)
来源：http://wpk.mhx1999.top

TS:   structuredClone(obj)
来源：http://ild.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://imd.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wqp.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nji.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zbk.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://vls.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svp.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://emm.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwb.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qnw.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fwn.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://irg.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lzo.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fef.jianghu66.top

[K07] 进制转换
来源：http://viu.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cbx.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lak.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cav.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jvy.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://usm.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://onj.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://awl.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eab.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://ttb.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://iea.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jqr.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://uat.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://vvn.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wjl.vehdjk.com

Go:   encoding/gob
来源：http://xrs.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://onr.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rba.hcnkem.com

================================================================================
来源：http://xbk.dianchejie.cn

L. 网络请求
来源：http://zxe.xuanzx.com

================================================================================
来源：http://chl.tarul.cn

[L01] 发送 GET 请求
来源：http://yjd.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qlw.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qfb.jianghu66.top

JS:   await fetch(url)
来源：http://jjm.chenjidiqi.icu

TS:   await fetch(url)
来源：http://pbz.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fau.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://gmm.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xro.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dgy.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://ovg.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://nwb.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://act.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rha.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wut.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cbq.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://swi.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://euh.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://goy.cqqwz.cn


<!-- 参考信息 -->