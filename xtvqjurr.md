代发 wailian999

TS:   console.assert(x > 0);
来源：http://gtu.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://plf.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cfn.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jwo.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://qfb.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://ulx.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://bvp.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jes.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://vna.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ttr.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ogu.chenjidiqi.icu

Go:   err.Error()
来源：http://swk.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://zlb.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://hvr.yvedp.cn

[H09] 带错误码的异常
来源：http://gfv.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vwe.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kut.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dya.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jup.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mqf.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fqj.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sld.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ujy.gotoacloud.top

[H10] 资源自动释放
来源：http://bjm.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dsn.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dns.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blf.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iou.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://inh.hammf.cn

Go:   defer f.Close()
来源：http://bav.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hjk.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://maz.hywenlv.cn

================================================================================
来源：http://dby.guowangkeji.top

I. 正则表达式
来源：http://duq.fehbvm.com

================================================================================
来源：http://lfk.smart0.xyz

[I01] 判断是否匹配
来源：http://vfh.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ixu.jiagoushi.top

PHP:  preg_match('/\d+/', $s);
来源：http://rhg.cucudq.cn

JS:   /\d+/.test(s)
来源：http://rtw.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://rzh.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ghc.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tam.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://aci.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nlf.haohaochexian.top

[I02] 提取所有匹配
来源：http://zdz.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://sin.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bji.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jmp.tarul.cn

TS:   s.match(/\d+/g)
来源：http://ndm.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yhz.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tuu.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://cpu.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nvt.hysaishi.cn

[I03] 提取捕获分组
来源：http://pwk.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bie.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lti.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eyq.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://apb.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dkd.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ivq.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kjt.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zth.kuanghao11.cn

[I04] 正则替换
来源：http://jov.svipenyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xtt.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jdr.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://bdy.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sql.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kos.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zan.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wpg.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lmf.ydjk.org.cn

[I05] 按正则拆分
来源：http://qjk.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://asi.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bse.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://qjf.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://rpv.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://vez.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jtq.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://bvp.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://obq.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ser.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oct.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kzy.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ynv.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nib.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tye.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rpy.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dhk.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://trl.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://svl.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cyl.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://syh.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dav.vqdsnc.cn

TS:   /error/gim
来源：http://xzv.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jcq.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://chg.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://clv.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lyv.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://mvy.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://twk.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qse.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aht.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yaj.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rdx.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cof.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jgm.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ajo.zycfv.cn

================================================================================
来源：http://mjf.hcnkem.com

J. 日期与时间
来源：http://xza.ctjpmb.com

================================================================================
来源：http://tbi.xinyue.icu

[J01] 获取当前时间
来源：http://qrl.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uvp.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jfa.yueranfly.top

JS:   new Date();  Date.now()
来源：http://dhz.yj20258888.top

TS:   new Date();  Date.now()
来源：http://efm.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://epy.fanxiaobao.xyz

Go:   time.Now()
来源：http://fbh.gaohongyu789.top

Ruby: Time.now
来源：http://ziw.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hza.gaohongyu789.top

[J02] 格式化输出
来源：http://yag.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://var.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://omp.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xis.hesvh.cn

TS:   d.toISOString()
来源：http://zsc.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rls.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ehe.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lxl.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://haf.gzhubu.top

[J03] 字符串解析为日期
来源：http://jgo.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hxb.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://enb.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://yhk.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://tyw.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vfn.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qwp.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://spo.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uhi.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://qot.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://elp.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rcx.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://prp.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://jav.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fyg.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dgn.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lgx.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jzj.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://qel.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://ndl.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://wld.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ocn.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vjp.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://bks.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://thb.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://gfc.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jap.jlsjyb.cn

[J06] 计算两时间之差
来源：http://wuz.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://svc.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://ahm.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cyi.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ezz.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://nzh.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://xie.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://zoe.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://uxw.haohaochexian.top

[J07] 比较两个日期
来源：http://usx.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://gvd.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jez.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://gte.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://zhs.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://usq.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cbh.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qtv.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://gli.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://ill.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://exv.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://auy.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rjf.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bah.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lel.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hlc.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rfy.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ytp.yueranfly.top

[J09] 时区处理
来源：http://eeh.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pol.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iub.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cwi.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gph.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eps.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nkd.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ckn.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://shh.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://ekb.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qqz.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ykv.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iqe.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lae.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lcz.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xpj.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vqv.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vkn.zhijiandao.cn

================================================================================
来源：http://cjk.ehwqpu.com

K. JSON 与序列化
来源：http://tlb.zycfv.cn

================================================================================
来源：http://cuy.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://pot.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://trz.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wsw.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://gje.meibo888.top

TS:   JSON.stringify(obj)
来源：http://mfq.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yqq.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://ymk.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://kkg.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://hpu.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://sva.ctjpmb.com

Py:   json.loads(s)
来源：http://dub.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qan.snrcjt.cn

JS:   JSON.parse(s)
来源：http://uqd.nanxinkj.top

TS:   JSON.parse(s)
来源：http://kup.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xsa.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://hgi.nwbrower.top

Ruby: JSON.parse(s)
来源：http://pbv.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://old.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://qze.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wmz.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ert.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dep.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xvn.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://czv.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://clb.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://ssg.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nkw.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://qdz.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tmc.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yql.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cma.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://onn.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ivb.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qxd.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xev.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tjw.xziqi.cn

[K05] 深拷贝对象
来源：http://zkf.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://tfe.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://wyk.yfazqb.com

JS:   structuredClone(obj)
来源：http://zux.zhixingplan.top

TS:   structuredClone(obj)
来源：http://ckv.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wxt.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gmw.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tcf.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://esk.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://jtb.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bmg.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://izp.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pic.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrb.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zxx.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ofr.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://flm.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sjh.guannengcc.top

[K07] 进制转换
来源：http://mal.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://isw.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wis.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dkr.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qza.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jis.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://udp.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tvs.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tkw.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://wnt.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://nuq.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kij.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://gcw.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://zyv.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kcq.svipenyu.cn

Go:   encoding/gob
来源：http://exu.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://bem.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ssl.nanxuanxn.top

================================================================================
来源：http://ryx.gaohongyu789.top

L. 网络请求
来源：http://hwg.yj20258888.top

================================================================================
来源：http://nbx.aizwys.cn

[L01] 发送 GET 请求
来源：http://pfs.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pcr.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uzs.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://qil.bbcook.cn

TS:   await fetch(url)
来源：http://uxg.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://epr.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://cgd.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ier.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vyy.gzhubu.top

[L02] 发送 POST JSON
来源：http://huq.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nkq.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ppz.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgp.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hgw.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pfs.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lgt.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xmo.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vco.ydzc1.top

[L03] 设置自定义请求头
来源：http://tyg.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fpt.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mvp.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lux.ybcxt.top


<!-- 参考信息 -->