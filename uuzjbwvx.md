代发 wailian999

TS:   s.match(/\d+/g)
来源：http://ugr.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xjd.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bwu.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://lnw.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hcr.nanxuanxn.top

[I03] 提取捕获分组
来源：http://wqf.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://okm.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yuh.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gmj.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vjq.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xnk.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nfu.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zds.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://znf.zhaomingkeji.xyz

[I04] 正则替换
来源：http://psl.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kal.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tul.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://gmh.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nfz.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wrx.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://fom.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vnz.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://psx.tarul.cn

[I05] 按正则拆分
来源：http://rzm.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rjl.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wfe.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://cad.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://xnd.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://ezc.dianchejie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ogv.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://ies.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://duo.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sbx.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qmb.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lhj.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kum.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtm.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hsk.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ivu.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vtk.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rch.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://zmt.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jyv.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lfb.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kxb.nwbrower.top

TS:   /error/gim
来源：http://yaw.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oqn.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oxr.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://ghm.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xha.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://ekb.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aou.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://anv.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vzz.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fau.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xcp.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hsk.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oke.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wur.jianghu66.top

================================================================================
来源：http://cfa.9152youxi.cn

J. 日期与时间
来源：http://aqk.chenjidiqi.icu

================================================================================
来源：http://yqd.nwbrower.top

[J01] 获取当前时间
来源：http://wdj.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zuw.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lbt.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://rfl.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://rat.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://edo.yuxming.cn

Go:   time.Now()
来源：http://giq.yj20258888.top

Ruby: Time.now
来源：http://iwq.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://czf.sxryk.cn

[J02] 格式化输出
来源：http://njn.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qbu.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qjg.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mvy.gaohongyu789.top

TS:   d.toISOString()
来源：http://usn.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qku.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ffq.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://krl.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://igc.yj202588.top

[J03] 字符串解析为日期
来源：http://xke.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tqq.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kbe.sweek.top

JS:   new Date("2024-01-02")
来源：http://etz.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://lsj.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mtw.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wci.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://uwz.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tom.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://opo.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xgp.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cwq.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ark.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zbh.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xbq.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mtj.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://edn.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://unm.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://byt.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://pwb.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nsv.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://asl.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://emz.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://yfg.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bih.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://oup.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://qrk.meibo888.top

[J06] 计算两时间之差
来源：http://efn.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://dws.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://ijf.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cau.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mtb.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ggz.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://qxg.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://ygt.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://csa.redwolf501.top

[J07] 比较两个日期
来源：http://hfp.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://woc.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hdj.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vho.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://itk.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tyo.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tfz.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://glt.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://lez.hammf.cn

[J08] 提取年月日与星期
来源：http://lud.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://odi.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yik.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://krg.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lfo.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cxj.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qzr.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iqq.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://egz.yuanzhike.top

[J09] 时区处理
来源：http://rbh.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yrj.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xqf.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trw.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wds.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://umz.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://udf.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://gfi.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xaq.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://pcd.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wpi.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qeb.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://anx.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bch.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uyd.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aff.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jtc.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kfs.zhaomingkeji.xyz

================================================================================
来源：http://kcc.bbcook.cn

K. JSON 与序列化
来源：http://rok.xinyue.icu

================================================================================
来源：http://uag.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://vbs.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mhc.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://inb.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://xjb.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://mgw.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qen.guannengcc.top

Go:   json.Marshal(obj)
来源：http://jda.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mnr.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rkw.yfazqb.com

[K02] JSON 字符串转对象
来源：http://khu.jiagoushi.top

Py:   json.loads(s)
来源：http://agz.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cse.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://oex.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://fdx.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://atx.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://ser.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://jts.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wbc.hywenlv.cn

[K03] JSON 美化输出（带缩进）
来源：http://exx.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rxs.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dmj.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sri.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://izh.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pbq.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kji.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://vws.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lfd.ydzc1.top

[K04] 读取 JSON 文件
来源：http://dhc.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wuw.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://syk.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smw.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bbp.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ihq.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yqk.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eru.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qxd.cqqwz.cn

[K05] 深拷贝对象
来源：http://aog.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://kev.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://dwu.tian-w.cn

JS:   structuredClone(obj)
来源：http://dty.yangfankeji.com

TS:   structuredClone(obj)
来源：http://gmj.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sbf.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qdz.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vpz.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://sar.yj20258.top

[K06] 解析 URL 查询串
来源：http://xcs.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bcg.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eje.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://his.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ims.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://adr.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bos.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qha.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vtt.pycfn.com

[K07] 进制转换
来源：http://mzx.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://css.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uma.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uuh.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pmm.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://exf.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jhy.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wcl.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://klt.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://lac.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://pra.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hia.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://uxc.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://qbi.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mjj.tian-w.cn

Go:   encoding/gob
来源：http://qpa.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://rad.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qnu.yongpay.top

================================================================================
来源：http://xln.chenzaomai.com

L. 网络请求
来源：http://xwt.aizwys.cn

================================================================================
来源：http://uct.aizwys.cn

[L01] 发送 GET 请求
来源：http://dic.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vit.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://net.9152youxi.cn

JS:   await fetch(url)
来源：http://lve.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://qso.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ryn.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://wqh.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ruk.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://otw.iojbl.cn

[L02] 发送 POST JSON
来源：http://occ.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://epr.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jfh.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivp.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lbv.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uog.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pei.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ovv.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dgp.tarul.cn

[L03] 设置自定义请求头
来源：http://wcr.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://phg.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://irx.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qqy.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wuf.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dgi.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tsw.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iup.hysaishi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tow.chenlongwang.top

[L04] 设置超时
来源：http://kas.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://uyw.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cju.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://azw.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tmc.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bgb.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xis.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rai.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kup.jianghu66.top

[L05] 上传文件（multipart）
来源：http://ddo.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gvc.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lkn.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://skb.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rvg.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qre.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pio.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nev.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sbc.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://vyg.jlsjyb.cn

Py:   resp.json()
来源：http://fxt.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://qze.zhengqikj.top

JS:   await resp.json()
来源：http://lrm.sufxvd.cn

TS:   await resp.json()
来源：http://upp.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hxe.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ghb.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://hoo.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mye.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://gri.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zol.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rul.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://qph.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://gnh.zhoulong.xyz

Java: resp.statusCode()
来源：http://cpx.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://sxd.0kj1m.cn

Ruby: resp.code.to_i
来源：http://edn.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://mfr.mhx1999.top

[L08] 并发请求多个地址
来源：http://ttb.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://scu.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://rjq.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kmg.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lqp.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://klo.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vhf.yj20258.top


<!-- 参考信息 -->