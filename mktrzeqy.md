代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://cxi.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sll.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dwj.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kop.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fga.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://yaw.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://fpm.yj20258888.top

[H10] 资源自动释放
来源：http://hwl.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dbu.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cbc.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qjk.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://beg.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://doz.fktsv.cn

Go:   defer f.Close()
来源：http://opm.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://grq.cashguo.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dzw.ybcxt.top

================================================================================
来源：http://equ.smart0.xyz

I. 正则表达式
来源：http://ekb.sufxvd.cn

================================================================================
来源：http://lvl.smart0.xyz

[I01] 判断是否匹配
来源：http://mrf.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ifr.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://phg.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://eju.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://vcx.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sbv.hnqzz.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uzm.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://olu.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://otd.gaohongyu789.top

[I02] 提取所有匹配
来源：http://fmy.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://eae.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gbi.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rlk.nwbrower.top

TS:   s.match(/\d+/g)
来源：http://dkk.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://brr.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jwo.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://fli.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hxl.andypj.xyz

[I03] 提取捕获分组
来源：http://axj.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xpx.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mcc.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hun.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xnq.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xfj.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ttk.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tqv.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bly.haohaochexian.top

[I04] 正则替换
来源：http://xyr.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cyg.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kgn.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://bbj.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://ybx.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://rzd.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://jsr.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hlw.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zoc.ppjwa.cn

[I05] 按正则拆分
来源：http://lww.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vfp.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zzj.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tlk.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://fur.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://tzw.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yjj.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pbr.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://csh.meibo888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qrh.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zfp.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://udm.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mvc.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://agm.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kgy.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://evk.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cgi.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jts.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://gjm.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oif.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ysb.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sfx.gotoacloud.top

TS:   /error/gim
来源：http://owt.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lpj.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://czy.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://spu.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qhg.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://kzd.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sdy.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ptt.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lbq.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://feq.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://azu.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vvo.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://doh.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://axd.zhiwuduotai.top

================================================================================
来源：http://lzn.sjlbkw.cn

J. 日期与时间
来源：http://oho.daxiang520.top

================================================================================
来源：http://ken.yangfankeji.com

[J01] 获取当前时间
来源：http://afl.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://mhc.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://srp.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://mxm.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://qlc.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://wnd.hesvh.cn

Go:   time.Now()
来源：http://qvy.chenlongwang.top

Ruby: Time.now
来源：http://dqk.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tej.daria6918.cn

[J02] 格式化输出
来源：http://ydt.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hjv.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kil.pycfn.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ajy.cqqwz.cn

TS:   d.toISOString()
来源：http://mik.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hkz.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://okh.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjv.sufxvd.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vee.sysykeji.top

[J03] 字符串解析为日期
来源：http://hfx.ydzc1.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lrj.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yap.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://luv.hammf.cn

TS:   new Date("2024-01-02")
来源：http://trh.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://upy.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ucx.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://ffw.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dwr.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://ieg.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yyf.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kuk.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dem.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hoo.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sqi.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gaf.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yrq.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vkq.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://xql.yonumen.top

Py:   now + timedelta(days=7)
来源：http://ypr.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dio.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zru.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqa.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://loz.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kyh.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://hfo.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iio.redwolf501.top

[J06] 计算两时间之差
来源：http://ovl.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://hee.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://szu.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nim.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yhm.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://gxf.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://hsl.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://jwn.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://ybq.nanxinkj.top

[J07] 比较两个日期
来源：http://buk.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://oqx.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rev.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://nll.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://yae.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aph.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://swt.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://ybp.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://bge.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://ezi.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hpn.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xoi.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://igp.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://edg.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kud.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xeg.dashuyun.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mwu.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yim.feifeiyinyue.top

[J09] 时区处理
来源：http://ync.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wco.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pwu.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kkr.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ews.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ldj.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lqu.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mhe.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pqb.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://rpn.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mpw.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ylt.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mxo.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yjz.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wbm.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fev.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://atv.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xwy.fktsv.cn

================================================================================
来源：http://kva.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://rbw.daria6918.cn

================================================================================
来源：http://epr.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://btm.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://una.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ffa.316326.xyz

JS:   JSON.stringify(obj)
来源：http://sfo.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://kfc.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cuk.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://dyj.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://vjy.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://joj.epnwcf.com

[K02] JSON 字符串转对象
来源：http://zjz.cheryme.top

Py:   json.loads(s)
来源：http://urf.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qlg.uphjek.com

JS:   JSON.parse(s)
来源：http://tzf.zhengqikj.top

TS:   JSON.parse(s)
来源：http://iyb.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://caz.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://jvj.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://emx.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ije.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://rkh.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rmu.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rsa.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://flo.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mdr.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fdk.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ntz.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://zgt.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://umy.sysykeji.top

[K04] 读取 JSON 文件
来源：http://hvn.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rwe.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://znr.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qad.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujd.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zfs.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xfn.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uxc.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ayf.kuanghao11.cn

[K05] 深拷贝对象
来源：http://xku.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://xtv.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://ryj.yonumen.top

JS:   structuredClone(obj)
来源：http://hqn.hywenlv.cn

TS:   structuredClone(obj)
来源：http://oqe.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ylf.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tqz.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ojb.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wen.yfazqb.com

[K06] 解析 URL 查询串
来源：http://mja.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ims.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uzw.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmq.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://suu.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hje.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oek.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nav.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rpr.hywenlv.cn

[K07] 进制转换
来源：http://fsj.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://soa.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yvw.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wjt.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fig.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xel.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bxt.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://awr.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wao.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://lwx.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://isd.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://svv.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://cve.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://oyp.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://boc.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://gnv.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://sxx.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rnf.sysykeji.top

================================================================================
来源：http://atf.cqqwz.cn

L. 网络请求
来源：http://pde.fengsongda.top

================================================================================
来源：http://xgd.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://fhe.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nux.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://soo.sysykeji.top

JS:   await fetch(url)
来源：http://fmx.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://wvu.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ray.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://qas.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kup.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mnc.guowangkeji.top

[L02] 发送 POST JSON
来源：http://oct.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qxs.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kng.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ein.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://glj.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xsh.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zsn.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ylh.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zlg.52xcode.cn

[L03] 设置自定义请求头
来源：http://qxk.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vxk.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iwk.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ubo.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://egk.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://urq.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dff.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://giu.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qkg.shuidangran.top

[L04] 设置超时
来源：http://jqz.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://qak.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cny.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nmx.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://efn.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://irb.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vzn.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kqv.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lps.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://srb.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ixp.xinyue.icu


<!-- 参考信息 -->