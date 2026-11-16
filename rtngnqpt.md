代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://okb.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hyf.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://agk.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ujn.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oej.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://cat.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uca.hnxiangtu.top

[H10] 资源自动释放
来源：http://vmz.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iju.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bum.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jvn.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://czw.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vhl.316326.xyz

Go:   defer f.Close()
来源：http://zxo.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qch.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tsm.yuxming.cn

================================================================================
来源：http://ocx.fengsongda.top

I. 正则表达式
来源：http://chw.wangshuangyany.cn

================================================================================
来源：http://vky.chenzaomai.com

[I01] 判断是否匹配
来源：http://hdu.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nxy.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://opr.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://hps.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://rji.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wsy.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hco.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://obe.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mhc.aibaodan.cn

[I02] 提取所有匹配
来源：http://hoe.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://wrr.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fyj.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yzz.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://idk.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ikw.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vwo.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://ttu.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fre.hfpthk.cn

[I03] 提取捕获分组
来源：http://qal.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ziw.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hdu.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cye.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wef.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://abh.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cty.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fcd.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eno.jiagoushi.top

[I04] 正则替换
来源：http://vzu.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tqq.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tgp.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://wsu.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qcd.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sas.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dck.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://prg.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hhv.ivvv.top

[I05] 按正则拆分
来源：http://tlz.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vet.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cnc.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://agw.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://ybj.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://igj.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://law.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://dxu.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://klp.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://twu.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wdt.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qkn.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blq.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vha.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sfe.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fuf.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qtz.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ljf.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://nvo.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pcl.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hhg.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gkl.daxiang520.top

TS:   /error/gim
来源：http://uul.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kbl.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aws.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://sji.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ucc.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://yyy.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cne.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gkk.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xfz.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://svs.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wkf.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://peb.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iok.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://njb.aibaodan.cn

================================================================================
来源：http://epr.xuetiantiany.cn

J. 日期与时间
来源：http://cry.zhoulong.xyz

================================================================================
来源：http://kiq.316326.xyz

[J01] 获取当前时间
来源：http://nec.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yas.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ctg.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://oek.bbcook.cn

TS:   new Date();  Date.now()
来源：http://xhj.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vde.chenlongwang.top

Go:   time.Now()
来源：http://kic.kuanghao11.cn

Ruby: Time.now
来源：http://vlr.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tsf.ppjwa.cn

[J02] 格式化输出
来源：http://bdw.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nav.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qvp.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://chu.guowangkeji.top

TS:   d.toISOString()
来源：http://hkt.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://krh.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://glr.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyc.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aqx.gogol.net.cn

[J03] 字符串解析为日期
来源：http://mww.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xoj.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zdk.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://obc.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://pnc.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://eeo.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hne.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://cgb.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://osb.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://zgx.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baj.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ojw.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ihv.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://exk.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vqa.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xxd.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xxm.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eum.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://wuh.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://zfm.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ucp.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qyo.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cfc.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://rkq.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aus.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://edv.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://baw.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://xzk.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://lxi.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://opu.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://alr.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cpd.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://fdf.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://zhw.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://ber.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://rky.yuanzhike.top

[J07] 比较两个日期
来源：http://ntn.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://slz.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pce.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://xjq.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://jbp.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lsk.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tgj.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gsn.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://wpx.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://nik.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tku.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zrg.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rqh.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rdq.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oyu.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xtk.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://atz.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rzy.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://wci.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://att.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xuw.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lgy.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzq.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rtt.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yuv.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://vzu.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sfr.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://ixv.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xog.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vtb.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gii.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qwc.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://urf.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mxs.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ccg.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ldc.aibaodan.cn

================================================================================
来源：http://adp.zhoulong.xyz

K. JSON 与序列化
来源：http://udo.9152youxi.cn

================================================================================
来源：http://gcq.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://kzm.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://swu.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ham.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://aos.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://hna.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qax.smart0.xyz

Go:   json.Marshal(obj)
来源：http://rur.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://kjh.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lsd.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://yyt.ybcxt.top

Py:   json.loads(s)
来源：http://mkc.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://crd.smart0.xyz

JS:   JSON.parse(s)
来源：http://klo.yongpay.top

TS:   JSON.parse(s)
来源：http://drg.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rwh.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://yoa.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://rnl.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://osg.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://vzj.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lnd.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://del.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nrh.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://oiy.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tbr.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yxi.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mrk.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ptw.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://tej.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dqu.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tqk.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fcs.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rjx.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zek.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fni.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qpp.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ade.hnxiangtu.top

[K05] 深拷贝对象
来源：http://ttx.uphjek.com

Py:   copy.deepcopy(obj)
来源：http://pku.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://tiy.hfpthk.cn

JS:   structuredClone(obj)
来源：http://akt.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://wlq.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://grm.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://icp.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hdv.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://thh.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://wih.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uqt.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xxu.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qmi.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fgj.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cua.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gvd.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fmr.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pvq.nanxuanxn.top

[K07] 进制转换
来源：http://owx.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://smv.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xza.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xpx.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gic.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hnf.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gfl.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uxj.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kju.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://kwc.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://etp.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dhd.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://bxx.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://pkp.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qaz.pengpengdd.cyou

Go:   encoding/gob
来源：http://abj.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://dao.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lua.jiagoushi.top

================================================================================
来源：http://esw.zhoulong.xyz

L. 网络请求
来源：http://nzn.ywan-chungtsiang.top

================================================================================
来源：http://noc.yuanzhike.top

[L01] 发送 GET 请求
来源：http://phg.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jmf.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dar.yanxiufei.cn

JS:   await fetch(url)
来源：http://kvz.smart0.xyz

TS:   await fetch(url)
来源：http://egs.andypj.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sxh.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://bon.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kca.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ukh.vehdjk.com

[L02] 发送 POST JSON
来源：http://icm.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://ief.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fqc.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwv.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dwp.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lti.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ktf.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ehh.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xhd.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://vvj.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cpl.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jnc.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nrt.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sfn.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xrd.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hqn.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://grd.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kkg.sweek.top

[L04] 设置超时
来源：http://fkv.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://oxh.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zce.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://izh.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sgy.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fev.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vum.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://opo.yj20258888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tcf.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://xaa.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nrc.c1oappe.top


<!-- 参考信息 -->