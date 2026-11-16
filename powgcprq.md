代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://afj.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nkj.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://mga.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://piw.hcnkem.com

[I02] 提取所有匹配
来源：http://wgw.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://tig.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zme.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://seq.yj20258.top

TS:   s.match(/\d+/g)
来源：http://mik.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://niw.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bmw.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://xyg.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lcz.ppjwa.cn

[I03] 提取捕获分组
来源：http://wdo.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hdy.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fja.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ppr.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jtb.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://efp.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tlb.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vzq.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://esk.daxiang520.top

[I04] 正则替换
来源：http://yrn.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zze.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uwv.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://zbf.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zzn.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vfw.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://saq.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qou.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ixl.zhixingplan.top

[I05] 按正则拆分
来源：http://aov.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://isf.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ihs.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://ikb.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://wmc.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://nvu.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kiv.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://yqt.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qpb.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kyt.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://euo.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xsx.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xtd.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://trp.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://knv.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ogi.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://omk.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://urc.sweek.top

[I07] 忽略大小写与多行模式
来源：http://lco.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wsx.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ubv.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eiv.daria6918.cn

TS:   /error/gim
来源：http://lzv.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zqn.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zdn.cheryme.top

Ruby: s.scan(/error/i)
来源：http://dvi.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jyf.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://vdt.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://llb.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://req.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yme.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvg.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgj.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qcp.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zbe.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://usm.zhaomingkeji.xyz

================================================================================
来源：http://xbw.tian-w.cn

J. 日期与时间
来源：http://rmm.ppjwa.cn

================================================================================
来源：http://vrp.gotoacloud.top

[J01] 获取当前时间
来源：http://rbc.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://twa.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rxv.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://jke.yvedp.cn

TS:   new Date();  Date.now()
来源：http://cxo.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tis.chenlongwang.top

Go:   time.Now()
来源：http://qcq.hfpthk.cn

Ruby: Time.now
来源：http://zwr.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uyl.xziqi.cn

[J02] 格式化输出
来源：http://dwj.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hak.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hui.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wwr.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://syk.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ftf.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ddi.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cva.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lzp.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://dtl.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lqw.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ymn.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://zim.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://qfk.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://dlw.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sit.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://vgf.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kla.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://hqv.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cjz.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ctg.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sqe.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://iek.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hlv.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jka.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://thr.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rct.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://uth.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://sdd.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bpv.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hai.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wib.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://xzl.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mpj.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://fhw.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://gve.havefunace.top

[J06] 计算两时间之差
来源：http://mxj.uphjek.com

Py:   (end - start).total_seconds()
来源：http://fxt.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://oky.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nlb.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rvf.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://esm.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://azo.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://qwd.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://aio.xuanzx.com

[J07] 比较两个日期
来源：http://rwd.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ezm.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://moz.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://lty.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://vep.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hyw.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://voj.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://lws.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://jiy.zhixingplan.top

[J08] 提取年月日与星期
来源：http://hil.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://geo.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yle.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ucx.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gxy.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ttg.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qgn.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://deu.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sxx.zhengqikj.top

[J09] 时区处理
来源：http://qvs.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zuh.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gba.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nsn.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pkg.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tqu.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zrj.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://bst.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cup.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://fzw.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hnt.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ltk.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nhd.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://edg.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lei.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qjs.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rwf.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gth.yonumen.top

================================================================================
来源：http://pwh.cucudq.cn

K. JSON 与序列化
来源：http://sus.pengpengdd.cyou

================================================================================
来源：http://drm.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://gyk.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uko.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uph.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://xba.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://use.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ihx.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://jwn.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://jke.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hgz.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://qnx.tarul.cn

Py:   json.loads(s)
来源：http://qdd.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ddk.jyoumei.cn

JS:   JSON.parse(s)
来源：http://oqm.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://tyy.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fek.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://dpf.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://fsm.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hir.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://rzj.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uuf.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cnf.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vqm.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ogo.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zvs.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tbm.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://igd.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://agr.zhongyouzk.top

[K04] 读取 JSON 文件
来源：http://cou.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vov.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qdm.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tfy.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zjd.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://adw.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://twd.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ayi.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gjw.daria6918.cn

[K05] 深拷贝对象
来源：http://oba.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://mcr.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://elw.bjfxy.top

JS:   structuredClone(obj)
来源：http://huj.yj20258.top

TS:   structuredClone(obj)
来源：http://xoh.yj20258.top

Java: // 手写拷贝构造，或序列化往返
来源：http://igr.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jni.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yrf.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cnj.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://nap.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xfg.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iae.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gtj.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cug.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ogs.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tjb.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hsa.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oks.9152youxi.cn

[K07] 进制转换
来源：http://szr.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cci.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eyk.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pqz.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xll.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ctt.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://olx.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vjn.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kiv.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://vrg.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://dgi.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ues.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://irp.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://amt.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fxp.smart0.xyz

Go:   encoding/gob
来源：http://hmt.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://bvt.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gff.iojbl.cn

================================================================================
来源：http://pcc.daxiang520.top

L. 网络请求
来源：http://qrw.sweek.top

================================================================================
来源：http://jxo.jqgfzy.top

[L01] 发送 GET 请求
来源：http://rra.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pzc.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tuv.ybcxt.top

JS:   await fetch(url)
来源：http://wkj.yangfankeji.com

TS:   await fetch(url)
来源：http://ejz.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oll.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://gah.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uhp.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bwk.tanke756.top

[L02] 发送 POST JSON
来源：http://kzz.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vle.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://duz.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cxg.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fwo.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://olq.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dww.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xna.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aig.shzxlz.cn

[L03] 设置自定义请求头
来源：http://qfj.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uck.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://seo.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qpl.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xnj.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qpl.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hft.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lzb.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://okm.cashguo.top

[L04] 设置超时
来源：http://rmr.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://ssz.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ybv.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wpw.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jtf.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jhm.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bqc.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zdm.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://luv.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://wip.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cqk.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mog.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rpp.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eyp.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yfx.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ycv.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zvq.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iic.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://ore.shangyingyoupin.top

Py:   resp.json()
来源：http://uqe.mhx1999.top

PHP:  json_decode($body, true);
来源：http://lxt.ydjk.org.cn

JS:   await resp.json()
来源：http://rsz.dashuyun.cn

TS:   await resp.json()
来源：http://pix.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pun.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://usv.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://ayh.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vqp.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://qra.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://det.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pcw.cheryme.top

JS:   resp.ok;  resp.status
来源：http://xwv.yj20258.top

TS:   resp.ok;  resp.status
来源：http://duu.ivvv.top

Java: resp.statusCode()
来源：http://pbf.zhengqikj.top

Go:   resp.StatusCode
来源：http://bqv.tianlin.xyz

Ruby: resp.code.to_i
来源：http://gyt.meibo888.top


<!-- 参考信息 -->