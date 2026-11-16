代发 wailian999

JS:   e.message;  e.stack
来源：http://fxp.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://akg.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vah.jqgfzy.top

Go:   err.Error()
来源：http://vkf.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://xdi.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://yoa.wangdashe.top

[H09] 带错误码的异常
来源：http://tks.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fft.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zrl.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vyo.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bmd.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mru.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nvm.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://psp.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://sej.yanxiufei.cn

[H10] 资源自动释放
来源：http://nyu.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yzy.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mhq.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://abd.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://quc.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://scv.xylfe.cn

Go:   defer f.Close()
来源：http://dgv.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ygl.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://met.gaohongyu789.top

================================================================================
来源：http://zeu.xuetiantiany.cn

I. 正则表达式
来源：http://lgb.fanxiaobao.xyz

================================================================================
来源：http://exa.c1oappe.top

[I01] 判断是否匹配
来源：http://vgo.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://snu.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zhd.meibo888.top

JS:   /\d+/.test(s)
来源：http://vrf.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://kor.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cyt.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://euk.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://qpi.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gnr.meibo888.top

[I02] 提取所有匹配
来源：http://kou.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://wzp.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mvf.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wjh.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://cwj.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wzq.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vib.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://jdt.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://idp.tarul.cn

[I03] 提取捕获分组
来源：http://qgf.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://txg.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xuv.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ysn.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bgc.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kuu.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wcg.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ixf.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zze.jqgufenzy.top

[I04] 正则替换
来源：http://mcf.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://vrf.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lcu.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://jqm.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://yah.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hth.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://nqx.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mvh.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jgj.ppjwa.cn

[I05] 按正则拆分
来源：http://bin.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://vva.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dre.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://uip.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://ysv.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://nfe.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cqo.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://xxb.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cpq.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://egb.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sra.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fgc.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhs.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hmf.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://twz.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://isq.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://owm.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rui.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://tah.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dav.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aue.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://adn.ivvv.top

TS:   /error/gim
来源：http://ede.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nkm.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nbl.yongpay.top

Ruby: s.scan(/error/i)
来源：http://odi.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tkb.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://kym.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qyb.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gzp.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qka.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gvs.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mfj.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oxh.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rgz.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dku.hesvh.cn

================================================================================
来源：http://dbf.hcnkem.com

J. 日期与时间
来源：http://goa.yvedp.cn

================================================================================
来源：http://bni.jiagoushi.top

[J01] 获取当前时间
来源：http://pwg.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wfb.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xar.hnqzz.top

JS:   new Date();  Date.now()
来源：http://jig.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://zob.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://puq.zdbjq.cn

Go:   time.Now()
来源：http://yxr.gotoacloud.top

Ruby: Time.now
来源：http://qyb.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xse.chenjidiqi.icu

[J02] 格式化输出
来源：http://ehl.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://igd.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://emo.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uvb.gogol.net.cn

TS:   d.toISOString()
来源：http://wka.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://unh.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fgr.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bpv.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nyq.zdbjq.cn

[J03] 字符串解析为日期
来源：http://yzl.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ofi.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rzd.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://qpk.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://tcy.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://gpm.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bvf.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://zxl.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yvj.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://msc.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tbb.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ial.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vjw.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cra.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hnr.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbt.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kss.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yhm.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://ymu.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://flz.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pck.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fya.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmh.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://nwi.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qbg.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://kki.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://lqh.ybcxt.top

[J06] 计算两时间之差
来源：http://qeb.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://xsv.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://hqq.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bms.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aeg.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://hwr.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://udu.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://nkg.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://jwe.yfazqb.com

[J07] 比较两个日期
来源：http://ksv.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://sgz.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ahw.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kza.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://jqw.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kbn.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zvh.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://fgp.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://fws.yfazqb.com

[J08] 提取年月日与星期
来源：http://aje.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vmz.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yng.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zab.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gtu.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rfg.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://apj.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hpp.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yjn.mhx1999.top

[J09] 时区处理
来源：http://cwa.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wfs.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qal.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hum.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fem.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jkv.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zet.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://jci.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nma.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://egt.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vob.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cog.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bxu.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dhy.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://osg.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nth.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qvr.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zvf.fengsongda.top

================================================================================
来源：http://udf.jianghu66.top

K. JSON 与序列化
来源：http://geh.fengsongda.top

================================================================================
来源：http://zzd.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://wox.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://caw.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wir.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://mhn.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://igp.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jyp.tian-w.cn

Go:   json.Marshal(obj)
来源：http://ejo.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xsh.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lct.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://tqr.nwbrower.top

Py:   json.loads(s)
来源：http://wcs.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lyk.jqgfzy.top

JS:   JSON.parse(s)
来源：http://yvn.sysykeji.top

TS:   JSON.parse(s)
来源：http://yfq.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yrw.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://bjo.sxryk.cn

Ruby: JSON.parse(s)
来源：http://qkv.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ghj.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://djg.yuanzhike.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ehw.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tox.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zgu.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ckp.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cqe.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pat.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://oqj.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sbx.yvedp.cn

[K04] 读取 JSON 文件
来源：http://aqc.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gdv.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ohv.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zns.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfv.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://okm.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zgn.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzj.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fgn.haohaochexian.top

[K05] 深拷贝对象
来源：http://yiy.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://gzs.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://hgl.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://pyd.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://uls.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pir.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lvm.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://trn.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ajw.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://zkr.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yoh.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ezh.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://abl.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nxo.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://spa.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vjs.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zyx.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zbd.fanxiaobao.xyz

[K07] 进制转换
来源：http://xhc.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hhd.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qsl.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vzm.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ylb.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bqg.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ams.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mfn.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gkk.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://hqw.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://hdf.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nts.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://svn.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://agw.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xxk.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://cpn.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://rxx.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kqv.yueranfly.top

================================================================================
来源：http://rok.yj202588.top

L. 网络请求
来源：http://oak.ppjwa.cn

================================================================================
来源：http://dwt.zdqjudy.top

[L01] 发送 GET 请求
来源：http://fbn.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yol.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ehv.jinqigfzy.top

JS:   await fetch(url)
来源：http://kuq.xuetiantiany.cn

TS:   await fetch(url)
来源：http://wjj.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://juh.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://mgr.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://doe.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bmv.aibaodan.cn

[L02] 发送 POST JSON
来源：http://rxt.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vcb.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://shr.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cbh.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufb.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctq.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bus.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vyt.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://neg.daxiang520.top

[L03] 设置自定义请求头
来源：http://cku.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://szy.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://owc.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfo.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tse.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aei.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vzc.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jaj.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ydq.cdnleiting.top

[L04] 设置超时
来源：http://jpr.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://oyb.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://spt.bjfxy.top


<!-- 参考信息 -->