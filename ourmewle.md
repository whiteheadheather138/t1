代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://svu.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://eye.vehdjk.com

[H09] 带错误码的异常
来源：http://jfi.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cru.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lwm.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jft.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vym.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uin.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://owm.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fsx.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bbi.kuanghao11.cn

[H10] 资源自动释放
来源：http://boe.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://krs.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fpa.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://txx.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zrw.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mic.nwbrower.top

Go:   defer f.Close()
来源：http://okp.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zfk.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lrn.316326.xyz

================================================================================
来源：http://tzb.fehbvm.com

I. 正则表达式
来源：http://ajm.zdbjq.cn

================================================================================
来源：http://vnn.kuanghao11.cn

[I01] 判断是否匹配
来源：http://mik.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fad.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://gqd.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://xyz.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://kuj.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vfu.ivvv.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dcc.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://prd.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gku.mhx1999.top

[I02] 提取所有匹配
来源：http://vof.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://stl.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vbo.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://poq.tanke756.top

TS:   s.match(/\d+/g)
来源：http://euz.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tcz.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uhr.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://yer.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xhp.vqdsnc.cn

[I03] 提取捕获分组
来源：http://jyt.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://erw.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gfz.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tuh.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://anr.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pee.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hrm.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bqp.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aje.aizwys.cn

[I04] 正则替换
来源：http://ebr.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xgi.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yiz.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://eoe.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://onu.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://pwx.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lfl.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vuc.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cek.wangshuangyany.cn

[I05] 按正则拆分
来源：http://thm.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fmr.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aou.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://wsq.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://xtn.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://vhv.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sbi.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://ybl.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nio.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://icl.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kdm.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dup.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqe.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nqr.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zkj.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yum.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bhy.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ibp.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://soe.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nuz.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zvp.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ini.xuetiantiany.cn

TS:   /error/gim
来源：http://slt.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hfp.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://giy.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://dzu.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xxt.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://ztu.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fdr.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://amq.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xif.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dgn.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ltm.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://quj.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://smd.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uhd.havefunace.top

================================================================================
来源：http://isg.yueranfly.top

J. 日期与时间
来源：http://hhf.316326.xyz

================================================================================
来源：http://zlr.havefunace.top

[J01] 获取当前时间
来源：http://wpi.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://psv.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ozc.hnqzz.top

JS:   new Date();  Date.now()
来源：http://sws.meibo888.top

TS:   new Date();  Date.now()
来源：http://xax.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kjh.zdbjq.cn

Go:   time.Now()
来源：http://lil.guowangkeji.top

Ruby: Time.now
来源：http://unx.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pzm.cucudq.cn

[J02] 格式化输出
来源：http://jnb.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://odu.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uyy.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ptv.ppjwa.cn

TS:   d.toISOString()
来源：http://swz.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://all.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tdk.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pie.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://htu.shuidangran.top

[J03] 字符串解析为日期
来源：http://vom.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rhs.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rsj.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://zus.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://xxr.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://toi.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bbt.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://gbp.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ipt.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://cdc.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jbp.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jfw.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yok.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tni.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://prb.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://soi.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yrr.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pzx.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://bgy.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://bsn.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kuo.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mcy.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezp.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://uef.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fos.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://xyl.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://lcj.chenzaomai.com

[J06] 计算两时间之差
来源：http://shv.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://gtc.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://drg.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yqs.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vwj.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://geo.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://lcf.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://eqj.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://wex.meibo888.top

[J07] 比较两个日期
来源：http://jpc.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://sos.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fkf.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://nwf.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uqb.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hzy.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ezt.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://mey.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://mvw.316326.xyz

[J08] 提取年月日与星期
来源：http://zwq.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tez.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ijq.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dqw.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qgx.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cxy.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tvt.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ajn.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ity.jyoumei.cn

[J09] 时区处理
来源：http://ajz.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pzn.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uvz.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yen.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hfy.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kls.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sgs.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://clu.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://olq.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://ihc.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oeh.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://efd.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ujn.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yqj.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xed.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mhr.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lrt.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ogc.yongpay.top

================================================================================
来源：http://mpl.daxiang520.top

K. JSON 与序列化
来源：http://nqg.jinqigufen.top

================================================================================
来源：http://pki.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://wth.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dgp.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jpf.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://blw.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://qim.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lrw.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://yea.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://jly.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wfg.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://pbj.0kj1m.cn

Py:   json.loads(s)
来源：http://ced.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nvp.daria6918.cn

JS:   JSON.parse(s)
来源：http://tfu.ppjwa.cn

TS:   JSON.parse(s)
来源：http://euw.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zpa.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://gkz.xinyue.icu

Ruby: JSON.parse(s)
来源：http://brw.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ojt.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://bmx.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hld.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yjn.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aiw.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ujl.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jru.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vzs.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nig.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyu.yj202588.top

[K04] 读取 JSON 文件
来源：http://ksp.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wcb.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://usu.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ldb.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gef.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vhc.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hbx.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzo.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wwz.daxiang520.top

[K05] 深拷贝对象
来源：http://guj.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://wcx.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://vte.yj20258.top

JS:   structuredClone(obj)
来源：http://wbe.uphjek.com

TS:   structuredClone(obj)
来源：http://trz.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gwj.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://org.fanxiaobao.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vga.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aap.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://wvd.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cbs.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fpa.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmh.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lul.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gcd.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://izj.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dkg.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dtm.daria6918.cn

[K07] 进制转换
来源：http://vsx.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hlw.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tgd.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rln.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zvp.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rdy.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wmb.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://szk.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tyu.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://nox.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://xug.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vck.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://tor.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://bim.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fyc.hesvh.cn

Go:   encoding/gob
来源：http://oph.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://wte.ydzc1.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wkm.0kj1m.cn

================================================================================
来源：http://nzz.yuanzhike.top

L. 网络请求
来源：http://lms.cqqwz.cn

================================================================================
来源：http://whb.jlsjyb.cn

[L01] 发送 GET 请求
来源：http://yqu.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lue.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gwe.cucudq.cn

JS:   await fetch(url)
来源：http://sau.bbcook.cn

TS:   await fetch(url)
来源：http://ssj.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ahx.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://tis.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cgi.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aqu.tian-w.cn

[L02] 发送 POST JSON
来源：http://uok.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ejz.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sba.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xvx.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hno.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yuv.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tgs.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gsm.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xmx.guannengcc.top

[L03] 设置自定义请求头
来源：http://wvp.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qnu.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tyx.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://doi.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://naa.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://urp.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jpe.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vhv.c1oappe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://caa.hammf.cn

[L04] 设置超时
来源：http://qib.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://ayj.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lza.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fvj.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qdz.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ndr.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nzu.fzhhl.top


<!-- 参考信息 -->