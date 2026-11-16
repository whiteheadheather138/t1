代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://pgk.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ckz.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ufk.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vxk.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xfv.bbcook.cn

Go:   defer f.Close()
来源：http://xhn.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sez.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdk.iojbl.cn

================================================================================
来源：http://pro.zhijiandao.cn

I. 正则表达式
来源：http://otk.tanke756.top

================================================================================
来源：http://hkd.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://fkz.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hfr.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://krl.yfazqb.com

JS:   /\d+/.test(s)
来源：http://vbw.xuanzx.com

TS:   /\d+/.test(s)
来源：http://pcb.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zxz.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://waf.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://jeo.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cfh.pycfn.com

[I02] 提取所有匹配
来源：http://kbu.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://fdy.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zlu.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://umh.yj202588.top

TS:   s.match(/\d+/g)
来源：http://odz.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://trb.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hpq.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://qxg.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mpk.yj202588.top

[I03] 提取捕获分组
来源：http://fdz.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://efo.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qcy.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://opt.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yyg.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bfv.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gvi.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qmh.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uyz.xuetiantiany.cn

[I04] 正则替换
来源：http://ova.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://etr.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ggx.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://bgy.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://beu.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://jyz.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://gzv.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xzg.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rtj.fzhhl.top

[I05] 按正则拆分
来源：http://toe.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xfm.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sfv.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://aop.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://iem.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://vcl.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qla.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://jfk.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mrf.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lky.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://upz.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dgs.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iqh.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cza.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tlf.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wrp.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hne.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pja.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://vug.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pbw.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cvd.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ubk.yongpay.top

TS:   /error/gim
来源：http://owi.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gcw.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://and.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://hqp.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rpm.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://qai.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jbt.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gva.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ymk.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vex.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ppf.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dji.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xbc.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lkv.yueranfly.top

================================================================================
来源：http://jeq.jinqigfzy.top

J. 日期与时间
来源：http://hqh.guannengcc.top

================================================================================
来源：http://vty.jiagoushi.top

[J01] 获取当前时间
来源：http://pzc.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ozt.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uyt.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://nml.hnqzz.top

TS:   new Date();  Date.now()
来源：http://qeb.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://mnf.tianlin.xyz

Go:   time.Now()
来源：http://eqo.guannengcc.top

Ruby: Time.now
来源：http://cdc.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lwh.yueranfly.top

[J02] 格式化输出
来源：http://fbc.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dlu.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hal.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pta.jqgufenzy.top

TS:   d.toISOString()
来源：http://vzo.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uud.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zty.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zwl.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vup.bbcook.cn

[J03] 字符串解析为日期
来源：http://hie.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cuq.xinyue.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qfy.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://nvv.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://opp.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://upj.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wya.jinyuanbaomall.cn

Ruby: Date.parse("2024-01-02")
来源：http://ljm.ivvv.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xuo.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://ciw.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bmq.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oej.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xcc.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yhr.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://amg.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rxa.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rcx.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vqk.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://dlt.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://dbb.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wvd.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ooc.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ole.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://uvp.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://geh.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://tio.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://zsz.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://jzf.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://kau.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://gan.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mel.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://abp.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://oav.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://rua.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://dlf.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://ama.jqgufenzy.top

[J07] 比较两个日期
来源：http://unj.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://oma.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gqk.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://axu.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tuv.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://glt.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iao.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://kjd.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://sjr.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://yoa.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hry.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xjz.jianghu66.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://coe.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wdl.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rij.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qmd.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oxs.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jhx.ydjk.org.cn

[J09] 时区处理
来源：http://sqz.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://clx.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tth.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jch.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lye.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aql.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mqi.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xqq.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eqq.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://nsn.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://svg.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fpk.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xpl.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ftj.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xnu.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hxo.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nyl.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jiz.sufxvd.cn

================================================================================
来源：http://hmt.hysaishi.cn

K. JSON 与序列化
来源：http://msu.nwbrower.top

================================================================================
来源：http://wwl.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://ygb.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://shl.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jld.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://dzz.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://uoc.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kpx.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://npq.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qti.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yfa.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://qks.quarkkingdee.top

Py:   json.loads(s)
来源：http://ryl.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ojg.jiagoushi.top

JS:   JSON.parse(s)
来源：http://mxv.guowangkeji.top

TS:   JSON.parse(s)
来源：http://vcf.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fnw.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://qcq.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://cmu.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xrm.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://evs.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iij.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cjw.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://okv.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wky.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qht.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://onb.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://qpd.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eft.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://hag.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qig.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wix.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ylg.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eaa.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ydr.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gnp.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rit.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yrj.ctjpmb.com

[K05] 深拷贝对象
来源：http://amw.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://wkt.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://jfp.dianchejie.cn

JS:   structuredClone(obj)
来源：http://uvc.9152youxi.cn

TS:   structuredClone(obj)
来源：http://vxb.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bzz.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cem.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xpi.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sak.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://pro.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hdp.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eex.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kpf.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nlv.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aps.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kbx.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lih.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gtj.sweek.top

[K07] 进制转换
来源：http://mxl.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hhc.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cnx.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eoo.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rvr.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://evk.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wrd.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tts.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://apg.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://gno.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://zsd.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://nqw.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://fxu.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://aer.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kqk.jyoumei.cn

Go:   encoding/gob
来源：http://ltg.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://rkq.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ucm.epnwcf.com

================================================================================
来源：http://yyo.fzhhl.top

L. 网络请求
来源：http://hoq.hcnkem.com

================================================================================
来源：http://twv.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://cik.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://taq.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mub.ppjwa.cn

JS:   await fetch(url)
来源：http://yuv.sufxvd.cn

TS:   await fetch(url)
来源：http://asn.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gzv.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://chy.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lvw.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cxp.316326.xyz

[L02] 发送 POST JSON
来源：http://wcq.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://fob.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://syg.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hik.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rwx.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nun.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fqr.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ycl.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xru.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://pzj.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bog.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bqh.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mqb.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://acj.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ewj.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eyt.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://htp.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jwz.cheryme.top

[L04] 设置超时
来源：http://vct.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://btm.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qut.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qlq.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vwp.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ved.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qcw.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cmp.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://thw.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://dns.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rnd.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pdo.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qkl.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vap.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gnm.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tgx.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jrf.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iam.hesvh.cn

[L06] 解析响应为 JSON
来源：http://vel.52xcode.cn


<!-- 参考信息 -->